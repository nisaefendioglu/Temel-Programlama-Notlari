### Reaktif Programlama
Günümüzde çoğu programlama dili prosedürel programlama temelinde çalışmaktadır. Bu yaklaşım ile, problemin çözüm aşamalarını yazılımcı adım adım kodlar. Makine ise bu aşamaları adım adım çalıştırarak verileri işler ve sonuç üretir.Oluşturulan kod yapısı ardışıl olarak oluşturulmuş aşamalara ve sürecin sonuna odaklanmıştır ve sarsılmaz bir şekilde bu süreç işlenmektedir. Eğer ki bu ardışıl yapıdaki sürece farklı bir parametre, yan etki(side effect) katılmaya çalışırsa yapı buna müsade etmeyecek, sıralama ya baştan yapılması gerekecek ya da tüm çalışmalar geri alınarak,(callback) hesap tekrardan uygulanacaktır.

Işte burada sürece katılmaya çalışan, farklı değerleri kodun akış sürecindeki herhangi bir ‘T’ noktasında işleme alınabilecek şekilde yapan tasarımlara sahip uygulamalara ya da kod parçacıklarına **Reaktif Programlama** denmektedir. Reaktif programlama, bir akışta çeşitli aşamalardan geçen verilerin sonucudur.

## **OOP ile Reaktif Programlama Arasındaki Fark Nedir?**

OOP’de yazılımlar, gerçek hayattaki olguları nesneler ile modelleyerek tasarlamaktadır.

Reaktif programlamada ise gerçek hayattaki olaylar baz alınarak tasarım gerçekleştirilmektedir.

## **X = Y+Z Denklemini ele alırsak;**

**Prosedürel programlama da,** denklemden sonraki süreçte Y ve X değişkenlerinden birinin değeri değişirse bu değişiklik X değişkenine yansımaz. Çünkü ardışıl işlem sıralamasında X değişkeninin değeri çoktan belirlenmiştir ve artık bu değer Y ve Z den bağımsızdır.

**Reaktif programlama** **da** ise Y ve Z değişkenlerinin değeri değiştiğinde X değişkeninin değeri yeniden şekillenir. Çünkü olaylar baz alınacağından dolayı sistem X değişkeninin değerini Y ve Z değişkenlerinin toplam sonucuna bağlamaktadır. Yani X değişkeninde değişiklik yapılmasına izin verecektir.
