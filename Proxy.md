# TUG-Proxy-Reverse/Forward Proxy-Load Balancer-API Gateway-Traefik, CDN(Content Delivery Network), Nginx, Service Discovery(Consul)

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


### Proxy Ayarları Nedir? Nasıl Yapılır?
Proxy ayarları, internete bağlanırken kullanacağınız proxy sunucusunun detaylarını belirlemeye yarar. Ayarlar, farklı işletim sistemlerine ve tarayıcılara göre değişiklik gösterebilir. İşte temel adımlar:

Windows İşletim Sistemi için:

- Kontrol Paneli'ni açın.
- Ağ ve İnternet seçeneğine gidin.
- İnternet Seçenekleri'ni tıklayın.
- Bir pencere açılacak, burada Bağlantılar sekmesine gidin.
- Yerel Ağ Ayarları'nı tıklayın.
- Proxy sunucusu bölümünde gerekli IP adresini ve port numarasını girin.
- Tamam'ı tıklayarak ayarları kaydedin.


### Proxy ile VPN Arasındaki Farklar Nelerdir?
Proxy ve VPN (Sanal Özel Ağ), internet trafiğini yönlendiren ve kullanıcıların anonim bir şekilde internette gezinmelerini sağlayan servislerdir. Ancak, bu iki servis arasında önemli farklar vardır:

**Güvenlik:**

- VPN: Tüm internet trafiğinizi şifreler ve güvenli bir tünel içinden geçirir. Bu, kişisel verilerinizin korunması için daha etkilidir.
- Proxy: Genellikle yalnızca belirli bir uygulama veya web sitesi için trafiği yönlendirir ve şifreleme sunmayabilir.


**Performans:**

- VPN: Genellikle trafiği şifrelediği için, hızda bir miktar düşüş yaşanabilir.
- Proxy: Şifreleme olmadığı için genellikle daha hızlıdır fakat güvenlik açısından daha zayıftır.


**Uygulama ve Protokol Desteği:**

- VPN: Tüm cihazlar ve uygulamalar için sistem geneli bir çözümdür.
- Proxy: Genellikle belirli uygulamalar veya tarayıcılar için geçerlidir.


**Anonimlik:**

- VPN: IP adresinizi değiştirir ve tüm çevrimiçi aktivitenizi anonim hale getirir.
- Proxy: Yalnızca belirli bir hizmet veya web sitesi için IP adresinizi saklar.


**Maliyet:**

- VPN: Genellikle ücretli planlar sunar ve daha kapsamlı özellikler sağlar.
- Proxy: Hem ücretsiz hem de ücretli seçenekler mevcuttur fakat ücretsiz olanlar genellikle reklamlarla desteklenir ve daha az özellik sunar.


**Kullanım Alanları:**

- VPN: Genel internet kullanımı, güvenlik, anonimlik, coğrafi kısıtlamaların aşılması gibi birçok alanda kullanılır.
- Proxy: Genellikle basit IP maskleme, hafif internet gezinme ve coğrafi kısıtlamaları aşmak için kullanılır.


Özellikle e-ticaret firmaları için VPN, müşteri verilerini koruma ve coğrafi kısıtlamaları aşma gibi daha kapsamlı ihtiyaçlara hizmet ederken, proxy daha hızlı ve belirli görevler için uygun olabilir.




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

Forward proxy istemci adına hareket ederken, reverse proxy sunucu adına hareket eder. İstemcilerin kaynak sunucuyla doğrudan iletişim kurmasını engelleyerek sunucuları korumak ve yönetmek için kullanılır. Reverse proxy'ler, gelen çok sayıda isteğin yükünü dengelemesi gereken popüler web siteleri için güçlü bir seçenektir. Gelen istekleri yöneten başka bir web sunucusu gibi davrandıkları için bir kuruluşun bant genişliği yükünü azaltmasına yardımcı olabilirler. Olumsuz tarafı ise, bir saldırganın sızması durumunda reverse proxy'lerin HTTP sunucu mimarisini açığa çıkarabilmesidir. Bu, ağ yöneticilerinin reverse proxy kullanıyorlarsa güvenlik duvarlarını güçlendirmeleri veya yeniden konumlandırmaları gerekebileceği anlamına gelir. Performansı ve güvenliği optimize etmek için sunucu adına hareket eder. (Nginx, HAProxy, Envoy..)


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




