## Java Nesne Yönelimli Programlama​

### Nesne ve Sınıf Yapısı​
Java Nesne ve Sınıf yapısı kullanılarak Nesneye dayalı programlama yapılmaktadır. Aslında nesneler sınıflardan oluşmaktadır. Java’da bir sınıfı class anahtar kelimesini kullanarak tanımlayabiliriz.​

Sınıf;  Nesnelerin özelliklerini ve işlevlerini tanımlayan bir şablondur.​

Nesne; Çevremizde gördüğümüz özellikleri ve işlevleri olan her şeyi nesne olarak tanımlayabiliriz. Bu canlı veya cansız bir varlık olabilir. Örn: Telefon, bilgisayar, araba, hayvan vs. Nesnelerin özellikleri önceki derslerimizde gördüğümüz Java Veri Tipleri ile belirtilebileceği gibi yine bizim tarafımızdan oluşturulan sınıflar aracalığı ile de belirtilebilir. Nesnelerin işlevleri ise yine daha önceden gördüğümüz Metot Yapısı ile belirtilerek nesnelerin birbirleri arasındaki iletişimi sağlanır.​

Sınıf​

Java Nesne ve Sınıf Yapısı’nda “Nesneler sınıflardan oluşur” demiştik, o halde öncelikle sınıf yapısı nasıl oluşur ona bakalım;​

    public class SinifAdi {​

    public degiskenTuru degiskenTuru;​

    //constructor​

    SinifAdi() {​

    }​

    //constructor​

    SinifAdi(degiskenTuru yeniDegiskenTuru) {​

        degiskenTuru = yeniDegiskenTuru;​

    }​

    //metot​

    void metotAdi() {​

    } ​
    
### Constructor (Yapıcı Metot)​
Burada daha önce görmediğimiz constructor yapısı bulunmaktadır. Aslında Java’da bir sınıf oluşturduğumuzda constructor yani yapıcı metotlar büyük önem taşımaktadır. Biz kod yazarken herhangi bir constructor metot tanımlamasak bile Java bizim için bir tane constructor metot oluşturmaktadır. Constructor metotlar bir sınıftan bir nesne oluşturulduğunda ilk çalışan metotlardır. Bu metotlar aracılığı ile sınıflara ilk çalıştıklarında vermek istediğimiz değerleri verebilir, varsayılan değerlere farklı değerler atayabilir veya bir metot çalıştırabiliriz.​
Oluşturduğumuz sınıfın yapısını daha net görebilmek adına görsel olarak bir tanımlama yapabiliriz Bir sınıfı görsel olarak anlatmanın yöntemi Unified Modeling Language yani UML kullanarak UML class diagram oluşturmakla mümkündür. Burada sınıfın adı, içindeki veri tipi alanları, constructor ve metotları görüntülenebilir. ​

[Constructor örnekleri, ve çözümleri için tıklayınız.](https://github.com/nisaefendioglu/Java-Tutorial/blob/main/Hafta%206/Constructor.java)


### Nesne​
Java Nesne ve Sınıf Yapısında nesnelerin sınıflardan oluşur. En basit ve genel yöntemle;​

SinifAdi sinifAdi = new SinifAdi();​

şeklinde bir tanımlama ile sinifAdi nesnesi oluşturulabilir.​

## OOP : Nesneye dayalı programlama tekniğidir. Her şey nesnelerden ibaret.

Temelinde OOP yatan 2  tür programlama vardır;

1- Class temeline dayalı —> C#

2- Prototip temeline dayalı —> JavaScript

### Abstraction - Soyutlama:

Abstract ifadesiyle tanımlanır.

Nesne oluşturulamaz.

Extends edilir.

Ortak özellikleri olan nesneleri tek bir çatı altında toplamak için kullanılır.

ÖRNEK:

```
public abstract class Ogrenci_Sinifi {

    private String ad;
    private String soyad;
    private int numara;

    public abstract String getAd();

    public abstract String getSoyad();

    public int getNumara() {
        return this.numara;
    }

    public class Ogrenci extends Ogrenci_Sinifi {

        public String getAd() {
            return "Burak";
        }

        public String getSoyad() {
            return "Kutbay";
        }

        public int getNumara() {
            System.out.println(super.getNumara());
            return super.getNumara();
        }
    }
}
```

### Encapsülation - Kapsülleme :

Sınıf içerisinde tanımlanan değişkenleri korumak ya da saklamak için kullanılan yapıdır.

Tanımlanan değişkenin direkt olarak değiştirilmemesi, metotlarla bizim izin verdiğimiz şekliyle değiştirilmesi. get-set. 

Örneğin; Klavyede tuşlarımız var ve biz bunlara bize sunulduğu kadarına erişebiliyoruz yani arka taraftaki işlemlerine erişim sağlayamıyorum. A harfine basınca Z harfi basması gibi yetkilere erişemiyoruz. Bize public olarak sunulan kısma erişim sağlayabiliyoruz.

Inheritence - Kalıtım :

Bir yerde tanımlamış olduğumuz herhangi bir nesneyi tekrar başka bir kod bloğunda kullanmak istediğimizde kullanılan yapıdır. Kod tekrarını önler. Babadan oğula, bir sınıftan alt sınıf üretmek. Anne-babadan çocuğuna geçen özellikleri örnek olarak verebiliriz.

### Polymorphism - Çok Biçimlilik :

Bir nesnenin birden fazla forma sahip olmasıdır. Yani oluşturulan nesne kendisi gibi değil de başka bir nesne gibi davranabilir. Kod içerisinde bir nesnenin davranışının override edilmesi. Aynı işlem farklı davranış.

Örnek: Yazılım dillerini ele alırsak kodun ilk başta bir derlenmesi gerekmektedir fakat bu derleme işlemi java içerisinde ayrı c++ içerisinde farklı olması.

Tüm taşıma araçları için sürmek eylemi kullanılmasına rağmen bir otomobil kullanımı ile bisiklet kullanımı arasında farklar olması.

Her öğrencinin okuduğu okuldan mezun olma koşuluna sahip olması fakat bir üniversite mezuniyeti için gereken koşullar ile bir lise mezuniyeti arasında farklılık olması.

### Class Ve Object(Nesne) İlişkisi:

Class, oluşturulan type’ın tanımıdır. Uygulama içerisinden dışarya açacağımız ya da uygulama içinde kullanacağımız data formatı için tanımdır. Object(Nesne) ise ilgili class’ın instance’ıdır. Yani Firma adında bir Class’ımız olsun firma türünden oluşan X Firması da Instance olmaktadır.

[Faydalı Link](https://feyyazacet.medium.com/object-oriented-programming-oop-a90c040e21b8)


