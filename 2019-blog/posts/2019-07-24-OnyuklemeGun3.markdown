---
layout: post
title: "Önyükleme 1-3. Gün: Matematik Köyü Bilgisayar Programlama Dersinden notlar"
author: "Mehmet Gençer"
date: "July 24, 2019"
output:
  html_document: default
  pdf_document: default
categories: onyukleme
oy: 1
---

Eğitimin üçüncü günü: Fonksiyon tasarlamaya alışmaları zaman alıyor. Gün içerisinde animasyonlara başlıyoruz. Bu kısmına bayılıyorum.

<!--more--> 

# 3. gün

Ders akışı:

Saat 08:00-12:00:

1. Ünite 3 sonrası: Tasarım reçetesi tekrar ve pekiştirme egzersizleri.


Saat 16:00-18:00:

1. 4. ünite: Roket animasyonu
1. Oyun nesnelerini hareket ettirme
1. 5. ünite: Oyun animasyonu


Öğrencilerden çoğunun daha önce kodlama yapmış olması bir talihsizlik! Öyle kötü kodlama alışkanlıkları edinmiş olarak geliyorlar ki. Fonksiyon tasarlama aşaması tam olarak bir bataklık olabiliyor hem biz hem de onlar için.

![Foto 1]({{ "assets/onyuklemeAssets/gun3-Ata.jpg" | absolute_url }}){: .postimgright}

Bu yüzden ünite 3'ten 4'e geçerken bu bataklığı arkada bıraktığımızdan emin olana kadar tekrarlar ve problem çözme egzersizleri yapıyoruz. Bataklığın bir sebebi daha önce kodlama yapmış öğrencilerin bizim ders notlarında **tasarım reçetesi** dediğimiz **test first programming** yaklaşımına direnç göstermeleri. Bu öğrenciler fonksiyon sözleşmesi ve örnekleri yapmadan fonksiyon tanımına atlamayı "cool" buluyorlar. Racket'ta contract denilen  sözleşme "strict typing" olmayan bir dilde ancak dökümantasyon için kullanılır (Python'daki gibi) ama tasarım süreci açısından ilk adım bu: yapılacak işin şeklini belirliyor. 

Bataklığın ikinci sebebi diğerlerine göre bu aşamada yavaş giden öğrenciler. Örneğin değişken tanımlama ile parametrik fonksiyon tanımlama arasındaki farkı anlamakta zorlananlar oluyor. Bunun için her örneği önce matematik dilinde sonra kodlama dilinde ayrı ayrı anlatmak önemli.

![Foto 1]({{ "assets/onyuklemeAssets/gun3-EgeSirinVeOgrenciler.jpg" | absolute_url }}){: .postimgright}

Tekrar oturumunda bir sayının karesini alma örneği yaptık. Tasarım reçetesini Chris'in modifiye ettiği kitaplıklardaki Türkçe test fonksiyonuyla yapıyoruz. Bu kitaplığı aktifleştirmek için ders notlarında [cebir ders malzemeleri](http://onyukleme.mgencer.com/onyukleme1/kodlar) dizininde bulunan dosyayı şu şekilde alıyoruz (working directory'ye dikkat ederek yapın)::

    (require "Teachpacks/bootstrap-teachpack.rkt")


sonrasında tasarım reçetemizi uygulayabiliriz::

    ;(1) SÖZLEŞME
    ; kareAl: sayı --> sayı
    ;(2) ÖRNEKLER
    (ÖRNEK (kareAl 2) (* 2 2))
    (ÖRNEK (kareAl 5) (* 5 5))
    ;(3) TANIM
    (define (kareAl x) (* x x))
    
  
Bunun arkasından bir sayının 4. kuvvetini alma örneği yaptık. Bu son derece renkli bir örnek oldu. Çünkü kimi öğrenciler ilk yaptıkları fonksiyonu kullanırken kimileri bambaşka şeyler yaptılar::

    (define (dördüncüKuvvet x) (* x x x x))
    (define (dördüncüKuvvet x) (* (kareAl x) (kareAl x)))
    (define (dördüncüKuvvet x) (kareAl (kareAl x)))

Bunları karşılaştırmak çok yararlıydı. Ayrıca son örneğin sadece iki çarpma işlemi yaptığını, ilk ikisinin ise sonucu ancak üç çarpma işlemiyle bulduğunu gösterdik. Avrupanın sıcak dalgasıyla boğuştuğu günlerde bu farkın, yani hesaplama verimliliğinin  bilgisayarlardan kaynaklı enerji tüketimine ve dolayısıyla küresel ısınmaya nasıl bağlı olduğunu konuştuk.

![Foto 1]({{ "assets/onyuklemeAssets/gun3-Satsi.jpg" | absolute_url }}){: .postimgright}


Hala ünite 3 ile ünite 4 arasında pekiştirme problemlerine devam ediyoruz. Bir sonraki örneğimiz iki daireyi üstüste çizerek halka yapma. Sonra Pisagor teoremi uygulayarak hipotenüs bulma. Burada bir cebirsel bir görsel problem diye gitmenin yararlı olacağını düşündük. Sonra bir kare üstüne yarı büyüklükte başka bir kare oturtma problemi, sonra iki sayının ortalamasını alma problemi gibi.

Öğleden önce sindire sindire tasarım reçetesi alıştırmaları yaptıktan sonra öğleden sonra basit bir animasyonla başladık: 4. ünitenin başındaki roket animasyonu. Eğlenceli, ayrıca hiç sorun çıkmadı. Hatta üstüne ivmelenen roket yaptık. 

En son etapta oyun taslağını açtılar ve artık nesne, tehlike vb. hareket ettiren fonksiyonları bulup animasyondan öğrendikleriyle değiştirebiliyorlar. Yani 5. ünite. Böylece uzun bir pekiştirme etabının ardından inanılmaz bir hızla iki  saatte iki ünite yapmış oluyoruz.

Hepsi büyük bir heyecanla günü bitirdi. Yoruldular, ama Perşembe matematik Köyü'nde tatil, güzelce dinlenecekler.

Günün sürprizi ise geçen seneki öğrencilerimizden Canay'ın ziyareti oldu. Videoda (aşağıda) dersimizle ilgili söledikleri bizi bayaa bir duygulandırdı.

{% include youtubePlayer.html id="0hlxi4NdOqg" %}


Üçüncü günün sonunda Chris Stephenson ve Tuğba Yıldız hocalarımız ve benim kısa videolarımız da aşağıda. 

{% include youtubePlayer.html id="2_kRWdJG1WU" %}

{% include youtubePlayer.html id="tf3_t3oeat8" %}