Resim kaynakçası: https://ucemucar.medium.com/api-gateway-nedir-neden-kullan%C4%B1l%C4%B1r-fadcb45d11fb

### Load Balancing & Filtering
Uygulamamıza gelen isteklerin performans sorunu yaratmaması ve yüksek erişilebilirlik değerleri için load balancing yani yük dağılımı yapmak isteyebiliriz. API gateway load balancing yapmak için de uygun bir noktadır. Servislerimizin önünde konumlanan API gateway, gelen istekleri alır ve bu istekleri belirlenen yönlendirme kurallarına göre hedef servislere yönlendirir. Ayrıca servis erişimleri için belirli IP adreslerine izin vermek veya bazı IP adreslerini kara listeye almak isteyebiliriz. API gateway bu filtrelemeyi yapmak için IP tabanlı erişim kontrolü sağlar. Bu sayede, belirli bir IP adresinden gelen istekleri kabul etmek veya reddetmek için API gateway üzerinde gerekli konfigürasyonlar yapılabilir. Bu filtreleme mekanizması, güvenlik politikalarını uygulamak ve istenmeyen erişimleri engellemek için önemli bir araçtır.




### Örnek API Gateway’ler:
- Kong, NGINX, AWS API Gateway, Traefik, Istio (Service Mesh içinde)
---

- Kong – Açık kaynak + ücretli (Enterprise sürümü mevcut)

- NGINX – Açık kaynak (NGINX Open Source) + ücretli (NGINX Plus)

- AWS API Gateway – Tamamen ücretli, AWS hizmeti

- Traefik – Açık kaynak + ücretli (Traefik Enterprise)

- Istio (Service Mesh içinde) – Açık kayna


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







## Genel Bakış: Bir Benzetme ile Açıklama

**Bir "Restoran Zinciri" benzetmesi yapalım:**

- Müşteri: Siz (istemci / client)

- Yemek Siparişi: HTTP/HTTPS isteği (request)

- Restoranın Kapısındaki Görevli (Kapıcı): Reverse Proxy

- Restoranın Garsonlarının Şefi / Menü Sorumlusu: API Gateway

- Garsonları Farklı Masalara Yönlendiren Hostes: Load Balancer (Yük Dengeleyici)

