### Reaktif Programlama
Günümüzde çoğu programlama dili prosedürel programlama temelinde çalışmaktadır. Bu yaklaşım ile, problemin çözüm aşamalarını yazılımcı adım adım kodlar. Makine ise bu aşamaları adım adım çalıştırarak verileri işler ve sonuç üretir. Oluşturulan kod yapısı ardışıl olarak oluşturulmuş aşamalara ve sürecin sonuna odaklanmıştır ve sarsılmaz bir şekilde bu süreç işlenmektedir. Eğer ki bu ardışıl yapıdaki sürece farklı bir parametre, yan etki(side effect) katılmaya çalışırsa yapı buna müsade etmeyecek, sıralama ya baştan yapılması gerekecek ya da tüm çalışmalar geri alınarak,(callback) hesap tekrardan uygulanacaktır.

Işte burada sürece katılmaya çalışan, farklı değerleri kodun akış sürecindeki herhangi bir ‘T’ noktasında işleme alınabilecek şekilde yapan tasarımlara sahip uygulamalara ya da kod parçacıklarına **Reaktif Programlama** denmektedir. Reaktif programlama, bir akışta çeşitli aşamalardan geçen verilerin sonucudur.

## **OOP ile Reaktif Programlama Arasındaki Fark Nedir?**

OOP’de yazılımlar, gerçek hayattaki olguları nesneler ile modelleyerek tasarlamaktadır.

Reaktif programlamada ise gerçek hayattaki olaylar baz alınarak tasarım gerçekleştirilmektedir.

## **X = Y+Z Denklemini ele alırsak;**

**Prosedürel programlama da,** denklemden sonraki süreçte Y ve X değişkenlerinden birinin değeri değişirse bu değişiklik X değişkenine yansımaz. Çünkü ardışıl işlem sıralamasında X değişkeninin değeri çoktan belirlenmiştir ve artık bu değer Y ve Z den bağımsızdır.

**Reaktif programlama** **da** ise Y ve Z değişkenlerinin değeri değiştiğinde X değişkeninin değeri yeniden şekillenir. Çünkü olaylar baz alınacağından dolayı sistem X değişkeninin değerini Y ve Z değişkenlerinin toplam sonucuna bağlamaktadır. Yani X değişkeninde değişiklik yapılmasına izin verecektir.

## RxJava
RxJava, JVM (Java Virtual Machine) için geliştirilmiş bir reactive programlama kütüphanesidir.

# **Asenkron nedir?**

Program parçacıklarının aynı anda farklı katmanlarda çalışmasıdır.

# **Event-based nedir?**

Klasik program akışı yukarıdan aşağıya doğru gerçekleşir,ancak event-based programlarda akışı olay belirler. Kod parçası çağrıldığında çalışır ve işlemi farklı bir katmanda yapıp sonucu iletir.Bu esnada program akmaya devam eder.Asenkron ve event-based bir program aynı anda birden çok işi,en az kaynak ile yapabilir.

# **RxJava çalışma yapısı**

[https://miro.medium.com/max/630/0*twRFMlvyfTWb07Vi](https://miro.medium.com/max/630/0*twRFMlvyfTWb07Vi)

RxJava da ReactiveX’den türetilmiş java için kullanabileceğiniz bir kütüphanedir. ReactiveX yapısında iki temel unsur vardır. Bunlar **Observer** ve **Observable.**

**Observable** : Veriyi dışa aktaran yapıdır.

**Observer** : Observable tarafından dışa aktarılan veriyi dinleyen yapıdır.

Observer ,Observable’ı dinleyerek Observable tarafından aktarılan veriyi alır. Dinleme işlemi farklı threadlerde gerçekleştirebilir.

# **RxJava’da bulunan temel unsurlar**

**Flowable,Observable,Single,Completable :** Bu yapılar yukarıda bahsettiğimiz observable unsurunun parçalarıdır. Veri üzerinde işlemler yapıp,dışa aktarırlar.

**Subsciption :** Observable ile Observer arasındaki bağlantıyı sağlar.

**Operator :** Özelleşmiş tipleri ile veri üzerinde sıralama,filtreleme gibi birçok işlem yapmanızı sağlar.

**Scheduler :** İşlemin gerçekleştiği katmanlardır.

**Subscriber :** İşlemin tamamlanmasının ardından cevabın gönderileceği yerdir.
