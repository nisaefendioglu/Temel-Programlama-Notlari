### Web Servis
Verilerinizi web sayfanız dışında tüm cihazlara göndermek istediğinizde devreye Web Service kavramı girer. Web Service ile platform bağımsız tüm cihazlara veri aktarımı gerçekleştirilir. Facebook’da mesajlaşırken karşılıklı olarak mesajların hem web sayfasına hemde Facebook Messenger uygulamasına gelmesini Web Service sağlar. Messenger uygulaması, Android, IOS, Wİndows Phone işletim sistemli cihazlarda çalışması Web Service kavramının gücünü kanıtlamaktadır.

Kısaca Web servisler platform bağımsız olmak üzere bir çok uygulama, cihaz ya da nodeun birbiri ile iletişim kurmalarını sağlayan yapılardır.

## **Rest ve Restful Kavramları**

Rest, client-server arasındaki iletişimin HTTP protokolü sayesinde kolay ve hafif bir şekilde yapılmasını sağlayan bir mimaridir. Rest mimarisinde SOAP’da bulunan GetProduct , GetCategory gibi metotlar üzerinden iletişim kurulması yerine tüm bilgiler, URI’ler üzerinden sunulur. Örn : [http://myserver/api/v1/products/1](http://myserver/api/v1/products/1) gibi web linkleri düşünebiliriz.Restful web servisleri ise , REST mimarisi temel alınarak geliştirilmiş oldukça hafif, genişletilebilir ve basit servislerdir. Restful servislerin amacı client-server arasındaki veri akışını platform bağımsız olarak gerçekleştirebilmek ve veri akışını en az yükle sağlayabilmektir.Restful servisleri response tipi olarak JSON, HTML, XML gibi bir çok formatta çalışabilirler. Yapısının az yer kaplaması ve bir çok mobil platformda kullanışlı olmasından dolayı response tipi olarak JSON kullanılmaktadır.Restful servisleri esnek ve kolay geliştiriebilir bunun yanında dil ve platform bağımsızdırlar. SOAP servislerinin aksine ekstra bir kütüphaneye ihtiyaç duymadan çalışabilirler.Bir servisin restful olması için temel karakteristik prensipler vardır.

![https://miro.medium.com/max/630/1*2q84bNIHxAAJz3hk1o9kaQ.png](https://miro.medium.com/max/630/1*2q84bNIHxAAJz3hk1o9kaQ.png)

**Client-Server yapısı :** Client, server tarafındaki veri kaynağı ile ilgili hiç birşey bilmediği gibi, server da client hakkında birşey bilmemelidir. Server sadece kendisine gelen istekler doğrultusunda değer döner. Böylece server daha basit ve scalable olur.

**Stateless :** Server tarafında client ile ilgili hiç bir bilginini tutulmamasıdır. Client tarafından gerçekleştirielecek olan her request, serverin response dönebilmesi için geçerli bilgiyi taşır. Client ayrımı ise clientin servera request geçme esnasında göndereceği bir token veya kimlik bilgisi ile gerçekleştirilir.

**Cacheable** : Tüm HTTP responselar client tarafından cachlenebilir olmalı. Veri tutarlılığını sağlayabilmek için ise server ilgili response bilgisini dönerken, ilgili verirnin cachelebilir olup olmadığını göndermesi gerekir.

**Layered System :** Clientın server yapısındaki hangi katmana bağlandığını bilmemesidir. Bu bir ara katmanda olabilir, son katmanda. Buradaki amaç ise serverlar arasında load-balancing yaparak ölçeklenebilirliği artırmak ve clientları bazı güvenlik politikalatına da zorlayabilmektedir.

**Uniform Interface** : Client ile server arasındaki ortak bir arayüzün(interface) olması ile birbirlerinden bağımsız bir şekilde geliştirilibliyor olurlar. Bir servisin RESTful olabilmesi için en önemli prensiplerden birisidir.

## **Kimler REST Kullanıyor?**

Neredeyse Yahoo’nun tüm servisleri REST kullanır. Amazon ve eBay hem SOAP hem de REST mimarilerini kullanmaktadırlar.

## **Soap Nedir ?**

SOAP(en: Simple Access Protocol ,tr: Basit Nesne Erişim Protokolu) en temel anlamda, internet üzerinden küçük miktarda bilgileri yada mesajları aktarma protokoludur. SOAP mesajları XML formatındadırlar ve genellikle HTTP(Hyper Text Transfer Protocol) protokolu(bazende TCP/IP) kullanılarak gönderilirler. SOAP ,XML tabanlı kullanıma mecbur bırakır. Bu konuda esnek değildir.

**WSDL(Web Services Description Language):**

SOAP isteklerini oluşturmak için de bir standart gerekmektedir. İşte burada WSDL devreye girmektedir. WSDL gerçekleştirilebilecek bütün SOAP isteklerinin kayıtarını tutan, XML tabanlı web servisleri tanımlamak ve yerini belirtmek için tanımlanmış dildir. WSDL, W3C standardıdır. Bir anlamda dağıtık programlamada kullanılan IDL’e (Interface Definition Language — Arayüz Tanımlama Dili) benzer. Web servisi tanımı işlemler, giren ve çıkan mesaj formatları, ağ ve port adresleri gibi bilgileri tanımlar. Bir web servisi tanım belgesi aşağıdaki temel elemanları içerir:

***Types :*** mesajlarda kullanılacak veri tiplerini belirtir.***Message :*** İletişimde kullanılacak measjları tanımlar.***PortType :*** Web servisinin içerdiği işlemleri (methods) ve ilgili mesajları tanımlar.***Binding*** : İşlem ve mesajlarda kullanılacak veri formatlarını tanımlar.***Port :*** Binding ve web adresinden oluşan servis noktasını tanımlar. Web adresi servisin çalıştırılacağı URL’dir.***Service :*** Kullanılan port’lar kümesidir.

## **Kimler SOAP Kullanıyor?**

Buna verilebilecek en büyük örnek Google. Blogger dışında bir çok uygulamasında SOAP kullanıyor. Bir çok kurumsal yazılımda SOAP kullanıldığını görebilirsiniz.

![https://miro.medium.com/max/621/1*oeT_i1HRfxI0ndrfryVhjg.png](https://miro.medium.com/max/621/1*oeT_i1HRfxI0ndrfryVhjg.png)

# **SOAP mı REST mi?**

Geldik en önemli konuya. SOAP daha iyidir ya da REST daha iyidir hükmünün net olarak verilemeyeceğini düşünüyorum. SOAP yada REST seçimi, kullandığımız yapının uygunluğu açısından değerlendirilerek yapılması gerekiyor. Değerlendirme için bize yardımcı olabilecek bazı karşılaştırmalar ise aşağıdaki gibidir.

- SOAP, XML veri tipini desteklerken REST mimarisinde istenen veri türüyle işlem yapabilir. JSON veri tipi ile XML’den çok daha düşük boyutlarla veri tutulabildiği için REST ile daha hızlı işlem yapılabilir.
- SOAP için WSDL ile tanımlama yapmak gerekirken REST için böyle bir zorunluluk yoktur. (WADL REST için kullanılan WSDL’e benzer bir yapıdır fakat kullanma zorunluluğu yoktur.)
- Bir dile ihtiyaç duymadan HTTP methodlarıyla tasarlanabildiği için REST’i kullanması ve tasarlaması daha kolaydır.
- SOAP için birçok geliştirme aracı mevcuttur, REST için geliştirme araçlarına ihtiyaç duyulmaz, tasarlaması kolaydır.
- SOAP, XML-Scheme kullanırken REST, URI-Scheme kullanır. Yani metotlar için URI’ler tanımlanır.
- Her ikisi de HTTP protokolünü kullanırlar. Fakat REST için HTTP zorunluluğu varken SOAP, TCP/IP, SMTP gibi başka protokollerle de çalışabilir.Test ve hata ayıklama aşaması REST için daha kolaydır. Çünkü HTTP hatalarını döndürür ve bunlar bir tool ihtiyacı duyulmadan görülebilir. SOAP için hata ayıklama araçları gerekebilir.
- REST basit HTTP GET methodunu kullandığı için cacheleme işlemi daha kolaydır. SOAP ile cacheleme yapabilmek için karmaşık XML requestleri yapılmalıdır.
- İkisi de HTTPS destekler, SOAP için WS-SECURITY adlı bir eklenti mevcuttur.
- Güvenlik açısından SOAP daha gelişmiştir çünkü hazır yapılar bulunmaktadır.
- Dokümantasyon bakımından SOAP daha gelişmiştir ve daha fazla kaynak bulunmaktadır.
