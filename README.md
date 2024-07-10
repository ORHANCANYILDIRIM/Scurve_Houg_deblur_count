 
 
 
 




 
S-CURVE METODU
 
"S-curve" metodu, bir görüntüdeki kontrastı artırmak için kullanılan bir tekniktir. Görüntüdeki piksel değerlerini değiştirerek kontrastı artırır. Tipik olarak, karanlık tonlarda daha fazla detay ve aydınlık tonlarda daha fazla ayrıntı sağlamak için kullanılır. Histogram analizi ile eğri oluşturulur ve piksel değerleri bu eğriye göre dönüştürülür. Sonuç olarak, daha canlı ve etkileyici bir görüntü elde edilir.
Avantajlar:
	Kontrastın Artırılması: S-curve yöntemi, görüntüdeki kontrastı artırmanın etkili bir yoludur. Bu, görüntünün daha canlı ve etkileyici görünmesini sağlar.
	Basit Uygulanabilirlik: S-curve, uygulanması oldukça basit olan bir yöntemdir. Piksel değerlerinin dönüşümü için tek bir eğri kullanılarak kolayca gerçekleştirilebilir.
	Kontrol Edilebilirlik: S-curve yöntemi, kontrast artırma işlemi için kullanılan eğriyi oluşturmak için kullanıcıya kontrol sağlar. Bu sayede, kullanıcı isteğine göre kontrastın derecesini ayarlayabilir.
Dezavantajlar:
	Veri Kaybı Riski: S-curve yöntemi, bazen görüntüdeki detayları kaybetme riski taşır. Özellikle aşırı kontrast artışı durumunda, bazı bölgelerde detay kaybı yaşanabilir.
	Renk Bozulması: Renkli görüntülerde S-curve uygularken, renklerde bozulma riski vardır. Bu nedenle, renkli görüntülerde uygulamadan önce dikkatli olunmalıdır.
Nerede ve Nasıl Kullanılır:
	Fotoğraf Düzenleme: S-curve, fotoğraf düzenleme yazılımlarında sıkça kullanılan bir tekniktir. Özellikle dijital fotoğrafçılıkta, görüntülerin daha etkileyici hale getirilmesi için tercih edilir.
	Tıbbi Görüntüleme: Tıbbi görüntüleme alanında, S-curve yöntemi, radyolojik görüntülerin daha iyi analiz edilmesi için kullanılabilir. Bu, doktorların teşhis koymasını ve tedavi planlarını oluşturmasını kolaylaştırabilir.
	Görüntü İşleme Uygulamaları: Görüntü işleme yazılımlarında geniş bir kullanım alanına sahiptir. Özellikle, video düzenleme, animasyon ve grafik tasarım gibi alanlarda sıkça kullanılır.
Kontrast güçlendirme metodları, uygun şekilde uygulandığında görüntülerin görsel çekiciliğini artırabilir ve belirli durumlarda oldukça faydalı olabilir. Ancak, aşırıya kaçılması veya hatalı bir şekilde uygulanması durumunda istenmeyen sonuçlar doğurabilir. Bu yüzden, dengeli bir şekilde kullanmak her zaman önemlidir. 


Standart Sigmoid Fonksiyonu: 
Standart sigmoid fonksiyonu;
f(x)=1/(1+e^(-x) )


 genellikle aktivasyon fonksiyonu olarak kullanılır ve giriş değerlerini belirli bir aralıktan (genellikle -sonsuz, +sonsuz) 0 ile 1 arasında bir çıkış aralığına dönüştürür.  
Sigmoid fonksiyonunun grafiği S şeklinde olup, belirli bir eğri boyunca sürekli ve monoton artan veya azalan bir eğri oluşturur. Bu fonksiyon, giriş değerlerini sıkıştırarak veya genişleterek, görüntüdeki kontrastı ayarlamak için kullanılabilir. Özellikle, düşük kontrastlı pikselleri koyulaştırarak ve yüksek kontrastlı pikselleri daha da aydınlatarak, görüntüdeki tonları daha dengeli bir şekilde dağıtmaya yardımcı olabilir. 
 
 
 
