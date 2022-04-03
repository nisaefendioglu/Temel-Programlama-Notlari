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

### Nesne​
Java Nesne ve Sınıf Yapısında nesnelerin sınıflardan oluşur. En basit ve genel yöntemle;​

SinifAdi sinifAdi = new SinifAdi();​

şeklinde bir tanımlama ile sinifAdi nesnesi oluşturulabilir.​


