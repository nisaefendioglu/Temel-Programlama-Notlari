### SOLID Prensipleri
**SOLID** yazılım prensipleri; geliştirilen yazılımın esnek, yeniden kullanılabilir, sürdürülebilir ve anlaşılır olmasını sağlayan, kod tekrarını önleyen ve Robert C. Martin tarafından öne sürülen prensipler bütünüdür. Kısaltması Michael Feathers tarafından tanımlanan bu prensiplerin amacı;

- Geliştirdiğimiz yazılımın gelecekte gereksinimlere kolayca adapte olması,
- Yeni özellikleri kodda bir değişikliğe gerek kalmadan kolayca ekleyebileceğimiz
- Yeni gereksinimlere karşın kodun üzerinde en az değişimi sağlaması,
- Kod üzerinde sürekli düzeltme hatta yeniden yazma gibi sorunların yol açtığı zaman kaybını da minimuma indirmektir.

Bu prensipler uygulanarak uygulamalarımızın büyürken, karmaşıklığın da büyümesinin önüne geçmiş oluruz. “İyi kod” yazmak için bu prensiplere uygun yazılım geliştirmelisiniz.

Biraz açalım;

## **S — Single-responsibility principle**

**ÖZET:** Bir sınıf (nesne) yalnızca bir amaç uğruna değiştirilebilir, o da o sınıfa yüklenen sorumluluktur, yani bir sınıfın(fonksiyona da indirgenebilir) yapması gereken yalnızca bir işi olması gerekir.

## **O — Open-closed principle**

**ÖZET:** Bir sınıf ya da fonksiyon halihazırda var olan özellikleri korumalı ve değişikliğe izin vermemelidir. Yani davranışını değiştirmiyor olmalı ve yeni özellikler kazanabiliyor olmalıdır.

## **L — Liskov substitution principle**

**ÖZET**: Kodlarımızda herhangi bir değişiklik yapmaya gerek duymadan alt sınıfları, türedikleri(üst) sınıfların yerine kullanabilmeliyiz.

## **I — Interface segregation principle**

**ÖZET**: Sorumlulukların hepsini tek bir arayüze toplamak yerine daha özelleştirilmiş birden fazla arayüz oluşturmalıyız.

## **D — Dependency Inversion Principle**

**ÖZET**: Sınıflar arası bağımlılıklar olabildiğince az olmalıdır özellikle üst seviye sınıflar alt seviye sınıflara bağımlı olmamalıdır.

Her bir prensibi ihlal eden ve doğru olan örnekleriyle birlikte detaylı olarak açıklayacağım bir yazı dizisi olacaktır. Burada hem uygulama yanlışlarını hem de dogru uygulanışını görerek daha iyi anlama ve teknik anlamda kolayca uygulanabilmesi amaçlanmıştır. S.O.L.I.D. temel olarak her yazılımcının öğrenmesi ve yazılım hayatı boyunca uygulanması gereken önemli prensipler bütünüdür.
