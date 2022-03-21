### Döngüler

Programlamada en çok kullanılan özelliklerden biri de döngülerdir. Döngüler aracılığı ile belli şartlar gerçekleşinceye kadar veya gerçekleştikçe bir komut parçasını çalıştırmak mümkündür. Bir programda bir komut parçasının belli koşullar gerçekleştikçe veya gerçekleşinceye kadar defalarca icra etmesi gerekebilir. Bu defalarca çalışmayı sağlayan komutlara döngü (çevrim) yapıları denir. Döngü (loop) deyimleri, bir kümenin belli bir koşul altında tekrar edilmesi için kullanılır.​

Döngü (loop) deyimleri, bir işlemi yerine getiren kod kümesinin belli bir koşul altında tekrar edilmesi için kullanılır.​

Bir değişken belirli bir değerden başlayıp, son değeri alıncaya kadar belirtilen işlemler tekrarlanır.​
Örn: n! değerinin hesaplanması (faktöriyel)​
​
Genellikle bir programlama dilinde birden fazla döngü çeşidi bulunmaktadır. Döngü çeşitleri kullanım yerlerine göre kolaylıklar sağlamaktadır.Döngü yapıları genelde karşımıza iki tür olarak çıkar. Çalışma sayısının belli olduğu durumlarda sayaçlı döngüler, döngü sayısının değişken olduğu durumlarda ise koşullu döngüler kullanılır.​

for,​
while,​
do...while​
olmak üzere üç tip döngü deyimi vardır.​

## WHILE DÖNGÜSÜ ​

While döngüsünde tekrar sayısı belli değildir. Döngü içerisinde oluşturduğumuz şartlara göre döngü devam eder veya sonlanır.​

Genel Kullanım Şekli​

        while(koşul)​

        {​

        //yapılacak işlemler​

        }​

### WHİLE ile Sonsuz Döngü​

        while(true){​

       System.out.println("Merhaba Java");​

        }​

Sonsuz döngüden çıkmak için break; komutunu döngünün bitmesini istediğimiz satırın altına ekleyerek döngüden çıkabiliriz.​
Koşul doğru ise döngü devam eder değil ise döngü hiç çalışmadan sonlanır.​

[While döngüsü örnekler, ve çözümleri için tıklayınız.](https://github.com/nisaefendioglu/Java-Tutorial/blob/main/Hafta%203/dongulerWhileOrnek/src/dongulerwhileornek/DongulerWhileOrnek.java)

## Do While Döngüsü​
Do while döngüsü, while döngüsünden farklı olarak koşula bakmaksızın 1 kere işlemi gerçekleştirir sonrasında koşulu kontrol eder. Koşul sağlanırsa döngüye devam eder.

Kullanım şekli :​

        do{​

        //yapılacak işlemler​

        }​

        while(koşul);​

[Do-While döngüsü örnekler, ve çözümleri için tıklayınız.](https://github.com/nisaefendioglu/Java-Tutorial/blob/main/Hafta%203/dongulerDoWhile/src/dongulerdowhile/DongulerDoWhile.java)

## For Döngüsü​
Yazmış olduğumuz kodu birden fazla kez çalıştırmak istediğimizde For döngüsünden yararlanırız. Bu döngü türünde belli bir aralık belirtilir ve bu aralık boyunca döngü çalışır.​

Genel Kullanım Şekli:​

        for(başlangıç değeri, koşul, artış/azalış miktarı){​

        //işlemler​

        }​

[For döngüsü örnekler, ve çözümleri için tıklayınız.](https://github.com/nisaefendioglu/Java-Tutorial/blob/main/Hafta%203/dongulerFor/src/dongulerfor/DongulerFor.java)

## Sonsuz For Döngüsü​
For ile sonsuz bir döngü yaratmak istediğinizde for(;;) kullanabilirsiniz. 

Örnek;​

        for(;;){​

            System.out.println("java");​

        }​

## İç İçe For Döngüsü​

İç içe döngüler, döngülerin iç içe kullanılmasına verilen isimdir. Buna göre bir döngü (loop) bir dönüşünü tamamlamadan diğer bir veya birkaç döngü dönme işlemi gerçekleştirebilir.
[İç içe for döngüsü örnekler, ve çözümleri için tıklayınız.](https://github.com/nisaefendioglu/Java-Tutorial/blob/main/Hafta%203/ic%C4%B0ceForDongusu/src/icicefordongusu/Ic%C4%B0ceForDongusu.java)

## Gelişmiş For Döngüsü​
Modern programlama dillerinin hepsinde for-each kavramı benimsenmiş ve programcıların gereksinim duyduğu standart bir özellik haline gelmiştir. For-each olarak bildiğiniz bu döngü Java’da bulunmamaktadır. C# gibi dillerin aksine Java, for-each döngüsünün yaptığı işi, for döngüsü içerisine entegre etmiştir. Yani Java’da bu döngünün gerçekleştirdiği işlemler for döngüsünün gelişmiş bir versiyonu tarafından yerine getirilir. Özel for olarak da adlandırılan bu yapı, dizi ve koleksiyon tabanlı nesneler üzerinde, baştan sonra kadar ilerleyen sıralı bir döngü oluşturmak için tasarlanmıştır.​

Gelişmiş For döngüsü, For döngüsü ile oluşturulmuş olan döngüleri daha kısa bir şekilde yazmamızı sağlayan döngüdür.​
​
Gelişmiş for döngüsünün genel biçimi aşağıdaki gibidir.​
​
        
        for(tip:değişken){​

        //ifade bloğu​

        }​

Burada dikkat edilmesi gereken nokta koleksiyonda ya da dizide yer alan verinin tipiyle değişkenin tipinin birbiriyle uyumlu olmasıdır.​
​

Örnek :

        int [] dizi={1,2,3,4,5};​

        for(int i: dizi)​

        System.out.println(i+"");​
            
            

