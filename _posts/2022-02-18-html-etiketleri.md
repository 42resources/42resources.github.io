---
layout: post
title:  "Html Etiketleri"
author: talhaaksoy
categories: Html
tag: Html
---

Açık kaynak topluluğunun web bölümündeki başlangıç seviyesinde olan arkadaşlar için html taglarını ve anlamlarını yazdım

---
<p>
 Öncelikle 3 temel tagımız var bunlar html,head,body
</p>
  
```html
  <html> => html tagidir site yapmaya başlarken en başa yazılır. 
    (Yazmamızın nedeni : İnternet tarayıcınız için metin ve resimlerin doğru biçimlendirilmesini sağlar.)
  <head> => html sayfamızın config kısmı gibi düşünebiliriz css dosyalarımı meta etiketlerimizi site titlesini vs. ayarlar burda yapılır
  <body> => sitenin gözüken kısmıdır görüntülenecek herşey burda olur
  
```
---
<p>Head dosyasının içine yazdıgımız tagler</p>

```html
  <title> => Sitenin sekme kısmında gözüken (genelde sitenin adının) yazılı olduğu kısım
  <style> => yerel css oluşturmak için yazılır ve css burada yazılabilir (fazla tercih edilmez)
  <link> => dışardan css vs. gibi dosyaları kendi dosyamıza bağlamak için kullanılır (ör : harici css)
  <meta> => karakter sınıfı (ör : utf - 8), sitenin yapımcısının adı,anahtar sözcükler, 
            sayfanın görünümüyle ilgili birkaç şeye de burdan erişebiliyomuşuz
  <script> => src özelliği de eklenip harici js dosyası bağlanabilir ve ya yerel js yazılabilir, 
    genel olarak head kısmına ya da body kısmının en aşağılarına yazılır.
```

<p> basit bir head örneği </p>

```html
  <head>
	  <meta charset="UTF-8">
	  <meta http-equiv="X-UA-Compatible" content="IE=edge">
	  <meta name="viewport" content="width=device-width, initial-scale=1.0">
	  <title>Document</title>
    <link rel="stylesheet" href="style.css">
    <script src="./jquery.js" type="text/javascript"></script>
  </head>
```
---

<p> body etiketleri </p>

```html
  <div> => htmlin kalbidir sitedeki herşey bunlarla yapılır , kutucuklardır ve bunlar özelleştiririz.
  <address> => adındanda anlaşılacağı gibi adres yazarken kullanabiliriz.
  <map>, <area> => iç içe kullanılırlar mapin içinde bir resim olur,
    area ile resmin belirli kordinatlarını işaretleyip o alanı ayırırz,
    ve o alana tıklandıgında farklı resimler gösterebiliriz (denemek için => https://www.w3schools.com/tags/tryit.asp?filename=tryhtml_areamap)
  <article> => makale yazmak için kullanılır (içine <h1[burdaki sayı 6 ya kadar çıkabilir]>, ve <p> etiketleri kullanılır)
  <h[1,2,3,4,5,6]> => başlık etiketidir sayı ne kadar küçükse başlık o kdr büyük
  <p> => paragraf yazmak için kullanılır
  <audio> => siteye ses eklemek için kullanılır
  <b> => kalın yazı yazmak için kullanılır
  <a> => sayfaya tıklanılabilir link adressleri koymak için (ör : <a href="google.com">Google</a>)
  <br> => eklediğimiz elemandan sonraki elemanları bi alt satıra götürür. (denemek için => https://www.w3schools.com/tags/tag_br.asp)
  <button> => sayfaya buton eklemek için
  <code> => içine yazılan kodları normal yazılardan daha farklı gösterir.
  <data> => elemanların içine değer girmek için (ör: https://www.w3schools.com/tags/tag_data.asp)
  <datalist> => girip sayfasından bakmanız daha açıklayıcı olur (ör :https://www.w3schools.com/tags/tryit.asp?filename=tryhtml5_datalist)
  <del> => yazının üstümne çizgi çeker silinmiş gibi gösterir.
  <details> => içine eklenen yazıya detay eklememizi sağlar yazıya tıklayınca detay gözükür (ör: https://www.w3schools.com/tags/tryit.asp?filename=tryhtml5_details)
  <dialog> => yazıyı dialog kutucuguna alır 'open' parametresini girerseniz gözükür. (ör: https://www.w3schools.com/tags/tryit.asp?filename=tryhtml5_dialog)
  <figcaption> => resmin altına 'resim yazısı yazmak için kullanılır' (ör: https://www.w3schools.com/tags/tryit.asp?filename=tryhtml_figcaption)
                  resim ve etiketin kendisi <figure> diye bi etiketin arasında kullanılır.
  <footer> => sitenin en alt kısmını burada yazarız.
  <form> => içine form elemanları koyarız [input etiketi sayesinde] (ör :https://www.w3schools.com/tags/tag_form.asp)
  <header> => sitenin üst menü kısmını yaparken kullanırız.
  <i> => italik yazmak için
  <img> => resim koymak için
  <ins> => yazıyı altı çizili yapmak için / <u> => yazıyı altı çizili yapar
  <mark> => yazının arkasını sarı yapar, vurgular.
  <meter> => içine değerleri verilerek, belirli bir kısmı dolu bar oluşturulur (ör: https://www.w3schools.com/tags/tryit.asp?filename=tryhtml5_meter)
  <select>, <option> => açılır liste yapmak için kullanılır selectler içine seçenek olarak option girilir. (ör: https://www.w3schools.com/tags/tryit.asp?filename=tryhtml_select)
  <textarea> => yazı yazmak için bi alan oluştulur textbox gibidir istenilirse boyutu değişken bırakılabilir, istenilirse sabitlenir
  <ul>, <li> => ul liste oldugunu belirtir li liste elamanıdır ve ul'nin içine yazılır
```

---

<p>Markdown dosyamızda yani şu anda okudugunuz dosyada da html elemanları kullandım işte örneği</p>

![markdown resmi](/assets/html-etiketleri/code.png)

---

<p> Arkadaşlar body etiketleri uzun sürdü ben size çok kullanılanlar ve işinize yarıyabilecek olanları yazdım unuttuklarım olabilir söylerseniz eklerim </p>
<p> Youtube Kanalımı Takip Ederseniz Hoş Olur => <a href="https://www.youtube.com/channel/UCDc0WPgvJkfThIAu4VcPDtQ">Youtube : Alhazen TR</a>
<p> Github Hesabım => <a href="https://github.com/TalhaAksoy">Github</a>
