### Diziler (Arrays) :
Bünyesinde aynı tip verileri barındıran yapılardır.​

Nesne gibi düşündükleri için referans tipleri olarak değer görürler. Referans tipleri 2 kısıma ayrılır. Referans ve İlkel veri tipleri. Referans, nesnelerin bellekteki yerlerini tutar. İlkel ver tipleriyse sadece 1 adet veriyi tutarlar.​
​
## Dizi Oluşturma ​
Java’da dizi tanımlaması aşağıdaki gibi yapılmaktadır;​

       int[] dizi; //dizi için yapılan referans tanımlaması​

Dizi tanımlaması yapılırken ilk olarak oluşturacağımız dizinin veri tipi belirtilir. ​

Dizinin türünü belirttikten sonra o tür dışındaki bir veriyi dizimiz içerisine ekleyemeyiz.​

Dizimiz için gerekli tür tanımlaması yaptıktan sonra köşeli parantezler konur. [] Köşeli parantezler bu verinin dizi olduğunu bizlere gösterir.​

## Dizi Tanımlama Şekilleri ​

       int dizi[];​

       String dizi[];​

       ​

       int [] dizi = {1,2,3,4,5};​

       ​

       String dizi[] = {"Mehmet" , "Nisa"}; ​

       ​

       int [] dizi = new int [5]; //dizi içerisi doldurulmadıysa eleman sayısı belirtilir.​

       ​

       Diziyi new ile oluşturmamız durumunda eleman sayısını girmek zorunludur.​

       ​

       int dizi[]; //referans oluşturuldu.​

       dizi = new int []{1,2,3,4}; // dizi içerisinin doldurulması sonucu dizi eleman sayısı belirtilmez.​

 ## Dizi Boyutunun Değiştirilmesi​
Dizi boyutu bir kez verildi mi, artık değiştirilemez,​

       int dizi[] = new int[5] ;​
       dizi = new int[15] ; ​

burada, yalnızca yeni bir dizi nesnesi daha oluşturulmaktır. liste dizi referansının daha evvelden bağlanmış olduğu dizi nesnesi (new int[5]), çöp toplama işlemi sırasında çöp toplayıcısı tarafından bellekten silinecektir.​
​

## Dizi Elemanlarına Erişim​
Java dilinde dizi kullanımı diğer dillere nazaran daha az risklidir; anlamı, eğer tanımladığımız dizinin sınırları aşılırsak, çalışma-anında (runtime) hata ile karşılaşacağımızdır. Örneğin 20 elemanlı bir double dizisi tanımlanmış olsun. Eğer bu dizinin 78. elemanına ulaşılmak istenirse (- ki böyle bir indisli eleman yok), çalışma-anında hata alınır; böylesi hatanın (ArrayIndexOutOfBounds Exception) çalışma-anında alınması güvenlik açısından güzel bir olaydır. Böylece dizi için ayrılmış bellek alanından dışarı çıkılıp başka verilere müdahale edilmesi engellenmiş olunur.​

### Int tipine değer atama​
       int[] dizi = new int[10];​

       dizi[0] = 1;​

### String tipine değer atama​
       String [] dizi = new String[5];​

       dizi[0] = new String(«java»);​

       dizi[1] = new String («merhaba»);​
       
## DİZİLERDE SIRALAMA İŞLEMLERİ​
Dizileri sıralamak için Arrays sınıfının sort() metodu kullanılır. ​

Bu sınıfı kullanmak için projemiz içerisinde java.util.Arrays paketini import etmemiz gerekmektedir.​

## Dizilerde Arama​
Java’da diziler içerisinde bir elemanı aratmak isteyebiliriz. Bunun için kullanacağımız yöntemin adı ise binarySearch yöntemidir.​

## BinarySearch Yöntemi ile Arama İşlemi ​
Bu metod ile aratılan elemanın dizideki indeksi bulunur. Eğer eleman dizide yok ise bu işlem bize negatif bir değer döndürür.​

