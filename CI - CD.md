### CI / CD
### CI(Continuous Integration)/CD(Continuous Delivery & Deployment) Nedir?

**CI (Continuous Integration/Sürekli Entegrasyon):** Geliştirdiğimiz projenin kaynak dosyalarının bir iş akışı sürecinden (Workflow/Pipeline) geçen kontrol ve derleme adımlarına CI denir. Bu süreçte kaynak dosyalar derlenmeden önce kırılmalar var mı, kalite süreçleri sağlıklı uygulanmış mı gibi kontrol mekanizmaları çalışır ve yeni eklentilerin tutarlılığı kontrol edilir. Beklenen standartların sağlanması durumunda uygulama paketleri oluşturulur.

**CD (Continuous Delivery&Deployment/Sürekli Teslimat&Dağıtım):** CI süreci sonrasında oluşan paketlerin ilgili ortamlarda teslim edilmesi/dağıtılması sürecidir. Teslimat daha çok ilgili ekipler tarafından yapılırken dağıtım daha çok sistem tarafından otomatik yapılır. Mesela Test ortamına çıkılacak paketler otomatik yapılabilir, prod ortamına çıkacak paketler bir ekip tarafından yapılabilir.

### CI/CD Neden önemlidir?

Bu konu üzerine ayrı bir yazı hedefliyorum ancak kısaca özetlemek için şunları söyleyebiliriz:

- Sürekli devam eden operasyonel işler geliştiricilerin ve altyapı ekiplerinin zamanını çok almakla birlikte, tekrar eden benzer işler olduğu için hataya açık olabiliyor. Bu sebeple süreçlerin otomatikleştirilmesine ihtiyaç duyuluyor.
- Derleme ve Paketleme süreçleri CPU ve RAM ağırlıklı işlemler olduğu için geliştiricinin makinesini yoruyor ve çalışmasına engel olabiliyor. Bu durumda geliştirici paketleme sürecinde – ki bu bazen 2-3 saat sürebiliyor- diğer çalışmalarını yapamıyor ve bloke oluyor.
- Her geliştiricinin ortamı (kullanılan IDE, kütüphane versiyonları gibi.) farklı olabileceğinden dolayı paketleme sonrasında farklı sonuçlar doğabiliyor. Bazen de önbellek tabanlı sorunlar oluşabiliyor. Bu sebeple ekiplerin ortak kullanabileceği bir ortama ihtiyaç duyuluyor.
- Kurumsal organizasyonlarda standartları oluşturmak ve korumak için herkesin ortak bir yapı kurması, tecrübeler doğrultusunda bu yapının iyileştirilerek kişi bağımsız bir yapı oturtulmasına ihtiyaç bulunuyor.
- Paketleme ve Dağıtım, geliştiricinin temel görevleri arasında değildir. Bu tip operasyonlar farklı bir disiplin olduğu için rol çatışması yaşanabiliyor.

Mobil dünya için ön plana çıkan  CI/CD ürünleri;

- Appcircle
- Bitrise
- Codemagic
- VS App Center

### **Neden CI/CD ihtiyacı duyarız?**

- Tekrar eden işleri otomatize hale getirir.
- Tüm testlerin kontolünü sağlar. Kod kalitesini arttırır.
- Büyük projelerde uzun süren kurulum süreçlerinde insan payını indirir ve zamandan tasarruf sağlar.
- Paketin kuruluma hazır olup olmadığını denetler.
