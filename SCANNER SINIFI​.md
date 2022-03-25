### SCANNER SINIFI​
Bir programlama dilinde, kullanıcıdan veri girişi yapmasını isteyebiliriz. ​

Kullanıcının girdiği bu verilere göre işlem yapabilir, bunları ekrana yazdırabilir veya herhangi bir yere parametre olarak verebiliriz. Bu tür işlemleri yapabilmek için Java’da Scanner sınıfı kullanılır.​

Scanner sınıfını projemizde kullanabilmek için java.util.Scanner sınıfını projemize import etmemiz yeterlidir.​
Scanner sınıfı ile klavyeden veri okumak için öncelikle bu sınıftan bir nesne oluşturmamız gerekir. 

Örneğin;​

       Scanner kullaniciGirdisi = new Scanner(System.in); ​

Burada kullaniciGirdisi ismini verdiğimiz nesneyi oluşturduk.​

Buradaki System.in input anlamına gelir ve dışarıdan bir veri alındığını belirtir. ​
Eğer kullanıcıdan alacağımız nesnenin veri tipi integer türünde ise bunun için;​

       int sayi=kullaniciGirdisi.nextInt(); //int türündeki değeri almak için​

       byte türü → nextByte();​

       Double türü → nextDouble();​

       Float türü → nextFloat();​

       Boolean türü → nextBoolean();​

       String türü → nextLine();​

       String türü → next(); //kullanıcıdan alınan girdide boşluğa kadar olan kısmı alır.​

[Scanner sınıfı ile ilgili örnekler, ve çözümleri için tıklayınız.](https://github.com/nisaefendioglu/Java-Tutorial/tree/main/Hafta%205)