- Restoranın Mutfağı: Backend servisleriniz (web sunucuları, API'lar, mikroservisler)

- Traefik: Bu restoran için özelleşmiş, hem kapıcılık hem hosteslik hem de garson şefliği yapabilen çok yetenekli ve modern bir eleman.

---

## CDN(Content Delivery Network)
İçerik dağıtım ağı (CDN), içerikleri son kullanıcılara yakın bir yerde önbelleğe alan, coğrafi olarak dağıtılmış bir sunucu grubudur. CDN, HTML sayfaları, JavaScript dosyaları, stil sayfaları, resimler ve videolar dahil olmak üzere İnternet içeriğinin yüklenmesi için gereken varlıkların hızlı bir şekilde aktarılmasını sağlar. CDN servislerinin popülaritesi giderek artıyor ve bugün web trafiğinin büyük çoğunluğu, Facebook, Netflix ve Amazon gibi büyük sitelerden gelen trafik de dahil olmak üzere, CDN'ler aracılığıyla sağlanıyor. CDN sunucularına genellikle "edge servers"(uç sunucu) denir.

<img width="890" height="648" alt="image" src="https://github.com/user-attachments/assets/6adc18af-236a-4fc4-b56e-968f2e23904e" />





Resim kaynakçası -> https://www.researchgate.net/figure/High-level-understanding-of-Content-Delivery-Networks_fig2_321791733

- Doğru şekilde yapılandırılmış bir CDN, web sitelerini Dağıtılmış Hizmet Reddi (DDOS) saldırıları gibi bazı yaygın kötü amaçlı saldırılara karşı korumaya da yardımcı olabilir. 
- Dağıtık yapıları sayesinde bir CDN, birçok kaynak sunucudan daha fazla trafiği yönetebilir ve donanım arızalarına daha iyi dayanabilir.


### CDN'ler nasıl çalışır?

Örneğin, web sitenizin Birleşik Krallık'taki (BK) bir kaynak sunucuda bulunduğunu varsayalım. Amerika Birleşik Devletleri'nden (ABD) biri sitenize erişirse, CDN bu kullanıcıya, web sayfası için Birleşik Krallık'taki kaynak sunucunuz yerine, kullanıcıya daha yakın olan ABD'deki bir uç sunucudan hizmet verir. Bu uç sunucu, kullanıcılar ve internet arasında bir ağ geçidi görevi gören bir tür proxy sunucusudur (bazen önbellek veya önbellekleme sunucusu olarak da adlandırılır).



### Bir CDN iki tür içerik sunabilir: statik ve dinamik.


- **Statik içerik** , bir web sitesinde sabit kalan çevrimiçi içeriktir . Siteyi ziyaret eden tüm kullanıcılar için aynı kalır. Web sitesi logoları ve HTML ile yazılmış marka bilgileri gibi içerikler statik içerik örnekleridir.
- **Dinamik içerik** , kullanıcı davranışına, konuma veya diğer faktörlere bağlı olarak değişen çevrimiçi içeriktir. Örneğin, sosyal medya akışları (Instagram, Facebook ve daha fazlası), yayın platformları (Netflix, Hulu ve diğerleri) ve e-ticaret siteleri (Amazon gibi), her kullanıcıya özel ve kişiselleştirilmiş, medya açısından zengin dinamik içerikler sunar.
 

---

- **Amaç**: Statik içerikleri (resim, CSS, JS, video vb.) kullanıcılara daha hızlı ulaştırmak.
- **Nasıl çalışır**: İçerik, dünya genelindeki cache sunucularına (edge servers) kopyalanır. Kullanıcı isteği, en yakın edge sunucuya yönlendirilir. Böylece origin sunucuya giden trafik azalır ve gecikme (latency) düşer.
- **Avantajları**:Daha hızlı yükleme. Origin sunucu yükünün azalması. DDoS ve trafik patlamalarına karşı koruma. Global erişimde tutarlılık. Daha iyi arama motoru optimizasyonu (SEO) sıralamaları. 


---
## CDN bileşenleri ve ilgili teknolojiler


### Alan adı sistemi (DNS) sunucusu
DNS , kullanıcıların IP adresleri yerine alan adları ve URL'ler kullanarak web sitelerine erişmelerini sağlayan standart internet protokolünün bir parçasıdır. DNS, internetin rehberidir; web tarayıcıları aracılığıyla belirli web sitelerini arama sürecini basitleştirir. İçerik dağıtım ağları (CDN'ler), kaynak ve uç sunucular için IP adreslerini takip etmek ve sağlamak ve dinamik istek yönlendirmesi gerçekleştirmek için DNS kullanır.

### Varlık noktası (PoP)
Varlık noktası, sunucuları ve yönlendiricileri dünya çapında farklı bölgelerde depolayan fiziksel bir konumdur. Optimum bağlantı ve performans sağlamak için stratejik olarak yerleştirilirler ve genellikle yüksek kullanıcı yoğunluğuna sahip veya birden fazla ağ yolunun kesiştiği alanlara yerleştirilirler.

### İnternet değişim noktası (IXP)
IXP, internet servis sağlayıcılarının ve CDN'lerin bağlandığı fiziksel bir konumdur.

