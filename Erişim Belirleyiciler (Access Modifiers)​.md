### Erişim Belirleyiciler (Access Modifiers)​
Nesne Yönelimli Programlamada erişim belirleyiciler ufak bir yere sahip olsalar da, hatta bir çok derste bahsi geçmese de önemli konulardan bir tanesidir. Java’da proje oluştururken paket mantıksal yapıları sınıf bazında ayırmanın yanı sıra paket yapısıyla da ayırmamız mümkündür. Java ile proje geliştirirken paket yapısı olmazsa olmaz denilebilir. Paket yapısı projenin geliştirildiği web sitesi veya firmanın domain adını içerecek şekilde tersten oluşturulur. ​

Paket yapıları kurulduktan, sınıflar bu paketler altında yerlerini aldıktan, ve sınıflar içerisinde farklı görevlere sahip metotlar oluşturulduktan sonra sınıfların farklı sınıflardaki metotlara erişim sağlaması gerekmekte veya bir sınıftaki özel bir metoda başka hiç bir sınıfın erişememesi gerekmektedir. İşte bu gibi durumları belirlediğimiz yapı Erişim belirleyicilerdir. 

Public : Herkes ulaşabilir.​

Protected : Olduğu sınıftan, olduğu sınıftan türetilmiş sınıflardan ve olduğu sınıfla aynı pakette bulunan sınıflar erişebilir.​

Private : Yalnızca tanımlanmış olduğu sınıftan erişim sağlanır.​

Default : Herhangi bir erişim belirleyici tanımlanmadığı esnada default olarak kabul edilir. Default olarak tanımlanan sınıf elemanlarına o sınıftan ve aynı paketteki sınıftan erişilebilir.​

<img width="717" alt="Screen Shot 2022-04-03 at 21 18 55" src="https://user-images.githubusercontent.com/48391281/161442280-53fe9108-4414-49be-b05d-b8d60144b567.png">

[Erişim Belirleyici örnekleri, ve çözümleri için tıklayınız.](https://github.com/nisaefendioglu/Java-Tutorial/tree/main/Hafta%206)
