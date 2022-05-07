### MVP, MVC, MVVM
### **Mimari Yapılar MVC MVVM MVP VIPER Nedir?**

Bu bölümde mimari yapılar MVC, MVP, MVVM ve VIPER ı inceleyeceğiz. Öncelikle neden bir mimari yapıya ihtiyaç duyarız?

Mimari yapıları açıklamadan önce buna bir göz atalım.

1. Teste dayalı uygulama geliştirmeyi kolaylaştırır.
2. Yazma ve okuma için kodları basitleştirir.
3. Katmanlı yapısı sayesinde karışıklığı engeller.
4. Tüm katmanlar arasındaki bağımlılığı azaltmaya yardımcı olur.

### **Mimari Yapılar – MVC**

**MVC**, Model, View ve Controller kelimelerinin baş harflerinden oluşan bir yazılım mimari desenidir.

**MVC** deseni, 3 katmandan oluşmaktadır ve katmanları birbirinden bağımsız olarak çalışmaktadır. Bu sebeple projelerin yönetiminin ve kontrolünün daha rahat sağlanabilmektedir. **MVC** ile geliştirilen projelerde projenin detaylarına göre bir çok kişi eş zamanlı olarak kolaylıkla çalışabilmektedir.

![https://i0.wp.com/www.teknokodi.com/wp-content/uploads/2021/04/mvcnedir.jpg?resize=500%2C292&ssl=1](https://i0.wp.com/www.teknokodi.com/wp-content/uploads/2021/04/mvcnedir.jpg?resize=500%2C292&ssl=1)

**Model Nedir?**Model, MVC’de projenin iş mantığının (business logic) oluşturulduğu bölümdür. İş mantığıyla beraber doğrulama (validation) ve veri erişim (data access) işlemleri de bu bölümde gerçekleştirilmektedir.Model tek katmandan oluşabileceği gibi kendi içinde birden fazla katmandan da oluşabilir. İç yapılandırma projenin büyüklüğü ile yazılım geliştiricinin planlamasına kalmış bir durumdur. Eğer proje büyük çaplı ise modeli birden çok katmana ayırmak projenin yönetimi açısından faydalı olacaktır.

**View Nedir?**View, MVC’de projenin arayüzlerinin oluşturulduğu bölümdür. Bu bölümde projenin kullanıcılara sunulacak olan HTML dosyaları yer almaktadır. Projenin geliştirildiği yazılım dillerine göre dosya uzantıları da değişebilmektedir.View’ın bir görevi de, kullanıcılardan alınan istekleri controller’a iletmektir.

**Controller Nedir?**Controller, MVC’de projenin iç süreçlerini kontrol eden bölümdür. Bu bölümde View ile Model arasındaki bağlantı kurulur. Kullanıcılardan gelen istekler (request) Controller’larda değerlendirilir, isteğin detayına göre hangi işlemlerin yapılacağı ve kullanıcıya hangi View’ın döneceği (response) belirtilir.

### **Mimari Yapılar – MVVM**

**MVVM**, Model, View ve ViewModel kelimelerinin baş harflerinden oluşan ve  “sorumlulukların ayrıştırılması” esasına göre geliştirilmesi temeline dayanan bir yazılım mimari desenidir. MVC deki Controller yerini MVVM de ViewModel almaktadır.

![https://i1.wp.com/www.teknokodi.com/wp-content/uploads/2021/04/mvvmnedir.png?resize=640%2C177&ssl=1](https://i1.wp.com/www.teknokodi.com/wp-content/uploads/2021/04/mvvmnedir.png?resize=640%2C177&ssl=1)

**Model Nedir?**Veritabanından, web servislerinden ya da herhangi bir veri kaynağından gelen verilerimizi temsil etmek için kullanılan entity sınıflarından oluşmaktadır. Ayrıca veri tutarlığını ve doğruluğunu kontrol eden iş kuralları da burada yer almaktadır

**View Nedir?**Bu kısım verilerimizi son kullanıcılara aktardığımız görsel ara yüzdür. Son kullanıcı ile uygulama arasında bir köprü görevi görür.

**ViewModel Nedir?**ViewModel ise görsel arayüz ile model arasında köprü görevi görmektedir, yani Model’i View’a bağlayan yapıdır. View ile Model arasında doğrudan bir etkileşim yoktur. View, ilgili işlemleri ViewModel üzerinden yapmaktadır. ViewModel’ın View’a direkt erişimi yoktur ve View ile ilgili hiçbir şey bilmez.

### **Mimari Yapılar – MVP**

**MVP**,  **MVC’den** evrilmiş bir mimaridir ve Controller’ın yerine Prenseter geliyor. Model, View ve Presenter dan oluşur.

![https://i2.wp.com/www.teknokodi.com/wp-content/uploads/2021/04/mvpnedir.png?resize=640%2C511&ssl=1](https://i2.wp.com/www.teknokodi.com/wp-content/uploads/2021/04/mvpnedir.png?resize=640%2C511&ssl=1)

**Model Nedir?**View de görüntülenecek veya başka bir şekilde davranacak verilerin işlendiği kısımdır. Presenter’ın ihtiyaç duyduğu bilgileri sağlar. İş mantığı bu kısımda ele alınır.

**View Nedir?**Verilerin görüntülendiği ve işlem yapmak için kullanıcı ile etkileşime geçilen kısımdır. **MVP** tasarım deseninde iki çeşit View kullanılabilir.

- Supervising Controller View
- Passive View

**Presenter Nedir?**Model ile View arasındaki bağlantıyı sağlayan kısımdır. Verileri modelden alır ve UI mantığını uygular. Ayrıca View’dan gelen kullanıcı etkileşimlerine tepki verir.

### **Mimari Yapılar – VIPER**

**VIPER,** adını View, Interactor, Presenter, Entity ve Router ’ın ilk harflerinden alan bir yazılım mimarisidir.

![https://i1.wp.com/www.teknokodi.com/wp-content/uploads/2021/04/vipernedir.png?resize=640%2C480&ssl=1](https://i1.wp.com/www.teknokodi.com/wp-content/uploads/2021/04/vipernedir.png?resize=640%2C480&ssl=1)

**View Nedir?**

VIPER mimarisinde view passive görevdedir ve Presenter’ın kendisine gösterilecek içeriği vermesini bekler. Hangi içeriğin gösterileceği View’e bağlıdır. Kullanıcı actionları presenter’a yönlendirir.

**Interactor Nedir?**

Business logic işlemlerinin yapıldığı kısımdır ve uygulamanın omurgasını oluşturur. Bu katmanda yapılan işlemler tamamen UI dan bağımsız olmalıdır.

**Presenter Nedir?**

Presenter esas olarak view ile ilgili logic’i içeren kodu içerir. User işlemlerine göre Interactor’dan data alır ve bunu gösterilmek üzere View katmanına iletir. View ile Interactor arasında bir köprü görevi görür. Bu katmanda view ile ilgili veya uygulamanın business kurallarıyla ilgili kod bulunmamalıdır.

**Entity Nedir?**

Interactor tarafından kullanılan model nesnelerini içerir. Entity’lerin sadece Interactor tarafından kullanılması çok önemlidir. Interactor asla presenter layer’a entity modellerini göndermez.

**Router Nedir?**

Hangi ekranların ne zaman gösterileceğini belirlendiği uygulama geçiş akışın bulunduğu katmandır. Ayrıca geçiş animasyonlarda bu katmanda bulunur. Router yalnızca Presenter ile iletişime geçer.

**VIPER mimarisinin avantajları**

1. Kodun test edilebilirliğini ve tekrar kullanılabilirliğini sağlar.

2. Rollerine göre uygulamayı komponentlere böler ve ilgili kodların birbirinden bağımsız ayrılmasını sağlar.

3. Yeni özelliklerin eklenmesini kolaylaştırır.

4. UI logic Business logicden ayrı yazıldığı için otomated testlerin yazımını kolaylaştırır.

**VIPER mimarisinin dezavantajları**

1. Küçük projelerde karmaşıklığı artırır.

2. Tüm ekibin paterni iyi bilmesi ve ona uygun kod yazması gerekir.

3. Projeye yeni başlayanlarda paterne uygun kod yazması için öğrenme süreci gerektirir.