### Uygulama dağıtım denetleyicisi (ADC)
ADC, genellikle bir uygulama dağıtım ağının (ADN) parçası olarak, uygulamaların internet üzerinden dağıtımını optimize etmek için kullanılan bir ağ cihazıdır. Büyük ölçekli, karmaşık veya dağıtılmış bir içerik dağıtım ağı (CDN) işleten bir kuruluş, hızı daha da artırmak ve performansı optimize etmek için ADC'leri de kullanabilir .


---


## Nginx
Nginx en kısa şekli ile açık kaynak olarak tasarlanmış bir ‘web server’ yazılımıdır. Odaklandığı noktalar ise en yüksek performans ve stabil davranışı, en basit ve küçük boyutlu bir şekilde kullanıcılara sunmasıdır. Yani Nginx , düşük bellek kullanımı ve yüksek eşzamanlılık sunmak üzere tasarlanmıştır. Her web isteği için yeni süreçler oluşturmak yerine, isteklerin tek bir iş parçacığında işlendiği eşzamansız, olay odaklı bir yaklaşım kullanır. Nginx Unix tabanlı işletim sistemlerinde çalışmaktadır, Windows makinelerde kısıtlı desteği bulunmaktadır.



Nginx ile tek bir ana işlem birden fazla çalışan işlemi kontrol edebilir. Ana işlem çalışan işlemleri yönetirken, çalışanlar asıl işlemi gerçekleştirir. Nginx eşzamansız olduğundan, her istek çalışan tarafından diğer istekleri engellemeden eş zamanlı olarak yürütülebilir.




- **Amaç**: Web sunucusu, reverse proxy, load balancer veya cache olarak kullanılabilir.
- **Özellikleri**: **Reverse proxy**: Trafiği backend sunuculara yönlendirir, SSL offloading yapabilir, caching sağlar. **Load balancing**: Trafiği birden fazla backend sunucuya dağıtır (round-robin, least connections gibi). **Statik içerik sunma**: Çok hızlıdır ve düşük kaynak kullanır. **Caching ve rate limiting**: Performans ve güvenlik iyileştirmeleri sağlar.

<img width="936" height="614" alt="image" src="https://github.com/user-attachments/assets/d249e239-815e-4427-b054-640f96271406" />



Resim kaynakçası -> https://www.freecodecamp.org/news/an-introduction-to-nginx-for-developers-62179b6a458f/



- Alternatifi ise Apache'dir. Apache, bir diğer popüler açık kaynaklı web sunucusudur. Ham veriler açısından, Apache mevcut en popüler web sunucusudur. Fakat Apache genel olarak en popüler seçenek olsa da, Nginx aslında yüksek trafikli web siteleri arasında en popüler web sunucusudur. Apache'nin kullanımı, bir sitenin trafiği arttıkça ters yönde hareket eder.




### Kurulum için:

```bash
sudo apt-get updatesudo apt-get install nginx
```


**nginx.conf**: Çekirdek ayarlar burada; üst düzey bağlamlar events ve http. HTTP bağlamı altında iç içe sunucu ve konum blokları yer alır. Bu dosya yapılandırılarak yandaki dosya yollarına yerleştirilir:  /usr/local/nginx/conf, /etc/nginx, /usr/local/etc/nginx 


### Basit bir configuration dosyası:

```bash
server {
  listen 80;
  include etc/nginx/mime.types;
  location /{
    root /usr/share/nginx/html/;
  }
}
```

- **listen** → Server’in hangi port üzerinden yayın yapacağını belirten config. Bizim durumumuzda container içerisinde hangi port üzerinden ulaşılacağını belirtiyor.

- **include** → Web servisimizin istemcilere sunabileceği tüm tipleri belirttiğimiz mime.types dosyasını dahil ediyoruz. Bu dosya hali hazırda kullandığımız Nginx imajında belirtilen dizinde mevcut olduğunu için kendimiz oluşturmadık. Örnek bir içeriğe buradan ulaşabilirsiniz. Yada benzer formatta kendiniz oluşturabilirsiniz.

