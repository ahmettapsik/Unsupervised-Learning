# Unsupervised-Learning

#MAKİNE ÖĞRENMESİ NEDİR


Makine öğrenmesi, insanların öğrenme şekillerini taklit etmek için veri ve algoritmaların kullanımına odaklanıp doğruluğunu kademeli olarak artıran bir yapay zeka (AI) ve bilgisayar bilimi dalıdır.

 ![download](https://user-images.githubusercontent.com/64674920/207737550-3a9bf263-3cde-49f1-9786-838f64c9a0b6.jpg)
 
 1) Denetimli Öğrenme 
  
Eğitim verilerinden, öngörülemeyen verileri tahmin etmenize yardımcı   olmak için öğrenen bir algoritmadır. Denetimli makine öğrenimi, istenen  sonuçları elde etmek için eğitim veri kümelerini kullanır.


![download](https://user-images.githubusercontent.com/64674920/207738218-7d51a651-ee1f-47b1-b7ca-789e993c64ba.png)

2)Denetimsiz Öğrenme 

Denetimsiz Öğrenme etiketsiz veriler arasındaki gizli kalmış  yapıyı/örüntüyü bulmaya çalışan bir makine öğrenmesi yöntemidir. Burada önemli olan elimizdeki verilerin etiketi hakkında bir bilgimizin olmadığı durumlarda denetimsiz öğrenme kullanılmaktadır.
Yani veri kümesi ile çıktıların olmadığı öğrenme metodudur. Veri kümesindeki verileri yorumlayarak ortak noktaları bulmak ve bunları kümeleştirme işlemi yapılarak anlamlı bir veri elde edebilmektir.

-Denetimsiz öğrenmede aslında her işi kendi kendine yapar.

Denetimli Ve Denetimsiz Öğrenme Arasındaki Farklılıklar 

![image](https://user-images.githubusercontent.com/64674920/207740057-8b178b8b-cdb0-4a22-a0bf-7328459fd29f.png)

2A)Kümeleme Algoritması

-Veri kümesindeki elemanların yakınlık, uzaklık ve benzerlik gibi ölçütlere göre analiz edilerek kendi arasında gruplandırmaya kümeleme denir.

-Temelde veriler kendi aralarındaki benzerlik ve farklılıklar analiz edilerek gruplandırılır.

-Kümeleme algoritmalarında kaç küme oluşması gerektiğine kullanıcı veya algoritma karar verir. Küme sayısı ile ayrıntı düzeyi belirlenir.

#Kümeleme Algoritması Kullanım Alanları

1-) Müşteri Segmentasyonu : Müşterilerin verileri ön tanımsız olarak makineye  verilir. Makine ortak özelliklere göre sınıflandırma yapar. Müşterilerin geçmiş verilerine bakılarak veya kendisine benzer kişilerin davranışlarına bakılarak ürün tavsiye edilir. Kişilere özel kampanyalar yapılır.

2-) Pazar Segmentasyonu :  Pazar araştırması kapsamında yaş grupları, kazanç dilimleri, kentsel, kırsal veya banliyö konumu gibi kategorileri belirlemek için kullanılabilir.  Pazarlamada, farklı müşteri gruplarının en alakalı mesajlarla hedeflenebilmesinde küme analizi kullanılır. Satın alma kalıplarına göre müşteri gruplarını karakterize edilir.

3-) Sağlıkta Kümeleme : Özellikle görüntü işlemede kümele çok kullanılır. Makine görüntüyü alıp analiz eder ve ardından kümele yapar.

2A.1)K-Means Kümeleme Algoritması

-K-Means kümeleme algoritması yinelemeli bir kümeleme algoritmasıdır. 

-"K" değeri kaç kümeye ayıracağımızı  belirleyen faktördür.  

-K değeri her yinelemede en yüksek değeri bulmaya yardım eder. 

-Başlangıçta K bizim tarafımızdan belirlenebilir. Sonrasında seçilen K değerine göre veriler K tane merkez noktada kümelenir.

-Kararlı hale gelinceye kadar merkez bulma döngüsü devam eder.

![image](https://user-images.githubusercontent.com/64674920/207835018-028f781e-2b14-4c93-9a08-9589b7552195.png)


K-Means Kümeleme Algoritması Kullanım Alanları: 

-Belge Sınıflandırılması : Belgeleri etiketlere, konulara ve belgenin içeriğine göre birden fazla kategoride kümeleyin. Bu standart sınıflandırma problemi K-Means ile çözülebilir.

-Suç Yerlerinin Belirlenmesi : Bir  şehirdeki belirli bölgelerde mevcut olan suçlarla ilgili veriler, suç kategorisi, suç alanı ve ikisi arasındaki ilişki, bir şehirdeki ya da bölgedeki suça eğilimli alanlara ilişkin kaliteli bilgiler verebilir.

-Görüntü Tanıma

-Oyuncu Analizi

-Çağrı  Kaydı Detay Analizi 

2A.2-) Hiyerarşik Kümeleme Algoritması Nedir?

Hiyerarşik kümeleme, birleştirici ve ayrıştırıcı hiyerarşik kümeleme yöntemleri olmak üzere iki türe sahiptir.  Birleştirici hiyerarşik kümelemede başlangıçta her bir değer bağımsız bir küme olarak değerlendirilir ve bu değerler çeşitli algoritmalarla birleştirilip her aşamada bir üst küme oluşturulur. Ayrıştırıcı kümelemede ise başlangıçta tüm değerler bir küme olarak değerlendirilip yine çeşitli ayrıştırma algoritmalarıyla alt kümeler elde edilir.  İşlem sonunda dendrogram denen tüm nesnelerin ilişkilerini gösteren bir ağaç yapısı oluşur.

Neden Hiyerarşik Kümeleme Algoritması?

K-means algoritmasının en kötü taraflarından biri küme sayısına karar vermenin zorluğudur. Küme sayısına ancak sistemi çok iyi bilen biri karar verebilir ki bu da probleme göre değişir. Örneğin bir ödev verdiniz ve hangi öğrencinin hangi öğrenciye yakın ödev yaptığını ve kaç küme oluştuğunu merak ettiğinizde küme sayısını önceden bilmenize olanak yoktur. Bir ödevde 3 küme çıkar, diğer ödevde 20 küme çıkabilir. İşte bu noktada x-means ve single pass gibi algoritmalar olsa da hiyerarşik kümeleme küme oluşturma için esnek bir yapı olması sebebiyle bir adım öne çıkar. 

-Bu yöntemde ise iki adet yaklaşım bulunmaktadır.

1-) Agglomerative 

Her bir veri öncelikle kendine ait bir küme oluşturur. Ardından birbirine en yakın olan iki küme birleşerek yeni bir küme oluşturur ve bu işlem tek bir büyük küme oluşuncaya dek devam eder.

2-)Divise



