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

[Dizi örnekleri, ve çözümleri için tıklayınız.](https://github.com/nisaefendioglu/Java-Tutorial/tree/main/Hafta%204)