- **location** → Server çalıştığında hangi konumu referans alacağını burada belirtiyoruz. Burada location ibaresinden sonra bir endpoint belirleyebiliriz.

- **root** → Web sayfasının kaynak kodlarının bulunduğu dosya yolunu belirtiyoruz. Nginx container içerisinde bu konum /usr/share/nginx/html olarak belirlenmiş. Fakat biz farklı bir konumu da belirtip kaynak dosyalarını oraya kopyalayabiliriz.



### Önemli ayarlar:

- worker_processes: CPU çekirdek sayısı kadar.

- worker_connections: Her işlem için eşzamanlı bağlantı sayısı.

- access_log & error_log: Kayıt dosyaları.

- gzip: Yanıt sıkıştırması, performans artırır.

### Sites dizinleri:

- sites-available: Tüm site yapılandırmaları.

- sites-enabled: Aktif siteler; sites-available dosyaları buraya sembolik bağlanır.


### Bloklar:

- Server bloğu: Belirli sanal sunucular için; birden fazla olabilir.
- Location bloğu: URI’ye göre istek yönlendirmesi (try_files, proxy_pass, rewrite).
- Upstream bloğu: Proxy veya yük dengeleme sunucularını tanımlar.


### NGINX'i başlatın

```bash
sudo service nginx start
```

### Herhangi bir değişiklik yaptığımızda, aşağıdaki komutu kullanarak (kesintisiz olarak) onu yeniden yüklememiz yeterli olacaktır.


```bash
service nginx reload
```


### NGINX'in durumunu kontrol etme


```bash
service nginx status
```


Kullanıma hazır pek çok özelliğiyle NGINX, uygulamanızı sunmanın veya diğer web sunucularınız için bir HTTP proxy'si veya yük dengeleyici olarak kullanmanın harika bir yolu olabilir. NGINX'in çalışma ve istekleri işleme şeklini anlamak, uygulamalarınızın yükünü ölçeklendirmenize ve dengelemenize büyük katkı sağlayacaktır.


## Nginx Agent

NGINX Açık Kaynak veya NGINX Plus örneğiniz için bir yardımcı programdır. Şunları sağlar:

- NGINX yapılandırmalarının uzaktan yönetimi
- Gerçek zamanlı NGINX performans ve işletim sistemi ölçümlerinin toplanması ve raporlanması
- NGINX olaylarının bildirimleri

<img width="885" height="325" alt="image" src="https://github.com/user-attachments/assets/e2740baf-c1e4-4453-931b-476647455955" />

NGINX Agent tarafından bildirilen metrikleri gösteren Grafana panosu


- Resim kaynakçası -> https://docs.nginx.com/nginx-agent/overview/



### Nasıl çalışır?

NGINX Agent, NGINX çalıştıran bir sistemde yardımcı bir işlem olarak çalışır. Yapılandırma yönetimi ve NGINX işlemlerinden ve işletim sisteminden ölçüm toplama için gRPC ve REST arayüzleri sağlar. NGINX Agent, yaygın Linux araçlarını kullanarak NGINX ile uzaktan etkileşime olanak tanır ve büyük NGINX örnek koleksiyonlarını yönetebilen gelişmiş izleme ve kontrol sistemleri oluşturma olanağı sunar.


<img width="852" height="654" alt="image" src="https://github.com/user-attachments/assets/15f4c545-74bf-4dbc-a565-a507bf57eeee" />



---


## Service Discovery (Consul örneği)

Service Discovery’nin amacı, dinamik ve değişken ortamlarda microservice’lerin birbirlerini bulmasını ve iletişim kurmasını sağlamaktır. Mikroservisler sürekli olarak ölçeklenir, taşınır veya yeniden başlatılır; bu nedenle, servislerin sabit adresleri yoktur. Service Discovery, bu dinamikliği yönetmek için kullanılır.