Uygulamalı Gösterim: 
 
 ![image](https://github.com/ORHANCANYILDIRIM/Scurve_Houg_deblur_count/assets/99863519/034b5f48-890c-45ef-8333-0f3609e25587)

 




Yatay Kaydırılmış Sigmoid Fonksiyonu:  
Yatay kaydırılmış sigmoid fonksiyonu;
𝑓(𝑥) =   

 Standart sigmoid fonksiyonunun bir türevidir ve genellikle aktivasyon fonksiyonu olarak kullanılır. 
Burada, c  parametresi, fonksiyonun yatay olarak kaydırılmasını kontrol eder. Bu fonksiyon, giriş değerlerini belirli bir aralıktan (genellikle -sonsuz, +sonsuz) 0 ile 1 arasında bir çıkış aralığına dönüştürür.
Yatay kaydırılmış sigmoid fonksiyonunun grafiği, standart sigmoid fonksiyonununki gibi S şeklinde olup, belirli bir eğri boyunca sürekli ve monoton artan veya azalan bir eğri oluşturur. Bu fonksiyon da, giriş değerlerini sıkıştırarak veya genişleterek, görüntüdeki kontrastı ayarlamak için kullanılabilir. Özellikle, düşük kontrastlı pikselleri koyulaştırarak ve yüksek kontrastlı pikselleri daha da aydınlatarak, görüntüdeki tonları daha dengeli bir şekilde dağıtmaya yardımcı olabilir.

Uygulamalı Gösterim: 
 
![image](https://github.com/ORHANCANYILDIRIM/Scurve_Houg_deblur_count/assets/99863519/e98f1be7-2bba-4682-a09e-bb0381a9c28a)

 
 
 

Eğimli sigmoid fonksiyonu: 
Eğimli Sigmoid Fonksiyonu;
𝑓(𝑥) =   

 Eğimli sigmoid fonksiyonu, standart sigmoid fonksiyonunun bir türevidir ve genellikle aktivasyon fonksiyonu olarak kullanılır. 
 Burada, 𝑎 parametresi, fonksiyonun eğimini kontrol eder. Bu fonksiyon, giriş değerlerini belirli bir aralıktan (genellikle -sonsuz, +sonsuz) 0 ile 1 arasında bir çıkış aralığına dönüştürür.
Eğimli sigmoid fonksiyonunun grafiği, standart sigmoid fonksiyonununki gibi S şeklinde olup, belirli bir eğri boyunca sürekli ve monoton artan veya azalan bir eğri oluşturur. Bu fonksiyon da, giriş değerlerini sıkıştırarak veya genişleterek, görüntüdeki kontrastı ayarlamak için kullanılabilir. Özellikle, düşük kontrastlı pikselleri koyulaştırarak ve yüksek kontrastlı pikselleri daha da aydınlatarak, görüntüdeki tonları daha dengeli bir şekilde dağıtmaya yardımcı olabilir.



Uygulamalı Gösterim: 
 
 ![image](https://github.com/ORHANCANYILDIRIM/Scurve_Houg_deblur_count/assets/99863519/6ae09861-1267-421e-b6c5-be3c53cb8a84)



Kendi Fonksiyonum:

Fonksiyon;
f(x)=1/(1+e^(-α(x-β)λ) )+x^2

	
giriş değerlerini S-Curve eğrisine dönüştürmek için sigmoid fonksiyonu (1 / (1 + e^(-x))) kullanır. Bu sigmoid fonksiyonunun çıkışı, gama parametresiyle üslenir ve bir kare terimiyle toplanır. Bu, eğrinin daha karmaşık bir şekle dönüşmesini sağlar.
Özellikle, x değerlerinin karesi üzerinden bir dönüşüm kullanarak, S-Curve eğrisi, giriş değerlerini dönüştürerek kontrastı ayarlamak için kullanılabilir. Örneğin, düşük kontrastlı pikselleri koyulaştırabilir ve yüksek kontrastlı pikselleri daha da aydınlatabilir.
Bu fonksiyon, görüntü işleme uygulamalarında, özellikle kontrast ayarlama işlemlerinde, etkili bir araç olarak kullanılabilir.

 
 
Uygulamalı Gösterim : 
 
![image](https://github.com/ORHANCANYILDIRIM/Scurve_Houg_deblur_count/assets/99863519/18609242-cd7b-4a06-8190-f6190b1f57ca)


 
HOUGH TRANSFORM METODU
 
Hough Transform, verilen bir görüntüdeki belirli parametrelere sahip (örneğin, çizgi) noktalarının hangi geometrik şekillerle (örneğin, doğrular) eşleştiğini bulmak için kullanılır. Temel olarak, bir noktanın bir geometrik şekle karşılık gelip gelmediğini belirlemek için kullanılan bir dönüşüm tekniğidir.
Hough Transform, aday çizgilerin (veya diğer şekillerin) olası parametrelerini (örneğin, doğrunun eğimi ve y-kesme noktası) içeren bir uzayda oy toplar. Bu, bir çizgiye karşılık gelen herhangi bir noktanın, parametre uzayında bir eğri oluşturması anlamına gelir. Daha sonra, bu oy uzayındaki piksellerin bir kısmı belirlenmiş bir eşik değerinin üzerinde birikir ve bu birikimler olası çizgi (veya diğer şekiller) parametrelerini belirler.
 
Yoldaki çizgileri tespit etmek için Hough Transform kullanımı: 
	Görüntüyü Yükleme: Kod, verilen bir görüntü dosyasını yükler. Bu, bilgisayar belleğine bir görüntü dizisi olarak yüklenir, her bir elemanı bir pikseli temsil eder.
	Görüntünün Boyutlarını Alma: Görüntü, yüklenmeden önce, yükseklik ve genişlik gibi temel özelliklerine sahiptir. Bu adımda, yüklenen görüntünün boyutları alınır. Bu, daha sonra ROI belirleme ve diğer işlemler için kullanılır.
	İlgilenilen Bölgeyi Belirleme (ROI): ROI (Region of Interest), yani ilgilendiğiniz bölge, genellikle bir maske yardımıyla belirlenir. Bu, tespit edilmek istenen nesnelerin bölgesini sınırlar ve diğer gereksiz kısımları filtreler.
	Renk Uzayı Dönüşümü (BGR'den HSV'ye): Görüntünün renk uzayını değiştirmek, genellikle işlemi basitleştirir veya belirli özellikleri daha iyi ortaya çıkarır. Bu kodda, BGR (Blue, Green, Red) renk uzayından HSV (Hue, Saturation, Value) renk uzayına dönüşüm yapılır.
	Kenar Tespiti: Kenar tespiti, genellikle nesnelerin sınırlarını belirlemek için kullanılır. Canny Edge Detection gibi algoritmalar kullanılarak, görüntüdeki keskin değişiklikler belirlenir ve kenarlar çıkarılır.
	Hough Dönüşümü Uygulama: Hough Transform, kenarları geometrik şekillere dönüştürmek için kullanılır. Bu kodda, Hough Transform'u uygulayarak, kenarlar (veya kenar pikselleri) çizgiler olarak algılanmaya çalışılır. Bu adım, belirli bir doğrultuda uzun ve düz çizgileri tanımlamak için önemlidir.
	Tespit Edilen Çizgileri Görüntüye Çizme: Hough Transform sonucunda tespit edilen çizgiler, orijinal görüntü üzerine çizilir. Bu adım, tespit edilen çizgilerin görsel olarak gösterilmesini sağlar ve sonuçları kullanıcıya sunar.
 

Uygulamalı Gösterim: 

 
![image](https://github.com/ORHANCANYILDIRIM/Scurve_Houg_deblur_count/assets/99863519/acd66c90-dc5c-442d-8d8f-61c223993f20)

 
 
 
 
 
 
 
Yüz resminde gözleri tespit etmek için Hough Transform kullanımı:  
	Resmi Yükleme: İlk adımda, verilen bir görüntü dosyasını yüklersiniz. Ardından, bu görüntüyü gri tonlamalı bir formata dönüştürürsünüz. Gri tonlamalı görüntüler, yüz ve göz tespiti gibi işlemlerde yaygın olarak kullanılır çünkü renk bilgisi olmadan daha kolay işlenebilirler.
	Yüz Tespiti: Yüz tespiti için OpenCV kütüphanesinin Haar Cascade sınıflandırıcısı kullanılır. Bu sınıflandırıcı, yüzlerin belirli özelliklerini (gözler, burun, vb.) tanımlayan eğitilmiş bir modeldir. Görüntüdeki yüzleri tespit etmek için bu sınıflandırıcı kullanılır. Yüzler, detectMultiScale fonksiyonuyla belirlenir ve koordinatları (x, y, genişlik, yükseklik) şeklinde döner.
	Göz Tespiti için Göz Tespit Sınıflandırıcısı: Göz tespiti için ayrı bir Haar Cascade sınıflandırıcısı kullanılır. Bu sınıflandırıcı, gözlerin belirli özelliklerini tanımlayan bir modeldir. Bu modeli kullanarak, her bir yüz bölgesindeki gözleri tespit etmeye çalışacaksınız.
	Her Bir Yüz Bölgesi için Gözleri Tespit Etme: Yüzler tespit edildikten sonra, her bir yüz bölgesindeki gözleri tespit etmek için bir döngü oluşturulur. Her bir yüz bölgesi (x, y, genişlik, yükseklik) koordinatlarıyla tanımlanır. Daha sonra, bu bölgenin gri tonlamalı versiyonu alınır (roi_gray). Ayrıca, orijinal renkli görüntüdeki yüz bölgesi de alınır (roi_color). Gözleri tespit etmek için, göz sınıflandırıcısı (eye_cascade) bu bölge üzerinde çalıştırılır ve gözlerin koordinatları (x, y, genişlik, yükseklik) şeklinde döner. Dönen koordinatlar, orijinal renkli görüntü üzerine yeşil dikdörtgenler çizmek için kullanılır.
	Sonuçları Döndürme: Son olarak, tespit edilen yüzler ve gözlerle işlenmiş olan orijinal renkli görüntü döndürülür. Bu, görsel sonucu kullanıcıya sunmak için kullanılır.
 
Uygulama: 
 

 
 ![image](https://github.com/ORHANCANYILDIRIM/Scurve_Houg_deblur_count/assets/99863519/e71e3bde-5f72-42fb-a599-db84a2e5b746)

 
 
 
 
 
 
 
DEBLURRING 
 
Deblurring işlemi, bir görüntünün bulanık veya keskin olmayan bölümlerini iyileştirmeyi amaçlar. Bu işlem, fotoğraf düzenleme, tıbbi görüntüleme, video analizi ve birçok diğer alan için önemlidir.  
 
	Görüntüyü Yükleme:
	Koddaki kullanımı: image = cv2.imread(image_path)
	Açıklama: Fonksiyon, belirtilen görüntü dosyasını yükler.
	Bulanıklık Modelini Belirleme (Kernel):
	Koddaki kullanımı: kernel = np.ones((3, 3), np.float32) / 9
	Açıklama: Bir bulanıklık modeli belirlenir. Bu genellikle bir düşük geçişli filtre şeklinde olur. Bu kodda, 3x3 boyutunda bir çizgi gibi bir filtre oluşturulur.
	Bulanıklık Modelini Görüntüye Uygulama:
	Koddaki kullanımı: deblurred_image = cv2.filter2D(image, -1, kernel)
	Açıklama: Belirlenen bulanıklık modeli, cv2.filter2D fonksiyonu kullanılarak görüntü üzerine uygulanır. Bu adım, görüntüdeki bulanıklığı azaltmayı amaçlar.
	Görüntüyü İyileştirme (Keskinleştirme):
	Koddaki kullanımı: enhanced_image = cv2.detailEnhance(deblurred_image, sigma_s=25, sigma_r=0.75)
	Açıklama: Bulanıklık azaltma işleminden sonra, görüntüyü daha keskin hale getirmek için bir iyileştirme adımı uygulanır. Bu adımda, cv2.detailEnhance fonksiyonu kullanılarak görüntü iyileştirilir.
	İyileştirilmiş Görüntüyü Döndürme:
	Koddaki kullanımı: return enhanced_image
	Açıklama: Son olarak, işlenmiş ve iyileştirilmiş görüntü döndürülür. Bu, fonksiyonun çıkışını oluşturur ve kullanıcının işlenmiş görüntüyü kullanabilmesini sağlar.
 




Uygulama: 
 
 ![image](https://github.com/ORHANCANYILDIRIM/Scurve_Houg_deblur_count/assets/99863519/85dbccec-0b30-46d1-b744-af3338ed0f66)

 
 
 
 
RESİMDEKİ NESNELERİ SAYMA VE ÖZELLİK ÇIKARMA 
 
İşlem adımları şunlardır:  • Görüntüyü bir NumPy dizisine dönüştürme. 
	Görüntüyü gri tonlamalı hale getirme ve gürültüyü azaltmak için Gauss filtresi uygulama.  
	Belirli bir renk aralığında maske oluşturma. 
	Maskeleme işlemiyle konturları bulma. 
	Her kontur için bazı özelliklerin hesaplanması (alan, merkez, sınırlayıcı dikdörtgen, çapraz, enerji, entropi, ortalama, medyan).  
	Bu özelliklerin bir veri çerçevesine kaydedilmesi. 
	Veri çerçevesinin bir Excel dosyasına kaydedilmesi.  
Bu işlem, görüntü işleme ve veri analizi alanlarında sıkça kullanılan tekniklerin birleşimidir. Bu kod, koyu yeşil alanlarla ilgili belirli özellikleri hesaplamak için oldukça kapsamlı bir yaklaşım sunar. 

Uygulama Adımları:
Adım1:  
![image](https://github.com/ORHANCANYILDIRIM/Scurve_Houg_deblur_count/assets/99863519/e5d7fba6-1603-457b-b93c-1ae540f144f9)

Adım2:
 ![image](https://github.com/ORHANCANYILDIRIM/Scurve_Houg_deblur_count/assets/99863519/4967ab9f-1c2d-4b19-a2b9-eed394cbd077)

Adım3:
 ![image](https://github.com/ORHANCANYILDIRIM/Scurve_Houg_deblur_count/assets/99863519/776ceffc-0714-4f4a-8840-eec2f3d2eef2)


		Excel Tablosu: 
 ![image](https://github.com/ORHANCANYILDIRIM/Scurve_Houg_deblur_count/assets/99863519/8e17c930-bb5e-44ab-90ea-b73a825eacad)




											Orhancan Yıldırım
       
                                                                                                                            
