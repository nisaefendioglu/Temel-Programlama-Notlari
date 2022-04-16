### API Design
**API**, iki uygulamanın birbiriyle konuşmasına olanak tanıyan bir yazılım aracısı olan Uygulama Programlama Arayüzü’nün kısaltmasıdır. WhatsApp gibi bir uygulamayı her kullandığınızda, her anlık mesaj gönderdiğinizde veya telefonunuzda hava durumunu her kontrol ettiğinizde bir API kullanıyorsunuz.

**API Nasıl Çalışır?**

Örneğin, cep telefonunuzdaki bir uygulamayı kullandığınızda, uygulama internete bağlanır ve verileri bir sunucuya gönderir. Ardından sunucu bu verileri alır, yorumlar, gerekli eylemleri gerçekleştirir ve telefonunuza geri gönderir. Sonrasında uygulama bu verileri yorumlar ve istediğiniz bilgiyi okunabilir bir şekilde size sunar. İşte **API** budur. Bunların hepsi **API** aracılığıyla olur.Bunu daha iyi açıklamak için günlük hayattan bir benzetme yapalım:Sipariş verebileceğiniz bir menüyle bir restorandaki bir masada oturduğunuzu düşünün. Mutfak, siparişinizi hazırlayacak “sistem”in bir parçasıdır. Eksik olan şey, siparişinizi mutfağa iletecek ve yiyeceğinizi masanıza geri teslim edecek kritik bir bağlantıdır. İşte garson ya da **API** burada resme dahil olur. Garson - veya **API** - siparişinizi alan ve mutfağa - sisteme - ne yapacağını söyleyen aracıdır. Ardından garson cevabı size geri iletir; bu örnekte cevap, yiyecek ve içecekleriniz oluyor.

**API’nin Ayrıca Sağladığı** **Şey İse Bir Güvenlik Katmanıdır**

Cihazınızın (Bilgisayar, telefon veya tablet) verileri asla sunucuya tam olarak savunmasızca açık değildir ve aynı şekilde sunucu da hiçbir zaman cihazınıza tam olarak savunmasızca açık değildir. Bunun yerine, her ikisi de küçük veri paketleriyle iletişim kurar ve yalnızca gerekli olanı paylaşır.API’ler, çok sayıda işletmenin gelirinin büyük bir bölümünü oluşturduklarından dolayı çok değerlidir. Google, eBay, Salesforce, Amazon ve Expedia gibi büyük şirketler, API'lerinden para kazanan şirketlerden sadece birkaçıdır. “API ekonomisi”nin ifade ettiği şey ise bu API pazarıdır. (İlerleyen yazılarımızda bu konuya ayrıca değineceğiz.)

**Modern API**Yıllar içinde, “API” genellikle bir uygulamayla olan herhangi bir tür genel bağlantı arabirimini olarak tanımlandı. Ancak son zamanlarda, modern API, kendini olağanüstü derecede değerli ve yararlı kılan bazı özellikler edindi:

- Modern API’ler standartlara (Tipik olarak HTTP ve REST) bağlıdır.
- Koddan daha çok bir ürün gibi davranırlar. Bunlar, belirli kitlelerin (Örneğin, mobil geliştiriciler) kullanması için tasarlanır, dokümante edilir ve kullanıcıların bakımı ve yaşam döngüsü ile ilgili belirli beklentileri olabilecek şekilde biçimlendirilir, versiyonlandırılırlar.
- Daha çok standartlaştırılmış olduklarından dolayı güvenlik ve denetim konusunda daha güçlü bir disipline sahiplerdir ve ayrıca iyi bir performans ve yeterli ölçek (scale) için yönetilir ve denetlenirler.
- Ürünleştirilen yazılımın başka bir parçası olarak modern API; tasarım, test, oluşturma, yönetme ve sürüm belirleme gibi kendine ait yazılım geliştirme yaşam döngüsüne (software development lifecycle) sahiptir. Ayrıca, modern API’ler kullanım ve sürüm yenileme için iyi dokümante edilir.

API tasarımı , geliştiriciler ve kullanıcılar tarafından kullanılmak üzere veri ve uygulama işlevselliğini ortaya çıkaran uygulama programlama arabirimleri (API'ler) geliştirme sürecini ifade eder .