<img width="774" height="779" alt="image" src="https://github.com/user-attachments/assets/4fee23fc-72f2-44d8-96b3-ee97ebe846ec" />



Resim kaynakçası -> https://gokhan-gokalp.com/microservice-mimarilerinde-consul-ile-service-discovery/


Yukarıdaki yapıya baktığımızda, auto scale olan ve dynamic olarak değişen instance’lara sahip bir yapıyı görüyoruz. Burada dikkat edersek IP adresleri de dynamic olarak assign edilmektedir. Bu gibi dynamic case’ler karşısında, client hangi IP adresine istek atacağını bilemeyecektir. Service discovery ise bu gibi durumları nasıl otomatik olarak handle edebilirize odaklanmaktadır.


Service discovery  temel olarak üç kavram üzerinde durmaktadır:

- Discovery: Service’lerin dynamic bir ortamda cluster içerisindeki diğer service’ler ile iletişim kurabilmeleri için, birbirlerinin IP ve port bilgilerini bulmaya ihtiyaçları vardır. Discovery ise bunu sağlamaktadır.
- Health check: Health check işlemi ile sadece up olan service’lerin sistemde kalmaları, down olan’ların ise dynamic bir şekilde sistem dışı kalmaları sağlanmaktadır.
- Load balancing: Hepimizin de bildiği gibi bir hizmete gelmiş olan request’in, bu hizmeti sağlayan diğer instance’lara da dynamic olarak dağıtılmasını sağlamaktır.



### Nerelerde ve Ne İçin Kullanılır?
Service Discovery, büyük ve karmaşık sistemlerde, özellikle de microservice mimarilerinde kullanılır. İşte bazı kullanım alanları:

- Dinamik Ölçekleme: Servisler dinamik olarak ölçeklendiğinde, yeni servis örnekleri otomatik olarak keşfedilir ve yük dengelemesi yapılır.
- Kapsayıcı Orkestrasyonu: Docker ve Kubernetes gibi ortamlar, servislerin otomatik olarak keşfedilmesi ve yönetilmesi için Service Discovery kullanır.
- Otomatik Yeniden Başlatma: Servisler yeniden başlatıldığında, yeni adresler Service Discovery mekanizmaları ile güncellenir.



Servis kayıt sistemleri, dinamik yönetim ve esneklik sağlayarak servis adreslerindeki değişikliklere hızlı uyum göstermeyi kolaylaştırır. Ayrıca merkezi yönetim sayesinde servislerin kontrolü basitleşir. Ancak bu yaklaşım, kurulum ve yönetimde karmaşıklık yaratabilir, merkezi yapının çökmesi durumunda tek nokta hatası riski taşır ve servis kaydediciye yapılan her isteğin ek performans yükü oluşturması dezavantajdır.

<img width="602" height="448" alt="image" src="https://github.com/user-attachments/assets/99f2a7f3-831d-40ed-b5ab-92f7b8a617da" />



Resim kaynakçası -> https://www.linkedin.com/pulse/service-discovery-nedir-ve-neden-%C3%B6nemlidir-burak-ka%C5%9F%C4%B1kc%C4%B1-yhuzf/


- **Amaç**: Mikroservis mimarisinde servislerin birbirini bulmasını sağlamak.
- **Problem**: Backend servisleri dinamik IP’ler ve portlar ile çalışır; statik IP ile ulaşmak zor.
- **Consul nasıl çözer**:Servisler Consul’a kaydolur (service registration).Diğer servisler, Consul’dan servis IP/port bilgisini alır (service discovery).Health check ile servislerin sağlıklı olup olmadığı sürekli kontrol edilir.
- **Avantajları**: Mikroservisler arası esnek ve dinamik iletişim. Yüksek erişilebilirlik ve failover yönetimi. Merkezi yönetim ve monitoring kolaylığı.


2 tür service discovery patterni bulunmakta.Client-Side Service Discovery ve Server-Side Service Discovery.


