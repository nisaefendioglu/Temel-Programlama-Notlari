### ENUM KAVRAMI​
Enum, önceden türleri tanımlanmış olan sabitlerdir. Kodun okunabilirliği arttırır ve tip güvenliğini arttırmaya yardımcı olurlar.​

Genelde değerleri değişmeyen günler, aylar, sayılar gibi tanımlamalar yapmak için kullanılır.​

Enumlar sınıflara benzer. Kendilerine ait yapıcı metodları vardır. Bünyesinde üyeler barındırır fakat new anahtar kelime ile nesne oluşturulamaz.​

Enum tanımlamak için enum anahtar kelimesinden yararlanırız​

## ORDİNAL METODU​
Enum elemanlarının indisini öğrenmek için ordinal metodundan yararlanırız.​

Enumlar yapısal olarak hem dizilere hem de sınıflara benzerler.​

Diziye benzeyen kısmı, enum elemanlarının da indisleri vardır ve dizilerde olduğu gibi bu indis değeri 0'dan başlar.​

Enum elemanının indisini öğrenmek için ordinal() metodundan yararlanırız.​

https://github.com/nisaefendioglu/Java-Tutorial/blob/main/Hafta%207/ordinalMetodu/src/ordinalmetodu/OrdinalMetodu.java

Örnek : 

Aylar adında enum metodu oluşturun ve içerisine ayları aktarın. Ardından şubat ayının indisini aldırarak switch case ile alınan indisin hangi aya denk geldiğini yazdıran programı yazınız.​

[Çözüm](https://github.com/nisaefendioglu/Java-Tutorial/blob/main/Hafta%207/EnumAylar/src/enumaylar/EnumAylar.java)
