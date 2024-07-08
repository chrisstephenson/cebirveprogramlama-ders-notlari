---
layout: post
title: "Önyükleme 1-1. Gün: Matematik Köyü Bilgisayar Programlama Dersinden notlar"
author: "Mehmet Gençer"
date: "July 22, 2019"
output:
  html_document: default
  pdf_document: default
categories: onyukleme
oy: 1
---

Beş yıl üstüste Şirince Matematik Köyü'ndeyiz. Bu yıl eğitim boyunca aldığım notları paylaşmaya çalışacağım. Bu notlar benzer bir eğitim yapmak isteyen eğitmenleri hedefliyor.  <http://onyukleme.mgencer.com> adresindeki ders malzemeleriyle beraber kullanıldıklarında bu notlardan destek alarak daha sorunsuz bir uygulama yapabilmelerini umuyorum

<!--more--> 

# Hazırlık

Bu eğitim için üç türden hazırlık gerekiyor. Birincisi eğitim malzemeleri. Eğitimimizin eksenini 2015 yılında benimsediğimiz bootstrapworld.org dersleri oluşturuyor. Bu dersler lise eğitim düzeyi ve içeriğine uygun olması için itinalı bir şekilde düşünülmüş. 2015'te ders malzemelerinin tamamını İngilizce'den Türkçe'ye tercüme etmiştim: <http://onyukleme.mgencer.com>. Sonraki yıllarda Bootstrapworld ekibi malzemelerini geliştirdikçe bizler de düzeltmeler yaptık (asistanlarımız Orkun Aşa ve Ege Şirin'in katkılarıyla). Sonraki yıllarda Chris orijinal içerikten farklı olarak kodları WeScheme.org yerine Racket üzerinde çalışacak şekilde uyarladı.

İkinci hazırlık eğitim koşulları. Bu eğitimin orijinali hiçbir hazırlık gerektirmeden, sadece web browser üzerinde çalışılabilecek şekilde tasarlanmış. WeScheme.org sistemi ayrıca Google drive ile de entegre olarak öğrencilerin dosyalarını bulut üzerinde saklamalarına izin veriyor. Harika. Ama ciddi bir sorun var: matematik Köyü'nde İnternet yok! Hal böyle olunca biz de eğitim malzemelerini uyarladık. Bu sisteme göre çalışabilmemiz için her öğrencinin bilgisayarında Racket (<http://racket-lang.org>) kurulu olması gerekiyor. Hazırlık olarak programın Windows/Mac/Linux versiyonlarını önceden İnternet'ten indirilmiş olarak USB drive'da getiriyoruz. Ayrıca eğitim için ihtiyaç duyacakları kod örnekleri ve şablonlarını da hazır ediyoruz. Eğitimin ilk gününde bu kurulumları yapıyoruz. 


![Ders öncesi hazırlık toplantısı]({{ "assets/onyuklemeAssets/hazirlik1.jpg" | absolute_url }}){: .postimgright}


Üçüncü hazırlık eğitim yaklaşımı ile ilgili. Biz klasik ders yaklaşımından oldukça farklı bir yaklaşım izliyoruz. Bu yaklaşım için benim tercih ettiğim tanımlardan biri "cevaplarla değil sorularla öğrenme". Esasen öğrencinin cevabı bulmasını sağlıyoruz, çünkü ancak o zaman gerçekten kalıcı bir öğrenme gerçekleşiyor. Her öğrenci ancak merak edip düşüncesini soruya yoğunlaştırdığında neden sonuç ilişkilerini kurmaya, cevapların meseleyi nasıl çözdüğünü anlamaya başlıyor. Bu yaklaşımı benimsemek eğitimci için ders malzemelerinin ötesinde bir oryantasyon gerektiriyor. Örneğin herhangi bir dersin akışı konu başlıklarından oluşmuyor. Onun yerine öğrenciler açısından sadece bir dizi problem çözme veya tasarım çalışması var. Eğitmen ise o oturum için öğretmeyi planladığı konuları bu egzersizlere yedirerek öğrenciye veriyor. Bu yüzden derse hazırlık için öğrenciye sağlanan malzeme ile eğitimcinin önündeki içerik akışı biraz farklı. Her günün öncesinde eğitim asistanlarımızla kısa bir toplantı yapıp bir sonraki günün akışını konuşuyoruz; gerekirse son dakika hazırlıkları için işbölümü yapıyoruz. Aşağıdaki bölümlerde her gün için kullandığımız problem/iş akışını ve uygulama gereklerini not etmeye çalışacağım. Ders malzemelerinin ayrıca <http://onyukleme.mgencer.com> adresinde olduğunu hatırlatayım.

# 1. gün

Planlanan akış ve gerekli malzemeler:

Saat 08:00-12:00:

1. Grup ısınma çalışması: İki kişilik oyun
1. Grup ısınma çalışması: grup oyun/hikaye tasarımı (malzeme: kalem-kağıt)
1. Çalışma ortamı için kurulumlar ve malzemelerin öğrenci bilgisayarlarına aktarımı (hazırlık: Racket 7.3 versiyonu Windows/Mac/Linux için, ve ders için gerekli kodlar)
1. Ninja kedi oyununu oynama ve oyunun sistematik analizi 
1. Klavye ve dosya sistemi kullanma egzersizi


Saat 16:00-18:00:

1. Koordinat sistemleri ve hareket ile ilişkisi. Hareketin hızda aritmetik değişiklik olarak ifadesi.
1. Fonksiyon uygulaması olarak "değerlendirme çemberleri". İçiçe aritmetik ifadeler.
1. Kodlama'ya giriş: Racket yorumlayıcısında değerler ve basit aritmetik fonksiyon ifadeleri.
1. Bootstrapworld.org'dan "Hour of code" dersi bu noktada  güzel egzersizler sağlıyor. (Biraz tekrar olmasına rağmen ders akışına ekledik, çünkü bu tekrarlar geride kalan öğrencilerin yakalamasına izin veren ancak diğerlerini de sıkmayan türden.)
1. Gün bitimi: (1) Ünite 1'deki oyun tasarımı (iş defterine girilecek) için düşünmelerini ödev olarak verdik, (2) Oyun kodunda bug'ı bulana ders döneminin sonunda ödül vereceğimizi duyurduk.


Dersliğe geldiğimizde 24 öğrencinin tamamı çoktan gelmiş, yerlerine oturmuş, bilgisayarlarını açmış vaziyetteydi. Bu hevesi görmek harika. Üniversitedeki derslerimde bunu görmeyeli çok uzun zaman oldu. 

Sınıftaki masaların bir çember şekilde dizilmesini istemiştik. Bir kare olarak dizilmişti, yine de iş görür. Buradaki amaç öğrencilerin her daim birbirlerine, yani eşitlerine bakıyor olması. Bu normal sınıf düzeninden, yani öğrencinin "üstün" bir hocaya dönük oturduğu durumdan çok farklı bir atmosfer yaratıyor. Hatta sanırım öğrenciler lise sınıflarında alışmadıkları derecede "göz önünde" hissediyorlar kendilerini. Bu yaş grubu için kalabalık önünde olmak bir stres kaynağı olabiliyor. Önce eğitimciler olarak kendimizi tanıttık. Onra herkesten ismini, hangi şehirden, okuldan geldiğini, kaçıncı sınıfta olduğunu söyleyerek paylaştı. Bu standart uygulama bile stresi aşmak için önemli bir adım.

Çalışma düzenimiz önemli bir eğitim yaklaşımını ifade ediyor. Bu öğrenciler iki hafta boyunca dinleyerek değil yaparak öğrenecekler. Bu yüzden yaptıklarını anlatacakları ve birbirlerini dinleyecekleri bir düzen olması çok önemli. Gerçekten de eğitim süresinin belki sadece dörtte birinde eğitimciler olarak biz konuşuyoruz. Kalan kısımlarda öğrenciler çalışıypr veya ürettiklerini paylaşıyor olacaklar.

Sınıf oturma düzenini bu şekilde hallettikten sonra öncelikle öğrencilere pratik bir oryantasyon verdik. Çoğu ilk kez böyle kalabalık bir kampa katılıyor. Günlük çalışma düzenimizi ve saatlerimizi, bilgisayarlarını derslikte güvenle bırakabileceklerini, dersten ayrılmaları gerekirse bize haber vermeleri gerektiği bilgisini verdik. Oryantasyonun fazlası azından her zaman iyi; onları yeni bir ortamda neyi nasıl yapabilecekleri konusunda rahatlatıyor.

Ancak öğrencileri en fazla rahatlatan şey pasif durumdan aktif duruma geçmeleri. Bunun için önceden hazırlıklıyız. İlk oturumumuza bir uyunla başladık: "Çıkartma oyunu". Oyun iki kişi oynanıyor. Oyuna başlayan bir sayı söylüyor. Diğer taraf bu sayıdan 1,2, veya 3 eksik sayıyı söyleyebiliyor. Sırayla bu şekilde çıkartma yaparak ilerliyorlar. 1 sayısına ulaşan oyunu kazanıyor. Önce oyunu ortada Chris ve Ege oynadılar ve herkesin anladığından emin olduk. Sonra öğrencileri ikişerli gruplara böldük (kendi hallerine bırakırsanız çekingen öğrenciler tek kalıyor, ve sonra iki çekingen öğrenciyi birleştirip grup yapmak zorunda kalırsınız). 10-15 dk kadar bu oyunu oynadılar. Aslında sıkıcı olabilecek bir oyun, ama nasıl bir kazanma stratejisi olabileceği merakı yüzünden bırakamıyorlar. 15 dk oynadıktan sonra gruba sorduğumuzda 3-4 öğrenci oyunu kazanmanın sırrını çözmüştü [^1].