### Client-Side Service Discovery

Bu yapıda client service registry ile iletişime geçer ve istediği domainin adresini sorar.Service registry üzerinde kayıtlı olan yani ulaşılabilir durumdaki microservice instance’larının ip adreslerini verir.Daha sonra client bir load-balancing algoritmasına göre bu microservicelerden en uygun olanı seçer ve microservice ile iletişim kurar.Gördüğünüz gibi burada client,ip adresini elde ederek microservice ile kendisi iletişim kurmaktadır.


<img width="692" height="655" alt="image" src="https://github.com/user-attachments/assets/cb03cc2f-b716-4bd2-8ada-f43728fc7084" />

Resim kaynakçası -> https://medium.com/i%CC%87yi-programlama/microservice-mimarilerinde-service-discovery-7a6ebceb1b2a


### Server-Side Service Discovery

Burada ise client bir Load Balancer(Yük Dengeleyici) ile iletişim kurar.İsteğini buraya iletir.Load Balancer ise Service Registry ile konuşarak avaliable durumdaki instance’ların listesini alır.Daha sonra da arasından kendi algoritmasına göre en uygun gördüğü instance’a client’tan aldığı isteği yönlendirir.



<img width="686" height="441" alt="image" src="https://github.com/user-attachments/assets/03c21d9d-495e-4e64-92c4-c315c3da97b8" />



Resim kaynakçası -> https://medium.com/i%CC%87yi-programlama/microservice-mimarilerinde-service-discovery-7a6ebceb1b2a


İkisinin arasındaki fark Client-Side Service Discovery yapısında client,instance ile kendisi iletişim kurmaktadır.Çünkü o instance’ın ip adres bilgisini service registry’e sorarak öğrenmektedir.Server-Side Service Discovery örneğinde ise request load balancer aracılığı ile instancelara iletilmektedir.


### Service Discovery Teknolojileri

- **Eureka (Spring Cloud Netflix**) : Merkezi servis kaydı ve keşfi sağlar. Özellikle Spring Boot uygulamaları ile uyumlu çalışır.
- **Consul** : Hizmet kaydı ve keşfi, konfigürasyon yönetimi ve sağlık kontrolleri sağlar.
- **Zookeeper** : Koordinasyon, servis keşfi ve senkronizasyon sağlar.


## Consul


Consul, kapsamlı bir service discovery aracıdır. Öncelikle consul’ün mimarisine biraz değinecek olursak consistency için server node’larında Raft consensus‘u kullanmaktadır. Raft consensus, Paxos temelli bir consensus algoritmasıdır.










### NOT: Nginx + CDN + Consul kombinasyonu, modern web uygulamalarında yük dağıtımı, güvenlik, performans ve servis yönetimini birlikte sağlar.



### KAYNAKÇA
https://www.geeksforgeeks.org/system-design/difference-between-forward-proxy-and-reverse-proxy/
https://www.fortinet.com/resources/cyberglossary/proxy-server
https://www.youtube.com/watch?v=4NB0NDtOwIQ
https://blog.bytebytego.com/p/ep25-proxy-vs-reverse-proxy
https://konghq.com/blog/learning-center/what-is-an-api-gateway
https://bulutistan.com/blog/load-balancer-yuk-dengeleyici-nedir/
https://www.cloudflare.com/learning/cdn/what-is-a-cdn/
https://www.ibm.com/think/topics/content-delivery-networks
https://medium.com/@aedemirsen/nginx-nedir-nginx-ile-bir-web-sayfas%C4%B1-nas%C4%B1l-sunulur-670eefadd047
https://kinsta.com/blog/what-is-nginx/
https://docs.nginx.com/nginx-agent/overview/ 
https://medium.com/i%CC%87yi-programlama/microservice-mimarilerinde-service-discovery-7a6ebceb1b2a
https://gokhan-gokalp.com/microservice-mimarilerinde-consul-ile-service-discovery/
