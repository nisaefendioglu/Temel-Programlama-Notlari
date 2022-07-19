# Enum Classes Nedir?
Enum sınıflar numaralandırma işlemlerinin yazılımdaki karşılıklarıdır. Tek bir tipteki veriyi gruplandırmak ve daha temiz kod yazabilmek adına enum classları kullanabiliriz.

Proje içerisinde bazı durumlarda koşula göre uygulamayı çalıştırmak gerekebilir. Örneğin uygulamamızda hem admin hem de user’a göre özelleştirilmiş iki farklı ekran var. Burada admin tipine 0 değerini, user tipine de 1 değerini atayarak gerekli koşul sağlandığında o ekranı gösterebiliriz. Peki nasıl yazabiliriz?
```
if(type==0)
{
//admin tipinde gösterilecek olaylar
}
else if(type==1)
{
//user tipinde gösterilecek olaylar
}
```
Gördüğünüz üzere bu kod çok da temiz ve anlaşılır bir kod değil. Bir süre sonra 1 veya 0 ifadesinin hangi tipe ait olduğunu bulmak işimizi zorlaştırabilir. Tam da bu noktada enum classları kullanırız.

Gelin bir enum class oluşturalım;
```
enum class USER_TYPE(val id: Int) {
    ADMIN(0),
    USER(1)
}

if (type == USER_TYPE.ADMIN) {
//admin tipinde gösterilecek olaylar
} 
else if (type == USER_TYPE.USER) {
//user tipinde gösterilecek olaylar
}
```
Bu kod bir önceki kod blogumuza göre çok daha anlaşılır bir yapıya sahip. Artık admin veya user kullanıcısının id numarasını kolayca kontrol edebileceğimiz bir USER_TYPE class’ımız bulunmakta.

# Sealed Classes Nedir?
Sealed classlar enum classların genişletilmiş halidir. Enumlar tek bir değişken tipi tutabilirken Sealed sınıflar içerisinde farklı veri tipleri barındırabilir. Enum classlardaki tek tip değişken sorunuyla karşılaşmamız durumunda gerçekleştirmek istediğimiz birçok işlemi gerçekleştiremeyebiliriz. Bu durumda ise sealed classlardan faydalanabiliriz.

Örneğimizi ilk olarak enum classları kullanarak gerçekleştirmeye çalışalım.

Öğrenci ders kayıt sistemimiz olsun ve öğrenciler derslere kayıtlı olsun.

Lessons adında bir data class oluşturalım ve öğrencinin ders kayıt sistemi üzerinden bu dersleri görüntüleyebiliyor olalım.
```
data class StudentInfo(var name: String, var age: Int)
```
Bu bilgileri enum class içerisinde parametre olarak alacağız.
```
enum class StudentRegistrations(val get: StudentInfo) {
    PythonLesson(
        StudentInfo(
            "Nisa",
             23 
     )
  ),
    AndroidLesson(
	StudentInfo(
	    "Halise"
	     22
        )
    )
}
```
Sınıfımızda iki öğrenci ve kayıt oldukları dersler bulunuyor. Burada Nisa isimli öğrenci Python dersinde bulunan kaydını iptal etmek istiyor. Bu durumda sonradan silinen kayıtların bilgisini de tutmak isteyebiliriz.

Örneğin derslerden ayrılan kişiyi DeletedRegistrations olarak adlandıralım. Dersten kaydı silinen öğrencilerin o derse ait bilgileri elimizde bulunmadığı için elimizdeki parametreler boş olarak kalacaktır. Enum classlar tek bir veri türü içermesinden dolayı ise DeletedRegistrations’ı kullanmamız mümkün olmayacaktır. Çünkü enum class’ımız bizden bir parametre bekliyor olacak. (StudentInfo(var name: String, var age: Int))

Bu durumda ise devreye sealed classlar girmektedir. Sealed class kullanarak;
```
sealed class StudentRegistrations
data class PythonLesson(val info: StudentInfo) : StudentRegistrations()
data class AndroidLesson(val info: StudentInfo) : StudentRegistrations()
object DeletedRegistrations : StudentRegistrations()
```
bu şekilde DeletedRegistrations objemizi oluşturabilir ve kullanabiliriz.

## Enum Class ile Sealed Class Farkları
- Enumlar tek bir değişken tipi tutabilir, Sealed Sınıflar ise her bir state için farklı değişken tipi tutabilirler.
- Enum classlarda tanımlanan bir parametre varsa tüm değerler oluşturma anında bu veri set edilmeli. (Sistemden bir kişiyi sildik deletedUser isimli değişkene silinen kişiyi atadık fakat burada değerler boş olacağından dolayı parametreler boş kalacaktır. Enum classlarda da tek tip veri barındırabildiğimiz için bunu yapabilmek mümkün olmayacaktır. Sealed class’ta ise bu işlemi gerçekleştirebiliriz.)
- Sealed classlar’dan nesne üretemeyiz. (Soyut oldukları için)
- Enumlar sabit değerler ifade etmek için kullanılır.
```
enum class USER_TYPE(val id: Int) {
     ADMIN(0), 
     USER(1)
}
```

[Medium](https://medium.com/@nisaefendioglu/enum-class-ve-sealed-class-nedir-aralar%C4%B1ndaki-farklar-nelerdir-b710c6efba1d)