![Grup çalışması]({{ "assets/onyuklemeAssets/gun1-grup.jpg" | absolute_url }}){:  .postimgright}

Grubun kendiliklerinden aldıkları oturma düzeninde kızlar sınıfın bir tarafına, erkekler ise diğer tarafına yığılmışlardı. Bu bir an önce halletmemiz gereken bir problemdi. Neyse ki ikinci oyunumuz bu işe yaradı. Ege'nin önerisi olan oyun için öğrencileri altı gruba ayırdık. Gruplar sırasıyla  zaman, mekan, karakter, sürpriz unsuru, tehdit unsuru, ve ödül
 alternatifleri içeren listeler hazırladılar (bkz. foto). Daha sonra her gruptan birer kişiden oluşan altışar kişilik yeni gruplar oluşturduk (kura ile) bu gruplarda herkes bir önceki grubunun listesinden bir seçim yaparak bir oyun hikayesi ortaya koydular. Bu egzersiz hem oyun tasarımına hazırlık için, ama daha önemlisi ilk saatlerden itibaren aktive olup beraber çalışarak kaynaşmaları ve rahatlamaları için çok kullanışlı.
 
Oyunların ardından oluşan atmosferle biraz daha sabır gerektiren işlere geçebiliyoruz. Bu aşamada her öğrencinin bilgisayarına gerekli kurulumları yaptık ve dosyaları kopyaladık. Daha sonra Ninja Kedi isimli oyun kodunu çalıştırıp oyunu incelemeye başladılar. Bu oyun ödülü avlamaya ve tehlikeden kaçınmaya çalışan bir ana karakteri (Ninja Kedi) olan tek kişilik bir oyun. Oyunu analiz ederek parçalarına ayırıyorlar ve onlara verdiğimiz çalışma defterindeki tabloyu dolduruyorlar. Bu şekilde her bir oyun unsurunun hareketinin hangi eksende ve ne yöne olduğunu teşhis ediyorlar. 

Bu çalışma sonrasında müfredat dışı bir egzersiz yaptık: Bir kod dosyasını kopyalama ve ismini değiştirme (dosya işlemlerini anlamaları için), içine noktalama işaretleri de gerektiren küçük değişiklikler yapma (klavyede normalde kullanmamış olabilecekleri sembollere, Shift ve AltGr modifikasyonlarına alışmaları için), ve son olarak ta bir URL ile dosya sistemi arasındaki ilişkiyi anlama. Bu egzersiz cep telefonuyla büyümüş çocukların kodlama öncesi temel becerilerinden emin olmak için. Ekan başında yaptıkları bazı şeyler beni şaşırtmaya devam ediyor; her soruna "sürükle bırak" refleksiyle tepki veriyorlar.

Öğleden sonra oturumunda koordinat sistemlerini işledik. Koordinatın değişimini hız ve zamanla ilişkili cebirsel ifade olarak gösterdik, böylece cebir kavramına girmiş oldular. Nesnelerin koordinatını değiştirmek için aritmetik işlem gerektiğini anlattık. Daha sonra aritmetik işlemleri değerlendirme çemberlerine geçtik. Böylece matematik notasyondan uzaklaşıp bilgisayar diline geçmeye hazır hale geliyorlar. Bu aşamadan sonra Racket ekranında aritmetik ifadeleri girdiklerinde çok az hata yaptılar. Bu son aşamada yapılması gerekenlerden biri veri tiplerini anlatmak. Diğeri ise Racket ekranında alacakları birkç hata mesajını görmelerini sağlamak.

Gün sonunda öğrenciler ve eğitmenlerle yaptığım kısa ropörtajları da videoda bulabilirsiniz. İlk gün bittiğinde öğrenciler beklediklerinden çok daha az kodlama yapmış oluyorlar. Ama cebir ve bilgisayar kodu ile ilişkisi hakkında önemli soyutlamaları "kapmış" oluyorlar.

{% include youtubePlayer.html id="ei-bHbRAfbg" %}

[^1]: Oyuna başlayan taraf her zaman karşıdakine 5-9-13-17-... gibi 1+4k sayı bırakırsa karşıdaki ne derse desin oyunu bu dizideki sayılar üzerinden götürebiliyor. En son 5 dedikten sonra da karşıdaki ne derse desin 1 sayısına ulaşabiliyor.