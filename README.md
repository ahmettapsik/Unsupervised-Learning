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

Bu yaklaşımda ise tüm veriler öncelikle tek bir küme içerisinde ele alındıktan sonra her bir veri noktası birer küme oluncaya dek bölünme işlemi gerçekleşiyor.
     
 
 ![Img_43](https://user-images.githubusercontent.com/64674920/207929363-1e38afc6-5966-49e0-b806-88d5e7788d42.jpg)

2B-) Boyut Küçültme Algoritması

Gerçek hayattaki veriler çok fazla boyuta (özniteliğe) sahip oluyor ve boyut büyüdükçe veri temizlemeden model kurmaya bütün süreçlerde harcamamız gereken zaman ve kaynaklar artıyor. Boyut azatma bu sorunun önüne geçmek için kullanılan yöntemlerden biridir. Hemen her veri setinde bazı öznitelikler arasında yüksek korelasyon oluyor ve bu bizim gereksiz bilgiye sahip olmamıza ve modelimizde overfitting problemine sebep olabiliyor.

Boyut Küçültme Nasıl Uygulanır

Boyut küçültmenin en kolay yolu verimizi en iyi tanımlayan öznitelikleri bulup diğerlerini atmaktır (öznitelik seçimi — feature selection). Dikkat edilmesi gereken nokta en az bilgi kaybıyla bu işi yapmaktır ve aslında önemli olan öznitelikleri silmemektir. Bunu yapmak için verideki dağılımın maksimum varyansını-bilgisini tutan minimum sayıda değişken oluşturuyoruz. Eğer bir değişken her örnek için aynı değere sahip ise gereksiz bir değişkendir. Biz en yüksek varyansa sahip olan değişkenleri bulmalıyız.

 2C-) Pazar Sepeti Analizi 
 
- Pazar sepeti analizi, tüketicilerin satın alma davranışlarının analiz ederek ürünler arasındaki ilişkileri ortaya çıkaran ve şirketlerin büyük ölçekte satış yapmasını amaçlayan bir yöntemdir.
- Örneğin bir marketten müşterilerin süt ve peynir satın alımlarının %70'inde  bu ürünler ile birlikte yoğurtta satın alınmıştır. Pazar sepeti analizi bu ilişkiyi ortaya çıkarır ve satıcılar buna göre bir satış politikası izlerler.
- Tüketicilerin satın alma davranışları, alışveriş alışkanlıklarının ve birlikte aldıkları ürünlerin incelenmesiyle elde edilir.

Pazar Sepeti Uygulamaları

2C.1-) Çapraz Satış Yapılması(Cross-Sell):

Bir ürünü satarken, bu ürünü tamamlayacak bir yan ürünü, ürünle beraber tüketiciye sunarak, tüketicinin birden fazla ürünü satın almaya yönlendirecek satış yöntemidir. Tüketicinin, “Sepet” sayfası üzerinde de kullanıcının sepete eklediği ürünle ilgili olabilecek alternatif ürünleri listelenmesi bir çapraz satış örneğidir.

2C.2-) Mağaza Düzeni(Store Layout): 
Satışları ve geliri artırmak için mağazadaki ürünler pazar sepeti analizine göre düzenlenebilir. 
 
-Pazar sepeti analizine göre ürünler müşterinin dikkatini çekecek ve diğer ürünü satın alma kararına yardımcı olacak şekilde sıralanabilir veya yerleştirilebilir.

-Pazar sepeti analizi, satışların artmasıyla sonuçlanan ürünleri ve kombinasyonları düzenlemek için bir rehber görevi görür.

 ![IC-Store-Layout-Loop](https://user-images.githubusercontent.com/64674920/207938343-eaa84efb-3094-44c6-b366-2237fe7c3851.jpg)

2C.3-) Tavsiye Motorları(Recommendation Engines)
- Pazar sepeti analizi, tavsiye motorlarını güçlendiren temel ilkedir.
- Tavsiye sistemleri, kullanıcıların deneyimlerini, davranışlarını, tercihlerini ve ilgi alanlarını kullanarak tüm dijital dünyayı keşfetmelerinin birincil yolu haline geliyor. Bilgi yoğunluğunun ve aşırı ürün alışverişinin olduğu bir dünyada, bir tavsiye motoru, şirketlere tüketicilere kişiselleştirilmiş bilgi ve çözümler sunmanın verimli bir yolunu sunar. 

  ![download](https://user-images.githubusercontent.com/64674920/207940292-d8f9be14-9f1b-4827-9db8-bef7ceb056a6.png)
  
  
  
  
  
  
  
  
  
  ###############################################################
  
  
  
  
  KAYNAKÇA
 - https://samed-harman.medium.com/makine-%C3%B6%C4%9Frenmesi-clustering-k%C3%BCmeleme-teknikleri-bd1b59a0a177 ​

https://medium.com/@gulcanogundur/pca-principal-component-analysis-temel-bile%C5%9Fenler-analizi-bf9098751c62​

https://medium.com/data-science-tr/makine-%C3%B6%C4%9Frenmesi-dersleri-boyut-azaltma-pca-5ae9e902ef92​

https://samed-harman.medium.com/makine-%C3%B6%C4%9Frenmesi-clustering-k%C3%BCmeleme-teknikleri-bd1b59a0a177​

https://erdincuzun.com/makine_ogrenmesi/hiyerarsik-kumeleme-hierarchical-clustering-odev-benzerlikleri-uzerinden-kopya-gruplarini-bulma/​

https://www.btkakademi.gov.tr/portal/course/player/deliver/python-ile-makine-oegrenmesi-11800​


https://medium.com/machine-learning-türkiye/adım-adım-makine-öğrenmesi-bölüm-3-denetimsiz-öğrenme-nedir-f890ada49a40​

https://www.ibm.com/cloud/learn/unsupervised-learning#:~:text=Unsupervised%20learning%2C%20also%20known%20as,the%20need%20for%20human%20intervention.​

https://www.expert.ai/blog/machine-learning-definition/​

https://www.neenopal.com/MarketBasketAnalysis.html​

https://www.slideshare.net/uslumetin/birliktelik-kurallar-kullanlarak-pazar-sepeti-analizi-market-basket-analysis-using-association-rules​

https://djinit-ai.github.io/2020/09/22/apriori-algorithm.html​

https://medium.com/@eminenurnacar/veri-madencili%C4%9Finde-pazar-sepeti-analizi-de44962f2086​

https://www.veribilimiokulu.com/associationrulesanalysis/​

https://yavuz.github.io/denetimsiz-ogrenme/ ​

https://www.youtube.com/watch?v=CMbLMiJAx_g ​

https://samed-harman.medium.com/makine-%C3%B6%C4%9Frenmesi-clustering-k%C3%BCmeleme-teknikleri-bd1b59a0a177 ​

https://www.btkakademi.gov.tr/portal/course/player/deliver/python-ile-makine-oegrenmesi-11800​
  
 

 
 
 
 
 
 
 
 
 
 


