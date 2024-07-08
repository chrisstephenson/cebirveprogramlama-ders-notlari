---
layout: post
title: "Önyükleme 1-2. Gün: Matematik Köyü Bilgisayar Programlama Dersinden notlar"
author: "Mehmet Gençer"
date: "July 23, 2019"
output:
  html_document: default
  pdf_document: default
categories: onyukleme
oy: 1
---

Eğitimin ikinci günü: kodlama, fonksiyon kavramı, değişken kavramı ve Racket dilinde tanımlanması ile küçük programlar yazmaya başlıyorlar 

<!--more--> 

# 2. gün

Ders akışı:

Saat 08:00-12:00:

1.  Önyükleme Ünite 2: Değerlendirme çemberi tekrar egzersizleri.
1. Ünite 2: Farklı veri tipleri ile çalışan fonksiyonlar: görseller ve metinleri kullanma
1. Ünite 2: Fonksiyon sözleşmeleri
1. Görüntü üreten fonksiyonlar.
1. Değişken tanımlama
1. Oyun tasarımı
1. Oyun kodunu değiştirme

Saat 16:00-18:00:

1. Önyükleme Ünite 3: Değişken tanımlama
1. Ünite 3: Fonksiyon tanımlama.


![Gün 2]({{ "assets/onyuklemeAssets/gun2-genel-kucuk.jpg" | absolute_url }}){: .postimgright}

Gün değerlendirme çemberinin tekrarı ile başlıyor. Çünkü bu çemberler görsel olarak Racket/Scheme dillerindeki parantez, fonksiyon, ve parametrelerine birebir denk düşüyor. Matematiksel ifadelerin dilinden değerlendirme çemberine ve ondan da Racket koduna geçiş öğrencilere Racket dilinin sözdizimi kurallarını anlatmanın en iyi yolu.

Hemen sonrasında öğrenciler için en keyifli etaplardan biri: görseller üreten fonksiyonlar. Bu noktada "circle", "star", "ellipse" ve diğer fonksiyonları kullanıyorlar. Bu noktada yaşadığımız bir güçlük Racket kitaplıkları ile ilgili oldu. Görüntü fonksiyonları birkaç kitaplıktan gelebilir. Racket standart teachpack/kitaplığı 2htdp/image, yani Felleisen ve ekibinin üniversite lisans dersinde kullandığı. Bootstrap ekibi ise bootstrap diye bir teachpack. Bu detayı kaçırdığımız için kısa bir bocalama yaşıyoruz. İnternet olsaydı WeScheme ile bu sorunları hiç yaşamayacaktık. Bir dahaki sefere hazırlık aşamasına bu detayı da eklemek gerekiyor.

Bu aşamada fazla ilerlemeden "fonksiyon sözleşmesi" kavramına girmek gerekiyor. Sözleşme bir fonksiyonun hem kullanım kılavuzu hem de tasarım şeması. Öğrenciler hemen "bu ne işe yarıyor" diye soruyorlar. Çünkü sözleşme kodun yeni "numara"lar yapmasını sağlayan birşey değil. Burada teknoloji odaklı ve sabırsız bir nesil var ve onları ikna etmek gerekiyor. Ne var ki sözleşmelerin değeri ancak eğitmenin hafta boyunca inadı ile yavaş yavaş idrak edilebilecek bir konu. Bu noktada yapabileceğiniz en iyi şeylerden biri Racket dökümantasyonunu onlara göstermek ve görüntü üreten fonksiyonları keşfetmelerini sağlamak. Bunu yaparken fonksiyon sözleşmelerini inceleyip kullanıyorlar ve bunun ne işe yaradığını biraz olsun hissetmiş oluyorlar.

Bizim dersimizde orijinal Bootstrap dersine göre daha fazla süre var. Bu yüzden bu aşamada biraz görüntü fonksiyonlarına dalıyoruz, çünkü onları cezbediyor ve derse angajmanlarını arttırıyor. Görüntü birleştirmeye yarayan "overlay", "beside", "put-image" gibi fonksiyonları anlatıp küçük challenge'lar veriyoruz: mesela bir ev yapma (kare bina üstüne üçgen çatı) gibi. Bu egzersizlerin yazım hatalarını deneyimlemek, hata mesajlarını okumak, klavyede normalde kullanmadıkları sembollere alışmak gibi yararları oluyor.

Bunun ardından değişken tanımlama geliyor. Burada ihtiyacı tarif etmek için önce onlardan basit bir ev çizmelerini istedim:

    (above
      (triangle 50 "solid" "red")
      (square 50 "outline" "black"))

Sonra da "bir mahalle çizmek istesek nasıl yaparız?" sorusunu sordum. Bunun üzerinde define fonksiyonu tam da yerini buluyor. Define ile ilgili olarak (1) hiç bir değer döndürmediği, ve (2) ikinci parametrese herhangi bir değer alabileceği için sözleşmesinin bir tuhaf olduğunu not etmek gerekiyor. Daha sonra yukarıdaki ifadeyi bir ev olarak tanımladılar::

    (define ev
            (above
              (triangle 50 "solid" "red")
              (square 50 "outline" "black")))


Bunun ardından uyun tasarımına geçtik. Oyunlarında kullanacakları karakterleri, tema ve arkaplanı düşünüp not aldılar. Bunları uzun uzun paylaşıyoruz, hem grubun etkileşimi için iyi oluyor hem de çok eğlenceli, sivri fikirler var ve herkesi eğlendiriyor. Bunlardan birkaçını videoda paylaşıyorum.

{% include youtubePlayer.html id="RYbrJ-18_28" %}

Bunu da bitirince oyun kodunu açıyorlar. Ders notlarındaki akışa uygun olarak önce tanımları bulup interaktif ekrandan yazdırıyorlar (örn. oyun ekranı başlığı). Sonra da tespit ettikleri define'ları değiştirerek oyunu biraz kişiselleştiriyorlar. 



Tanımlarla Tuba hocamız bol bol egzersiz yaptırdı. Bu arada görüntü işlemek için rotate, scale, above, aside gibi birçok fonksiyonu da öğrenmiş oldular. Bunları yaparken zaman zaman Racket-2htdp/image kitaplığı ile bootstrap kitaplığı arasında sinir bozucu farklar buluyoruz. Bütün bunlar WeScheme kullanamamanın sonucu. Ama doğrusu öğrencilerin İnternete takılarak dikkatlerinin dağılmaması bu sıkıntılara değer.

Günün ve 3. ünitesin son etabında fonksiyon tanımlarına geçiyoruz. Chris Bootstrap'in en keyifli taraflarından olan tümevarımla fonksiyon tanımlama konusunu anlatıyor: yani birkaç örnek yazıp sonra genelleyerek fonksiyonu tanımlamayı "çocuk oyuncağı" haline getiriyoruz.


