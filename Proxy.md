# TUG-Proxy-Reverse/Forward Proxy-Load Balancer-API Gateway-Traefik

## Proxy Nedir

Proxy sunucusu, kullanıcılar ile internet arasında bir ağ geçidi sağlayan bir sistem veya yönlendiricidir. Bu nedenle, siber saldırganların özel bir ağa girmesini engellemeye yardımcı olur. Son kullanıcılar ile çevrimiçi ziyaret ettikleri web sayfaları arasında bağlantı kurduğu için "aracı" olarak adlandırılan bir sunucudur. Proxy sunucusu, özünde internette kendi IP adresine sahip bir bilgisayardır. 


<img width="1207" height="684" alt="image" src="https://github.com/user-attachments/assets/e6780eaa-9a53-40d7-b430-6b68cbacbbfc" />

### Proxy Sunucuları ve Ağ Güvenliği

Proxy'ler, bilgisayarınız için değerli bir güvenlik katmanı sağlar. Web filtreleri veya güvenlik duvarı olarak kurulabilirler ve bilgisayarınızı kötü amaçlı yazılımlar gibi internet tehditlerinden koruyabilirler. Bu ekstra güvenlik , güvenli bir web ağ geçidi veya diğer e-posta güvenlik ürünleriyle birleştirildiğinde de değerlidir . Bu sayede, trafiği güvenlik seviyesine veya ağınızın (veya bireysel bilgisayarlarınızın) kaldırabileceği trafik miktarına göre filtreleyebilirsiniz. 




Proxy nasıl kullanılır? Bazı kişiler proxy'leri kişisel amaçlar için kullanır; örneğin, çevrimiçi film izlerken konumlarını gizlemek gibi. Ancak bir şirket için, aşağıdaki gibi birkaç önemli görevi yerine getirmek için kullanılabilirler:

- Güvenliği artırın
- Çalışanlarınızın internet aktivitelerini, onları gözetlemeye çalışan kişilerden koruyun
- Çökmeleri önlemek için internet trafiğini dengeleyin
- Ofisteki çalışanların ve personelin web sitelerine erişimini kontrol edin
- Dosyaları önbelleğe alarak veya gelen trafiği sıkıştırarak bant genişliğinden tasarruf edin
---

## Proxy nasıl çalışır?
Proxy sunucusunun kendi IP adresi olduğundan, bilgisayar ile internet arasında bir aracı görevi görür. Bilgisayarınız bu adresi bilir ve internet üzerinden bir istek gönderdiğinizde, istek proxy'ye yönlendirilir. Proxy, web sunucusundan yanıt alır ve sayfadaki verileri Chrome, Safari, Firefox veya Microsoft Edge gibi bilgisayarınızın tarayıcısına iletir.

### Proxy bilgisayar gizliliğini ve verilerini nasıl korur?


Proxy sunucusu, güvenlik duvarı ve filtre işlevi görür. Son kullanıcı veya ağ yöneticisi, verileri ve gizliliği korumak için tasarlanmış bir proxy sunucusu seçebilir. Bu sunucu, bilgisayarınıza veya ağınıza giren ve çıkan verileri inceler. Ardından, dijital adresinizi dünyaya ifşa etmenizi önlemek için kurallar uygular. Bilgisayar korsanları veya diğer kötü niyetli kişiler yalnızca proxy sunucusunun IP adresini görebilir. Kişisel IP adresiniz olmadan, internetteki kişiler kişisel verilerinize, programlarınıza, uygulamalarınıza veya dosyalarınıza doğrudan erişemez. Bu özellik sayesinde, web istekleri proxy'ye gider ve proxy de internete ulaşarak istediğinizi alır. Sunucu şifreleme özelliğine sahipse, parolalar ve diğer kişisel veriler ek bir koruma katmanına sahip olur.


