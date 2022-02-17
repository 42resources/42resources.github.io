---
layout: post
title:  "Python ile get-next-line için test dosyaları oluşturmak"
author: erengun
categories: Python C
tag: Python
---

Herkese selamlar 👋🏽,

umarım gününüz güzel geçiyordur. Bugün sizlere evolarımda gösterdiğim get-next-line için yaptığım python text dosyası oluşturucusunu göstermek istiyorum.

Kodu oldukça basit sadece 4 line (gerçekten). 

Python bilgisine ihtiyacınız yok :D

Evolarda hepimizden main istiyorlar ve genel olarak yazılan mainler şuna benzer:

```c
	#include <fcntl.h>
	#include <stdio.h>

	int   main(int argc, char **argv)
	{
	  int   fd;
	  char *c;

	  fd = open("test.txt", O_RDWR);
	  c = get_next_line(fd);
	  //tüm lineları tek seferde okutmak istediğim için şartı böyle yaptım 
	  //dosya sonuna geldğimiz zaman fonksiyonumuz 0 dondürecek ve döngüden çıkacak
	  while(c)
	  {
	    printf("%s",c);
	    free(c);
	    c = get_next_line(fd);
	  }
	  // Leak kontrolü için kullanabilirsiniz
	  //system("leaks a.out");
	}
```

## Peki test.txt dosyasını nasıl oluşturucaz

Bunun için biraz python kullanabiliriz 😉

Öncelikle `open` fonksiyonu ile dosyayı tanımlamamız gerekiyor.

[open fonksiyonu hakkında daha fazla bilgi için](https://www.w3schools.com/python/ref_func_open.asp)

```python
	fd = open("test.txt", "w")
```
Open fonksiyonun aldığı ilk değer "dosyaadı.uzantı" ikincisi ise üzerine yazacağımız için "w" yazdık

![open fonksiyonu flagleri](/assets/python-get-next-line/flags.png)

Dosyayı okuduk şimdi de write ile yazma işlemini yapalım.

```python
	for i in range(1000):
		fd.write(f"satır numarası : {i}\n")
```
`Range`'in içine istedğiniz satır sayısı numarasını yazabilirsiniz. Ben 1000 yazdım.

`write(f"yazı {degisken}")` ile de i'nin değerini `satır numarası : 1` gibi yazdırdık.

Yazma işlemini bitirdik şimdi de `close` ile işlemi bitirebiliriz.

```python
	fd.close()
```

Kodumuzun son hali şu şekilde.

```python
	fd = open("test.txt", "w")
	for i in range(1000):
	fd.write(f"satır numarası : {i}\n")
	fd.close()
```

NOT: Dosyayı önceden oluşturmak zorunda değilsiniz. Dosya yoksa bile kod çalıştığında otomatik oluşturuluyor.

## Sırada çalıştırması var

Çalıştırması oldukça basit tek yapmanız gereken

```bash
	python3 doysyaadi.py
```

## (Bonus) main örnekleri

Bonus olarak size bikraç main örneği göstermek istiyorum. Maini yazarken `argv` kullanınca çok tatlı oluyor 😄

```c
	#include <fcntl.h>
	#include <stdio.h>
	
	// argv ile dosya adını terminalden alabiliriz
	int   main(int argc, char **argv)
	{
	  int   fd;
	  char *c;
	
	  //terminalden girilen dosyayı okutuyoruz.
	  fd = open(argv[1], O_RDWR);
	  c = get_next_line(fd);
	  while(c)
	  {
	  	printf("%s",c);
		// leak oluşmaması için yazdıktan sonra freeliyoruz.
	    	free(c);
	    	c = get_next_line(fd);
	  }
	  // Leak kontrolü için
	  //system("leaks a.out");
	}
```

Çalıştırması da oldukça basit tek yapmanız gereken:

```bash
	./a.out dosyaadi
```

Bugünlük benden bu kadar yazdığım koduları [github](https://github.com/Erengun) hesabımda paylaştım. Sorularınızı slackten sorabilirsiniz :D
