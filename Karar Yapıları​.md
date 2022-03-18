# Karar Yapıları​

Herhangi bir uygulama yazılırken yazılan kodların çalışma sırası, her satırın tek tek okunması ile olur. Ama bazen bazı kod bloklarının atlanması veya bir koşula bağlı olarak çalışması istenir. Tam burada karar yapıları bizim için kolaylık sağlar.​

Örnek: Eğer hava güneşli ise dışarı çıkacağım, değilse dışarı çıkmayacağım.​

​<img width="317" alt="Screen Shot 2022-03-18 at 12 57 58" src="https://user-images.githubusercontent.com/48391281/158981823-c2071272-d94f-49f3-8ebc-9f7887dd9473.png">

# If , Else , Else İf​
Java’da koşula bağlı durumlar oluşturmak için if, else if ve else ifadeleri kullanılır.​

if koşulu geçerli değilse ve else if ve else koşulları varsa sırasıyla bunları da kontrol eder. ​

## İF - ELSE​

if (koşul ifadesi) { ​

koşulun doğru olması durumunda işletilecek kod parçacığı ​

} ​

else { ​

koşulun doğru olmaması durumunda işletilecek kod parçacığı ​

} ​

[if - else örnekler, ve çözümleri için tıklayınız.](https://github.com/nisaefendioglu/Java-Tutorial/blob/main/Hafta%202/ifElse/src/ifelse/IfElse.java)

## İF - ELSE İF​

if - else if deyimleri, bir koşulun sağlanmadığı durumda diğer koşul ya da koşulların denetlenmesini sağlayan bir yapıdadır. ​

Denetlenen koşullardan herhangi birisinin sonucu mantıksal doğru olursa, o kod bloğu işletilir ve programın akışı en sonraki else bloğunun bitimine sapar. ​

Hiç bir koşul doğru değilse, o zaman else bloğu işletilir. else bloğunun yazılması zorunlu değildir.​

if (1. koşul ifadesi) { ​

koşulun doğru olması durumunda işletilecek kod parçası ​

} else if (2. koşul ifadesi) { ​

2. koşulun doğru olmaması durumunda işletilecek kod parçası ​

}  ​

…// istenildiği kadar else if bloğu ​

else { ​

hiçbir koşulun doğru olmaması durumunda işletilecek kod kesimi ​

} ​

[if - else if örnekler, ve çözümleri için tıklayınız.](https://github.com/nisaefendioglu/Java-Tutorial/blob/main/Hafta%202/ifElseIf/src/ifelse%C4%B1f/IfElseIf.java)

## İç İçe İF Deyimi​
Bir if bloğunun içine başka if deyimi ya da deyimleri de gelebilir. Burada herhangi bir sınır yoktur. Algoritmaya göre, iç içe if deyimleri yazılabilir.​
​

int a = 7, b = 3, c = 1;​

if (a > b) { ​

System.out.println("a, b'den büyüktür."); ​

if (a > c) { ​

System.out.println("a, c'den de büyüktür."); ​

 } ​

else { ​

System.out.println("a, c'den büyük değildir."); ​

  } ​

} ​

[İç içe if-else örnekler, ve çözümleri için tıklayınız.](https://github.com/nisaefendioglu/Java-Tutorial/blob/main/Hafta%202/ic%C4%B0ce%C4%B0fElse/src/iciceifelse/Ic%C4%B0ce%C4%B0fElse.java)

# Switch Case​
switch deyimi, if-else-if deyimleri ile yazılabilecek bir kod kesimini daha basitçe yazmayı sağlayan, bir ifadenin değerine göre dallanmayı sağlayabilen bir deyimdir. ​

switch (ifade) { ​

case deger1: ​

ifadeler; ​

break; ​

case deger2: ​

ifadeler; ​

break; ​

.... ​

case degerN: ​

ifadeler; ​

break; ​

default: ​

ifadeler; ​

} ​

[Switch Case örnekler, ve çözümleri için tıklayınız.](https://github.com/nisaefendioglu/Java-Tutorial/tree/main/Hafta%202)

