---
layout: post
title: "Önyükleme 1-5. Gün: Matematik Köyü Bilgisayar Programlama Dersinden notlar"
author: "Mehmet Gençer"
date: "July 27, 2019"
output:
  html_document: default
  pdf_document: default
categories: onyukleme
oy: 1
---

Beşinci ve ilk dersin sonuncu günü. Bugün hedefimiz oyunu bitirmek ve ilk haftayı bir oyun sunumu seansıyla taçlandırmak.

<!--more--> 

# 5. gün

Ders akışı:

Saat 08:00-12:00:

1. Ünite 7: Koşullu işlemler (parçalı fonksiyonlar)
1. Ünite 8:  Pisagor teoremi ve oyunda çarpışma kontrolü


Saat 16:00-18:00:

1. Ünite 9: Oyun sunumu

Güne mantıksal cebirle algoritmaları birleştiren koşullu işlemlerle başlıyoruz. Bunlar da mantıksal cebir gibi kolay görünüyorlar. Yine de matematikteki parçalı fonksiyon kavramı (partial function) bilgisayarın "karar verme" eyleminin temelini oluşturuyor. Yan, belli durumlarda şu şekilde hesap yaparken başka bazı durumlarda başka türlü hesap yapmasını sağlıyor. 

Ayrıca koşullu işlemler algoritmalardaki çok temel bir mekanizmanın da temeli: döngüler. Döngüler Racket/Scheme gibi fonksiyonel dillerde özyineleme (recursion) ile kuruluyor. Diğer diller (Python, Java ,vb) ise farklı bir kurgu sağlıyor: for/while vb. döngüler. Ne var ki sadece özyinelemenin matematiksel bir karşılığı var. Yani hesaplama kuramında yeri var. O yüzden yeni programcılara bu kurgunun öğretilmesi gerekiyor. Ancak bu derste o kadar ileri gitmeyeceğiz. Döngüler/özyineleme bu yaş grubunun soyutlama becerilerinin sınırlarını biraz zorluyor. O yüzden bir "ilk" derste buna girmeyi tercih etmiyoruz. Ne varki sınıftaki iyi öğrencilerin en çok sorduğu konu bu: "birden n'e kadar sayılar için bir işlemi tekrarlamayı ne zaman öğreneceğiz". Sorarken çoğu adının "döngü" olduğunu bilmiyor, ama for veya while kullanmışlar. Kültürümüzde kavramın değil teknolojinin önemsenmesinin tipik bir örneği. İnsanların kullanmayı bilmediği, kavramsallaştıramadığı aletlerle elinin kolunun ve aklının tıkanmasına neden oluyor. En aklı başında şirket yöneticileri bile aynı hataları yapıyor. Yine de işte döngüler onlar için sonsuzluğa uzanan güçlü bir araç gibi, çok sayıda tekrar yapabilmenin gücünü istiyorlar. "Önce matematiksel kavramı öğrenmeniz gerek, bu derste buna zaman yok" cevabı onları ikna etmiş görünmüyor. Zaten hiçbirşeye zaman yok, hele durup düşünmeye. Zamanın ruhu bu.

"if" kullanan parçalı fonksiyonlarla egzersizler bütün gün sürüyor. İlk etabın sonunda oyundaki unsurların ekrandan dışarı  çıkıp çıkmadığını tespit edebilen fonksiyonalrı yazdılar ve ekrandaki hareket daha gerçekçi görünmeye başladı. 

Bugün zorlandıkları şeylerden biri de şu: kodları geliştikçe ifadeler daha uzun ve karmaşık olmaya başladı. Aslında ifadelerin nasıl parçalardan oluştuğu konusunu anlıyorlar. Ancak beş aritmetik işlem, iki karşılaştırma, ve bir mantıksal operatörden oluşan ifadelerle başetmek konusunda zorlandılar. Bu noktada iki pratiğin altını çiziyoruz: (1) kodlamadan önce çözümü kağıt üzerinde geometrik çizimler ve sembollerle ifade etmeleri, yani koddan önce kafada çözmeleri, ve (2) kodlarını girintileme ve birden fazla satıra bölme gibi pratikleri takip etmeleri. Ne yazık ki bunların herbiri biraz bocalamadan ders alarak ancak olabiliyor.

Son olarak Pisagor teoremini de kodlayarak oytundaki şeylerin çarpışma kontrolünü yapabiliyorlar. Bu kısımda sadece çok sıradışı görseller kullanan öğrenciler biraz bocalıyor çünkü internetten indirdikleri görsel kalite, çözünürlük ve boyutları sorun çıkartıyor.

Gün sonunda herkes oyununu bitirmişti. Sırayla kısaca anlattılar. Onlardan ayrıca hafta boyunca zorlandıkları ve keyif aldıkları şeyleri de paylaşmalarını istedik. Videoları editledikten sonra kısa süre içinde bu sayfaya ekleyeceğim.