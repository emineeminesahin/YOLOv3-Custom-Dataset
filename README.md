## Data
https://drive.google.com/file/d/1xdIivov7687aCJ_Hyf9QsJz2gcBnrt5r/view?usp=sharing

https://www.linkedin.com/posts/emine-sahin_deeplearning-yolo-darknet-activity-6993558796946059264-o9Ql?utm_source=share&utm_medium=member_desktop
 
 ### Veri Seti

Tüm veri setine oran ile %80 oranında eğitim verisi 11291 fotoğraftan, %20 oranında doğrulama veri seti 2823 fotoğraftan oluşmaktadır. Veri setinde 1280 x 720 ve 640 x 640 boyutlarında 14114 fotoğraf bulunmaktadır.  Eğitim veri setinde 11907 etiketleme, doğrulama veri setinde 2910 etiketleme işlemi yapılmıştır.
Veri seti yeterli olduğu için eğitim veri setinde veri seti arttırımı uygulanmamıştır. Aynı görüntü üzerinde karşılaştırma yapmak amacıyla doğrulama veri setinde +15, -15 derece döndürme; +50, -50 parlaklık arttırma ve azaltma; +35 bulanıklık ve görüntü kırpma işlemleri uygulanmıştır. Ayrıca doğrulama veri setine helikopter ve kuş görüntüleri de eklenerek FP değeri gerçekçi şekilde denenmiştir. 

![image](https://user-images.githubusercontent.com/114474881/223395646-7134a3e3-7aef-4af3-8f03-5cea576ff60b.png)

#### Şekil 1.1 Eğitim verisinde 11907 etiketlemenin boyutlarına göre dağılım grafiği

![image](https://user-images.githubusercontent.com/114474881/223395720-412940d3-a72d-4f6a-8cf4-bbf2f1643032.png)

#### Şekil 1.2 Doğrulama verisinde 2910 etiketlemenin boyutlarına göre dağılım grafiği

YOLOv3, YOLOv3-Tiny derin öğrenme modellerinde 20000 tur(epoch) sayısında eğitilmiştir.

Eğitim sırasında eğitimi yavaşlatmamak amacıyla doğrulama veri sayısı küçük kullanılmıştır. Eğitim sonucunda elde edilen ağırlık oluşturulan %20 oranlı doğrulama veri seti ile doğruluğu ölçülmüştür.
Elde edilen grafiklerde Google Colab’ da yaşanan GPU kullanım kısıtlamasından dolayı kesintiler oluşmuştur, bu durum ağırlık verisi için bir sorun olmayıp kalınan yerden devam edilmiştir.

![Ekran görüntüsü 2023-03-07 132917](https://user-images.githubusercontent.com/114474881/223396315-02882192-993b-45d6-bc07-a97d65adf3f3.jpg)

#### Şekil 2 YOLOv3(a), YOLOv3-Tiny(b) modellerinin iterasyona bağlı mAP ve average loss değerleri

![Ekran görüntüsü 2023-03-07 133308](https://user-images.githubusercontent.com/114474881/223397306-e08f6187-c102-4829-b009-ce99c136d315.jpg)

## Kullanılan Sistem: 
Casper S500
İşlemci:Intel(R) Core(TM) i5-10210U CPU @ 1.60GHz, 2112 Mhz, 4 Çekirdek, 8 Mantıksal İşlemci
Ekran Kartı: NVDIA GeForce MX230
RAM: 8 GB
