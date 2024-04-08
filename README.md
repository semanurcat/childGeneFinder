# childGeneFinder



Bu proje, "Kalem" kelimesini oluşturmayı amaçlayan basit bir genetik algoritma simülasyonudur. C dilinde yazılmış olan bu simülasyon, başlangıçta rastgele seçilmiş iki ata (anne ve baba) üzerinden, rastgele mutasyonlar ve çaprazlamalar yaparak yeni nesiller üretir. Program, hedef kelimeye ulaşana kadar yeni nesiller oluşturur ve bu süreçte kaç nesil geçtiğini kaydeder.


### Önkoşullar

Bu programın çalıştırılabilmesi için sisteminizde C dilini derleyebilecek bir ortamın kurulu olması gerekir.


Program çalıştırıldığında, "Kalem" kelimesine ulaşana kadar devam eden nesilleri ve her nesil için üretilen çocukları gösterir. Program, hedef kelimeye ulaştığında kaç nesil geçtiğini ekrana yazdırarak sonlanır.

## Programın İşleyişi

-**Değişken Tanımlamaları:** Karakter dizileri ve sayısal değişkenler tanımlanmıştır. Bu değişkenler genetik algoritmanın çalışması için gerekli olan bilgileri saklar.

-**ciftlestir Fonksiyonu:** Anne ve baba genlerinin birleştirilmesiyle yeni bir çocuk üretilir. Her gen için, %50 şansla babadan, %45 şansla anneden gen alınır ve %5 şansla genHavuzundan rastgele bir gen seçilir. Üretilen her çocuğun "saglik" durumu, "Kalem" kelimesi ile ne kadar benzer olduğuna bağlıdır (benzer gen sayısı).

-**kontrol Fonksiyonu:** Üretilen kabile üyelerinin (çocukların) içinde hedef kelimeye ("Kalem") tam olarak uyan bir birey olup olmadığını kontrol eder. Eğer varsa 0 döndürür ve döngü sonlanır.

-**sirala Fonksiyonu:** Kabile üyelerini sağlık (hedef kelimeye benzerlik) durumlarına göre sıralar ve en sağlıklı iki bireyi yeni anne ve baba olarak seçer.

-**main Fonksiyonu:**

Program başlatıldığında, ilk nesil için 5 çocuk üretir.
Üretilen çocuklar ve sağlıkları ekrana yazdırılır.
Daha sonra, bu çocuklar sağlıklarına göre sıralanır ve en uygun anne-baba belirlenir.
"Kalem" kelimesi elde edilene kadar yeni nesiller üretilmeye devam eder.
Hedef kelime elde edildiğinde, kaç nesil geçtiği ekrana yazdırılır.
