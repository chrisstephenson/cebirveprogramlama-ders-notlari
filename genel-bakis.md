# Cebir ve Programlama Yaz Okulu - Genel Bakış

## Özet

* Yaz okulumuz birer haftalık (6şar gün, günde 6 saat) iki modülden oluşur. İlk modüle "cebir", ikinci modüle "evren" kod adılarını kullanıyoruz. 
* Eğitimin tamamı boyunca öğrenciler kendi tasarladıkları bir oyunu hayata geçirirler. Bunu yaparken lise müfredatında (matematik ve fizik dersleri) öğrendikleri konuları tekrarlayıp pekiştirirler. 2011 yılında bu eğitimlere başladığımızda çıkış noktası olarak aldığımız [http://bootstrapworld.org] girişimi bu konuları ABD lise müfredatındaki konularla net olarak eşleştiriyor, ancak bizim müfredatlar değişken olduğundn biz bunu (denedikse de) yapmıyoruz.
* İlk modülde öğrenciler kendilerine verilen oyun şablon kodundaki belirli fonksiyonları doldurarak çalışırlar. İkinci modülde ise sıfırdan kod yazarlar ve ilk modüle ilaveten veri yapılarını öğrenirler.

## Uygulama

* Kara tahtada ders anlatıyoruz. Öğrenciler kendi laptop'larında çalışıyorlar. İnternet yok. Bu yüzden eğitimin başında öğrencilere bir yazılım kiti veriyoruz. İçerisinde kullanacakları yazılımlar ve kod örnekleri var.
* Ayrıca her öğrenciye egzersiz yapmaları için basılı birer çalışma defteri dağıtıyoruz. 
* Eğitimin orijinali [http://wescheme.org] online aracı üzerinde yapılıyordu. Ancak köyde internet olmadığından biz DrRacket isimli programı kurarak çalışıyoruz.
* Ders anlatımından ziyade temel kavramların paylaşılması, öğrencileri aktive edici sorular yöneltmek, ve onların farklı yaklaşımlarını sınıfla paylaşmalarını sağlamak yoluyla katılımcı bir öğrenme faaliyeti yürütüyoruz. 
* Her modülün son günü yeni konu işlemek yerine öğrencilerin kodlarında son düzeltmeleri yapmaları ve herkesin sırayla ortaya çıkardığı işi sınıfa sunarak paylaşmasına ayrılmıştır.
* Modül boyunca oyun tasarımı için gerekli temel becerileri geliştiren egzersizler yapılır. 

## Programlama dili

* Scheme veya Racket olarak adlandırılan dil 'fonksiyonel dil' grubundadır. Eğitim amaçlı tasarlandığından sadece algoritma geliştirmek için gerekli en temel özelliklere indirgenmiştir. Örneğin değişken kavramı yoktur.
* Bu yüzden dilin kurallarını öğrenmek son derece hızlı olmaktadır.
* Öğrenciler programlama dilinden ziyade doğru programlama yöntemlerini öğrenirler. Örneğin "tasarım reçetesi" öğrencileri bir fonksiyon yazmadan önce fonksiyonun girdi ve çıktılarını tasarlamaya, kodlarını dökümante etmeye teşvik eder. "Test first programming" tekniği kodu yazmadan önce testleri yazmayı gerektirir, vb.

## Konu akışı

Yaklaşık konu akışı aşağıdadır. Bu akış grubun genelinin gidişatına göre esneyebiliyor:

**MODÜL 1: CEBİR (6 gün)**

Bu modülde öğrenciler örnek oyunu ve oyun şablon kodunu kullanırlar.

1. İlk gün dersi örnek oyunun analizi ve oyunda olup bitenlerin teşhisidir. Kaynaştırma egzersizi ile başlıyoruz. Sonrasında öğrenciler kendi oyunlarını tasarlarlar: oyun kahramanı, tehlike, ödül, arkaplan gibi unsurlara karar verirler. Sonrasında DrRacket ile basit komutlarla programlama dilinin kurallarını keşfetmeye başlarlar. Bu noktadar "değerleme çemberi" kavramı kullanılır.
2. 


**MODÜL 2: EVREN (6 gün)**

Bu modülde öğrenciler sıfırdan kod yazarlar ve DrRacket/WeScheme sistemindeki big-bang adlı evren simülasyonu kitaplığını kullanırlar.

1. Bu modülün ilk gününde öğrenciler veri yapısı kavramı ile tanışır. 