### Proxy sunucusunun faydaları
- **Gelişmiş güvenlik** : Yukarıda bahsettik.
- **Gizli gezinme, izleme, dinleme ve alışveriş** : İstenmeyen reklamlarla boğulmaktan veya IP'nize özgü verilerin toplanmasından kaçınmak için farklı proxy'ler kullanın. Bir proxy ile site gezinmesi iyi korunur ve izlenmesi imkansızdır.
- **Konuma özgü içeriğe erişim** : Başka bir ülkeyle ilişkili bir adrese sahip bir proxy sunucusu belirleyebilirsiniz. Böylece, o ülkedeymiş gibi görünebilir ve o ülkedeki bilgisayarların etkileşim kurmasına izin verilen tüm içeriğe tam erişim sağlayabilirsiniz. Örneğin, bu teknoloji, görünmek istediğiniz konumun yerel IP adreslerini kullanarak konum kısıtlamalı web sitelerini açmanıza olanak tanıyabilir.
- **Çalışanların uygunsuz veya dikkat dağıtıcı sitelerde gezinmesini engelleyin** : Kuruluşunuzun ilkelerine aykırı web sitelerine erişimi engellemek için kullanabilirsiniz. Ayrıca, çalışanların önemli görevlerinden dikkatini dağıtan siteleri de engelleyebilirsiniz. Bazı kuruluşlar, zaman kaybına neden olan cazibeleri ortadan kaldırmak için Facebook ve benzeri sosyal medya sitelerini engeller.

---

## Proxy sunucu türleri

<img width="862" height="512" alt="image" src="https://github.com/user-attachments/assets/dc2eb010-00be-4797-ab79-f1281e7bd7f3" />

## Forward ve Reverse Proxy


<img width="799" height="846" alt="image" src="https://github.com/user-attachments/assets/5eefbfc2-5c66-444e-9b48-1c938e77a2b1" />


### Başka bir örnek fotoğraf

<img width="999" height="496" alt="image" src="https://github.com/user-attachments/assets/a505e533-590a-484c-8780-67743acef734" />


### Forward proxy

Forward proxy (aynı zamanda "proxy server" olarak da adlandırılır), istemci cihazları ile internet arasında bulunan bir sunucudur. Bir istemci bir web sitesine veya çevrimiçi kaynağa erişim isteği gönderdiğinde, istek önce forward proxy'ye yönlendirilir. Proxy daha sonra isteği istemci adına hedef sunucuya iletir. Bir istek gönderildiğinde, "proxy server" bunu inceleyerek bağlantı kurmaya devam edip etmeyeceğine karar verir. Forward proxy, tek bir giriş noktasına ihtiyaç duyan dahili ağlar için en uygunudur. Ağdakiler için IP adresi güvenliği sağlar ve kolay yönetim kontrolüne olanak tanır. Ancak, forward proxy, bir kuruluşun bireysel son kullanıcıların ihtiyaçlarını karşılama yeteneğini sınırlayabilir.Gizliliği artırmak ve erişimi kontrol etmek için istemci adına hareket eder.


### Forward proxy kullanımı

- Müşteri anonimliğini artırma
- Coğrafi olarak engellenen veya kısıtlanan içeriğe erişim
- Kuruluşlarda içerik filtreleme ve izleme
- Önbelleğe alma yoluyla bant genişliği tüketimini azaltma(Mesela aynı videoyu bir ağda herkes açıyor. Bunu tekrar çağırmak yerine direkt önbellekten gönderiyor videoyu)
- Uyumluluk için kullanıcı etkinliğinin kaydedilmesi ve izlenmesi


### Reverse proxy

Forward proxy istemci adına hareket ederken, reverse proxy sunucu adına hareket eder. İstemcilerin kaynak sunucuyla doğrudan iletişim kurmasını engelleyerek sunucuları korumak ve yönetmek için kullanılır. Reverse proxy'ler, gelen çok sayıda isteğin yükünü dengelemesi gereken popüler web siteleri için güçlü bir seçenektir. Gelen istekleri yöneten başka bir web sunucusu gibi davrandıkları için bir kuruluşun bant genişliği yükünü azaltmasına yardımcı olabilirler. Olumsuz tarafı ise, bir saldırganın sızması durumunda reverse proxy'lerin HTTP sunucu mimarisini açığa çıkarabilmesidir. Bu, ağ yöneticilerinin reverse proxy kullanıyorlarsa güvenlik duvarlarını güçlendirmeleri veya yeniden konumlandırmaları gerekebileceği anlamına gelir. Performansı ve güvenliği optimize etmek için sunucu adına hareket eder.


### Reverse proxy kullanımı

