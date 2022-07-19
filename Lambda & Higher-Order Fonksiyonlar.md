# Lambda & Higher-Order Fonksiyonlar

## Lambda Fonksiyonu

Lambda, programlamada herhangi bir tanımlayıcıya gerek duymayan fonksiyondur. Bir fonksiyonu tek bir satırda yazabilmenize olanak sağlar. Lambda, fonksiyonel programlama dillerinde veya diğer birinci sınıf fonksiyonlara sahip dillerde bulunabilir. (C, C++, Java, Kotlin…)
Lambda fonksiyonunu kod olarak nasıl yazarız ona bakalım.

Lambda fonksiyonu,

**(Parameter1, Parameter2) -> { Code Block }** şeklinde tanımlanır.

Örneğin lambda kullanmadan kullanıcı adını alan bir kod parçacığı oluşturalım.
```
fun name(myName: String) {
 print(myName) 
}
name("Nisa")
```

Aynı örneği lambda fonksiyonu ile gerçekleştirelim.

``` 
val name = { myName: String -> print(myName) } 
name("Nisa")
```

Gördüğünüz üzere Lambda fonksiyonları sayesinde daha az kod ile daha hızlı geliştirme sağlayabilirsiniz.

## Higher-Order Fonksiyonlar

Higher-Order fonksiyonlar parametre olarak bir veya birden fazla fonksiyon alabildiği gibi sonuç olarak bir fonksiyonu da geri döndürebilirler.

Higher-Order Fonksiyonları kod olarak nasıl yazarız ona bakalım.

**fonksiyonAdı: (parametreAdı: parametreTipi) -> fonksiyonDönüşTipi**

Örnek olarak, iki sayı alan ve sonucunda bu iki sayının toplamını bize döndüren bir Higher-Order fonksiyonu yazalım.
```
fun main() {
higherOrderFunc("Toplama",15,5, ::addition)
}
fun higherOrderFunc(operationType: String,
num1 : Int,
num2 : Int,
operation:(Int,Int) -> Int) {
	println(operationType)
	print("İşlem sonucu : ")
	println("${operation(num1,num2).toString()}")
}
fun addition(a:Int,b:Int) : Int{
return a+b
}
```
Bu kod parçacığında Higher-Order fonksiyonumuz operationType, num1, num2 ve operation fonksiyonunu parametre olarak alıyor. Bu fonksiyon sonucunda bize ilk olarak işlem türünü (operationType) yazdırarak aldığı 2 sayıyı işleme sokuyor ve sonucu bize geri döndürüyor.
