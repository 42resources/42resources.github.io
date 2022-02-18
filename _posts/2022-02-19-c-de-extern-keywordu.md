---
layout: post
title: "C Dilinde extern Anahtar Kelimesi"
author: mkaramuk
category: C
---

Merhaba Dünya!

Bu yazıda sizlere C programlama dilinde `extern` anahtar kelimesinin ne işe yaradığından bahsedeceğim.

Normalde global olarak tanımlanan bir değişkenin kullanılabileceği aralık sadece bulunduğu kaynak dosyasıdır. Bu demektir ki **A.c** içerisinde global olarak tanımladığımız bir değişkene **B.c** dosyası içerisinden erişemeyiz. `extern` olmasaydı :)

`extern` anahtar kelimesi sayesinde herhangi bir kaynak dosyamızda tanımladığımız global bir değişkene erişebiliyoruz.
Aşağıdaki örneklere bakalım:

**other.c**

```c
int sayi = 42;
```

**main.c**

```c
#include <stdio.h>

int main() {
}
```

**other.c** içerisinde bulunan **sayi** değişkenine ulaşmak için **sayi** değişkeninin **main.c** içerisinde extern ile bildirimini yapmamız gerekiyor.

**main.c**
```c
extern int sayi;
```

Dikkat ettiyseniz değişkenin sadece bildirimini yapıyoruz. Yani değer atamıyoruz. Bu bizim derleyiciye "bu değişken programın bir yerlerinde tanımlı" dememiz anlamına geliyor. Farklı dosyalardaki fonksiyonları kullanmak için prototiplerini bildirmemiz  gerekir. Farklı dosyalardaki global değişkenlerimize erişebilmek için ise `extern` anahtar kelimesi gerekir. Dosyaların son halleri aşağıdaki gibidir:

**other.c**
```c
int sayi = 42;
```

**main.c**
```c
#include <stdio.h>

extern int sayi;

int main(void)
{
	printf("Merhaba %d!\n", sayi);
	return (0);
}
```

### Kaynaklar
[kadifeli.com - Standard C Programlama Dili](https://www.kadifeli.com/fedon/stdcprtr.php?4_3_4)
[ckaynak.com](https://ckaynak.com/c-programlama-dili-depolama-sinifi-belirtecleri-auto-extern-static-register-1112)