- Birden fazla web sunucusunda yük dengeleme
- Sunucu performansını iyileştirmek için içeriği önbelleğe alma
- Arka uç sunucularının internete doğrudan maruz kalmasının önlenmesi
- Sunucu verimliliğini artırmak için SSL/TLS boşaltma(SSL'de handshaking maliyeti artırır ama reverse proxy bu maliyeti azaltır)
- SSL iletişimlerini şifreleyin ve şifresini çözün
- DDoS saldırılarını azaltma ve güvenliği artırma




## Forward Proxy ve Reverse Proxy arasındaki farklar

| Özellik | Forward Proxy | Reverse Proxy |
|---------|-------------|------------|
| Amaç | Müşteri adına erişimi kontrol etmek ve gizliliği artırmak için hareket eder. | Performansı optimize etmek ve güvenliği artırmak için sunucu adına hareket eder. |
| Konum | Müşteri ile internet arasında yer alır. | İnternet ile sunucu arasında bulunur. |
| İstemci Görünürlüğü | İstemci proxy'nin farkındadır ve onu yapılandırması gerekir. | Müşteri genellikle proxy'nin varlığından habersizdir. |
| Yapılandırma | İstemcinin proxy'yi kullanabilmesi için cihazını yapılandırması gerekir. | Sunucu ters proxy kullanacak şekilde yapılandırılmıştır. |
| Kullanım Alanları | İçerik filtrelerini aşma, erişimi kontrol etme, gizliliği artırma. | Yük dengeleme, önbellekleme, DDoS koruması, SSL boşaltma. |
| İstek Yönlendirme | İstemciden internete gelen istekleri yakalar ve iletir. | İnternetten gelen istekleri yakalar ve bunları ilgili sunucuya iletir. |
| Önbellekleme | Yanıt sürelerini iyileştirmek için istemci tarafındaki içerikleri önbelleğe alabilir. | Yükü azaltmak ve içerik dağıtımını hızlandırmak için sunucu yanıtlarını önbelleğe alabilir. |
| SSL/TLS | Genellikle SSL/TLS şifrelemesini işlemez. | Sunucu için şifreleme/şifre çözme görevlerini kolaylaştırarak SSL/TLS boşaltma işlemini gerçekleştirebilir. |

---


## Load Balancer (Yük Dengeleyici) - Reverse Proxy'nin Bir Fonksiyonu

Gelen ağ trafiğini birden fazla backend sunucusuna akıllıca dağıtan bir sistem bileşenidir. Aslında bir reverse proxy'nin sahip olabileceği en temel ve kritik işlevlerden biridir.



### Amacı:

- Performans ve Ölçeklenebilirlik: Tek bir sunucunun kaldıramayacağı yükü, birden fazla sunucuya paylaştırarak uygulamanın hızlı ve erişilebilir kalmasını sağlar.

- Yedeklilik ve Hata Toleransı: Sunuculardan biri çökerse, trafiği sağlıklı olan diğer sunuculara yönlendirerek uygulamanın kesintisiz çalışmasını sağlar.



Yük dengeleme, günümüzün çok uygulamalı, çok cihazlı iş akışları tarafından oluşturulan çok sayıda istekle başa çıkması için en ölçeklenebilir yoldur. Günümüzün dijital işletmelerindeki birçok uygulamaya, dosyaya ve masaüstüne sorunsuz erişim sağlayan sistemlerle birlikte yük dengeleme, çalışanların daha tutarlı ve güvenilir bir son kullanıcı deneyimine sahip olmasına yardımcı olur. 




Sunucular arasında hareket eden trafiği yönetmenin yanı sıra, bir global sunucu yük dengeleyici (GSLB) kullanarak çeşitli konumlardaki birden çok veri merkezini de yönetebilirsiniz.





--- 


##  API Gateway (API Ağ Geçidi) - Özelleşmiş Bir Reverse Proxy

API Gateway, istemciler (mobil uygulama, web app, IoT cihazları vb.) ile arka uç servisleri (microservice’ler) arasında tek giriş noktası olarak çalışan bir katmandır. API ağ geçidi, güvenlik politikalarını uygularken API trafiğini yöneterek istekleri ve yanıtları kontrol eder. Bu, geliştiricilerin kullanıcı kimlik doğrulaması ve hız sınırlama gibi görevler de dahil olmak üzere karmaşık API ağlarıyla uğraşmak yerine tek tek hizmetler oluşturmaya odaklanmalarına yardımcı olan merkezi bir kontrol noktası sağlayarak API yönetimini basitleştirir. Reverse proxy'nin mikroservis dünyası için özelleşmiş, çok daha "akıllı" halidir.


### API gateway üzerinde yürütebileceğimiz operasyonlar

<img width="874" height="575" alt="image" src="https://github.com/user-attachments/assets/b078fbd9-4f8b-416d-8ad8-d92abdcdd784" />


### Örnek API Gateway’ler:
- Kong, NGINX, AWS API Gateway, Traefik, Istio (Service Mesh içinde)

---

## Traefik (veya Nginx, HAProxy) - Bir Araç / Yazılım
**Tanım:** Traefik, yukarıda bahsettiğimiz kavramları (reverse proxy, load balancing) hayata geçiren somut bir yazılımdır(çok güçlü bir şekilde). Modern, dinamik ve konteyner dostu (Docker, Kubernetes) bir reverse proxy ve load balancer'dır. Ek eklentileri ve yetenekleriyle (kimlik doğrulama, rate limiting) basit bir API Gateway olarak da kullanılabilir. Ancak, AWS API Gateway, Kong veya Tyk gibi tam teşekküllü API Gateway'lerin tüm gelişmiş özelliklerini içermeyebilir. Kısaca, Reverse Proxy ve Load Balancer olarak çalışan, özellikle konteyner ortamları için tasarlanmış popüler bir yazılım aracıdır diyebiliriz.

- **Avantajı:** Docker, Kubernetes, Consul, Etcd gibi servis keşif (service discovery) araçları ile otomatik entegre olur. Yani yeni bir servis eklediğinizde manuel konfigürasyon yapmanıza gerek kalmaz, Traefik kendisi keşfeder. (Geleneksel araçlar (Nginx) yapılandırma dosyası değişikliği ve yeniden başlatma gerektirir)
- **Let's Encrypt Desteği:** Otomatik ve ücretsiz SSL sertifikası alımını ve yenilenmesini destekler.
- **Dashboard:** Kullanışlı bir web arayüzü sunar.




 ### Traefik Özellikleri

- Dynamic Configuration → Servisleri otomatik keşfeder

- Reverse Proxy → İstekleri doğru backend servisine yönlendirir

- Load Balancing → Servisler arasında yük dağıtır

- SSL/TLS (Let's Encrypt) → Otomatik sertifika yönetimi

- Observability → Monitoring (Prometheus, Grafana entegrasyonu)

- Middlewares → Rate limiting, authentication, redirect, retry gibi ekstra işlemler


### Load Balancing & Filtering
Uygulamamıza gelen isteklerin performans sorunu yaratmaması ve yüksek erişilebilirlik değerleri için load balancing yani yük dağılımı yapmak isteyebiliriz. API gateway load balancing yapmak için de uygun bir noktadır. Servislerimizin önünde konumlanan API gateway, gelen istekleri alır ve bu istekleri belirlenen yönlendirme kurallarına göre hedef servislere yönlendirir. Ayrıca servis erişimleri için belirli IP adreslerine izin vermek veya bazı IP adreslerini kara listeye almak isteyebiliriz. API gateway bu filtrelemeyi yapmak için IP tabanlı erişim kontrolü sağlar. Bu sayede, belirli bir IP adresinden gelen istekleri kabul etmek veya reddetmek için API gateway üzerinde gerekli konfigürasyonlar yapılabilir. Bu filtreleme mekanizması, güvenlik politikalarını uygulamak ve istenmeyen erişimleri engellemek için önemli bir araçtır.








## Genel Bakış: Bir Benzetme ile Açıklama

**Bir "Restoran Zinciri" benzetmesi yapalım:**

- Müşteri: Siz (istemci / client)

- Yemek Siparişi: HTTP/HTTPS isteği (request)

- Restoranın Kapısındaki Görevli (Kapıcı): Reverse Proxy

- Restoranın Garsonlarının Şefi / Menü Sorumlusu: API Gateway

- Garsonları Farklı Masalara Yönlendiren Hostes: Load Balancer (Yük Dengeleyici)

- Restoranın Mutfağı: Backend servisleriniz (web sunucuları, API'lar, mikroservisler)

- Traefik: Bu restoran için özelleşmiş, hem kapıcılık hem hosteslik hem de garson şefliği yapabilen çok yetenekli ve modern bir eleman.



### KAYNAKÇA
https://www.geeksforgeeks.org/system-design/difference-between-forward-proxy-and-reverse-proxy/
https://www.fortinet.com/resources/cyberglossary/proxy-server
https://www.youtube.com/watch?v=4NB0NDtOwIQ
https://blog.bytebytego.com/p/ep25-proxy-vs-reverse-proxy
https://konghq.com/blog/learning-center/what-is-an-api-gateway
https://bulutistan.com/blog/load-balancer-yuk-dengeleyici-nedir/