Bu arama işleminde dizi içerisinde bir arama işlemi gerçekleştirmeden önce dizimizi sıralamamız gerekir. Sıralama işlemi gerçekleşmediği durumda arama işlemi de gerçekleşemez.​

İşlem sonucunda bulduğu elemanın indisi, sıralama yaptıktan sonraki indise aittir.​

## Dizileri Karşılaştırma İşlemleri​
Herhangi bir yerde iki diziyi birbiriyle karşılaştırmamız gerekebilir. Dizileri karşılaştırabilmek için karşılaştırma işlemi yapacağımız iki dizinin de aynı tipte olması gerekmektedir.​

Dizileri karşılaştırma işlemi için Arrays sınıfı içerisinde yer alan equals() metodu kullanılır.​

## Dizilerde Eşitlik Kontrolü​
Dizileri birbirleriyle karşılaştırarak eşitlik durumunda true, eşit olmama durumunda ise bizlere false sonucu döndürür.​

# Çok Boyutlu Diziler (Arrays)​
Java’da çok boyutlu array’ler, arraylerin array’i olarak tanımlanır. Başka bir deyişle, bileşenleri (öğeleri) array’lerden oluşan bir array’dir. Bir, iki, üç, dört, … boyutlu arr array’inin bildirimleri şöyle yapılır: ​

       int[] arr =[1,2,3,4}; ​

       int[][] arr = {}​

       int[][][] arr ; ​

       int[][][][] arr ;​

Boyut sayısı için bir kısıt yoktur. Tek boyutlu array bir boyutlu matris, iki boyutlu array iki boyutlu bir matris, üç boyutlu array üç boyutlu bir matris, … gibidir. Örneğin, iki boyutlu a[][] array’inde soldaki [] array bileşeni matrisin satırlarını, sağdaki [] bileşeni ise matrisin kolonlarını belirler. Üç boyutlu array’de en en sağdaki [] bileşeni, iki boyutlu düzlemsel matrisin üzerine çıkılan dikmeler gibidir. Boyut sayısı istenildiği kadar artırabilmesine karşın, uygulamada çoğunlukla iki boyutlu array’ler ile karşılaşılır. ​

Bir boyutlu array’ler için yaptığımız gibi, çok boyutlu array’lerin bileşenlerine de bildirim anında değer atayabiliriz. Aşağıdaki array, bileşenleri int tipi olan 2-boyutlu bir arraydir. ​

       int[][] ikilSayı = { {1, 2}, {3, 4}, {5, 6} }; ​

## Çok Boyutlu Dizi Tanımlamaları​
       int [][] ikiliSayi = {{1,2}, {3, 4}, {5, 6}};​

       int [][] dizi = new int [2][2];​

       dizi[0][0] = 1;​

       dizi[0][1] = 1;​

       dizi[1][0] = 1;​

       dizi[1][1] = 1;​

       int [][] ikiliSayi = {{1,2}, {3, 4}, {5, 6}};​

       int [][] dizi = new int [2][2];​

       dizi[0][0] = 1;​

       dizi[0][1] = 1;​
  
       dizi[1][0] = 1;​

       dizi[1][1] = 1;​

## Çok Boyutlu Dizi Elemanlarına Erişim​
Çok boyutlu dizilere erişim, tek boyutlu dizilere erişime benzer yapıda bulunmaktadır. Köşeli parantezler içerisine indeksler yazılarak erişim sağlanır.​

       int dizi[][] = {{1,33}, {5,88}};​

       System.out.println(dizi[1][1]);​

## toString() metodu​
Dizileri string ifadeye çevirerek tüm diziyi köşeli parantezler arasında ekrana yazdırmamızı sağlayan metoddur. Tek boyutlu dizilerde kullanılır.​

## Çok Boyutlu Dizileri Listeleme​
Çok boyutlu dizileri listeleme, tıpkı tek boyutlu dizilerde olduğu gibi yapılmaktadır.​

[Dizi örnekleri, ve çözümleri için tıklayınız.](https://github.com/nisaefendioglu/Java-Tutorial/tree/main/Hafta%204)

