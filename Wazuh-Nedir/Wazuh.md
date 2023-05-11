![](vertopal_50440ba390d044fbab36323b23391591/media/image1.jpeg)
**Wazuh Nedir ve Ne İçin
Kullanılır**
Wazuh, güvenlik tehditlerini tespit etmek, olayları izlemek ve güvenlik
olaylarını analiz etmek için kullanılan bir açık kaynaklı güvenlik
bütünleşik bir çözümdür. Wazuh, siber güvenlik operasyonlarını ve olay
yönetimini geliştirmek amacıyla tasarlanmıştır. Bu yazımızda Wazuh\'un
ne olduğu, nasıl çalıştığı, hangi amaçlarla kullanıldığı ve nasıl
kurulduğunu ayrıntılı bir şekilde kodlarla beraber ele alınacağız.
İsterseniz lafı daha fazla uzatmadan başlayalım. 

**Wazuh Bir Güvenlik Platformudur**

Wazuh, ölçeklenebilir ve çoklu platform desteği sunan bir güvenlik
platformudur. İlk olarak, Wazuh\'un özelliklerini ve avantajlarını
anlamak için platformun yapılandırma ve bileşenlerine bir göz atalım.
Wazuh, ajanlar, sunucular ve kullanıcı arabiriminden oluşur. Ajanlar,
izlenen sistemlere kurulur ve olayları toplar, sistem güvenlik durumunu
kontrol eder ve güvenlik tehditlerini algılamak için gerekli bilgileri
sağlar. Sunucu, ajanlardan gelen olayları alır, analiz eder ve merkezi
bir konumda izlemeyi sağlar. Kullanıcı arabirimi ise güvenlik olaylarını
görüntülemek, raporlamak ve yönetmek için kullanılır. 

**Wazuh Kullanım Amacı Nedir**

Wazuh\'un kullanım amacı, ağ ortamında oluşabilecek güvenlik
tehditlerini tespit etmek ve müdahale etmektir. Wazuh, saldırı tespiti
ve olay yönetimi yetenekleriyle bilinen bir sistemdir. Sistem
günlüklerini izler, ağ trafiğini analiz eder ve zararlı yazılımların
algılanması için imza tabanlı ve davranış tabanlı analiz yöntemlerini
kullanır. Ayrıca, sisteme yapılan saldırı girişimlerini izler, güvenlik
açıklarını tespit eder ve saldırılar için erken uyarı sistemleri sunar.
Wazuh, siber güvenlik uzmanlarına, güvenlik olaylarını hızla tespit
etme, analiz etme ve müdahale etme imkanı sağlar. 

**Wazuh Kullanımı Nasıldır**

Wazuh\'un kurulumu da oldukça önemlidir. Kurulum süreci, ajanların hedef
sistemlere kurulumunu, sunucunun yapılandırılmasını ve kullanıcı
arabirimine erişimi içerir. Wazuh, Linux, Windows, macOS ve Docker gibi
farklı işletim sistemlerinde çalışabilen bir platformdur. Kurulum
sürecinde, her bir bileşenin doğru yapılandırılması, güncel sürümlerin
kullanılması ve gereksinimlerin karşılanması önemlidir.
Kilincfurkan.com\'daki kaynağa başvurarak adım adım kurulum
talimatlarına ulaşabilirsiniz.

Wazuh\'un güçlü yanlarından bir diğeri, esnek yapılandırma
seçenekleridir. Wazuh, kullanıcıların kendi güvenlik politikalarını ve
izleme gereksinimlerini belirlemelerine olanak tanır. Böylece, farklı
organizasyonların farklı ihtiyaçlarına uygun şekilde özelleştirilebilir.

Wazuh\'un diğer önemli bir özelliği, gerçek zamanlı tepki
yetenekleridir. Tehditlerin tespit edildiği anda otomatik tepkiler
verebilir ve hızlı müdahale sağlayabilir. Örneğin, zararlı bir dosya
tespit edildiğinde, otomatik olarak dosyayı izole edebilir veya
saldırgan IP adresini engelleyebilir.

Wazuh ayrıca kapsamlı bir güvenlik olay yönetimi ve raporlama
yetenekleri sunar. Güvenlik olaylarını merkezi bir konumda toplar,
analiz eder ve kullanıcı arabiriminde görsel olarak sunar. Kullanıcılar,
güvenlik durumunu izleyebilir, olayları araştırabilir, trendleri analiz
edebilir ve gerektiğinde raporlar oluşturabilir.

Wazuh, açık kaynaklı bir proje olması nedeniyle sürekli geliştirilmekte
ve güncellenmektedir. Kullanıcılar ve geliştiriciler, yeni özellikler
ekleyebilir, hataları düzeltebilir ve topluluk tarafından paylaşılan
güvenlik imzalarını kullanabilirler. Bu, Wazuh\'un güncel kalmasını ve
güvenlik tehditlerine karşı etkin bir şekilde korunmayı sağlar.

**Wazuh ajanının bir sunucuya kaydolması**

Wazuh ajanları, izlenen sistemlere kurulur ve güvenlik olaylarını
toplamak, sistem güvenliğini kontrol etmek ve tehditleri algılamak için
gerekli bilgileri sunmak için kullanılır. Wazuh ajanını bir sunucuya
kaydettikten sonra, ajanlar günlük olayları ve diğer güvenlik verilerini
sunucuya iletecektir. Bu kaydolma işlemi, ajanın Wazuh sunucusuyla
iletişim kurabilmesini sağlar ve merkezi bir güvenlik izleme ve yönetim
noktası sağlar. 

**Bir güvenlik kuralı oluşturma**

Wazuh, güvenlik kuralları aracılığıyla belirli güvenlik olaylarını
tespit eder ve buna göre bir tepki verir. Güvenlik kuralları, XML
formatında tanımlanır ve Wazuh\'un belirli bir tehdidi veya güvenlik
durumunu algıladığında ne yapması gerektiğini belirtir. Örneğin, bir
rootkit veya truva atak tespit edildiğinde tetiklenecek bir güvenlik
kuralı oluşturabilirsiniz. Kural, e-posta, syslog veya Slack gibi farklı
bildirim yöntemlerini kullanarak bir uyarı gönderebilir. 

**Olayları izleme**

Wazuh, sistem günlüklerini izler ve güvenlik olaylarını gerçek zamanlı
olarak takip eder. Wazuh ajanları, sistemindeki güvenlik olaylarını
toplayarak Wazuh sunucusuna iletir. Bu olaylar daha sonra Wazuh
kullanıcı arabiriminde görüntülenir. Örneğin,
\"/var/ossec/bin/agent_control -l\" komutunu kullanarak ajanlar
tarafından toplanan günlük olayları görüntüleyebilirsiniz. Bu sayede
güvenlik olaylarını anında izleyebilir ve hızlı bir şekilde müdahale
edebilirsiniz. 

**Wazuh API\'sini kullanarak güvenlik olaylarını sorgulama**

Wazuh, RESTful API\'ler aracılığıyla programatik olarak erişilebilir. Bu
API\'ler, kullanıcıların Wazuh sistemine sorgular göndererek güvenlik
olaylarını veya ajan bilgilerini almasını sağlar. Örneğin, Python dilini
kullanarak Wazuh API\'sini kullanabilir ve ajan bilgilerini
alabilirsiniz. Bu bilgileri kullanarak ajanların durumunu, bağlantı
durumunu veya diğer ajan özelliklerini görüntüleyebilirsiniz. Bu sayede
otomatikleştirilmiş işlemler gerçekleştirebilir veya özel güvenlik
raporları oluşturabilirsiniz. 

**Wazuh kullanıcı arabirimine erişim**

Wazuh, kullanıcı arabirimi aracılığıyla güvenlik olaylarını
görselleştirmenizi, sistem durumunu izlemenizi ve ajanların
yapılandırmasını yönetmenizi sağlar. Kullanıcı arabirimi, web tabanlı
bir arayüze sahiptir ve Wazuh sunucusunun IP adresini tarayıcınızda
ziyaret ederek erişebilirsiniz. Kullanıcı arabirimi, grafiksel olarak
sunulan güvenlik olayları, güvenlik durumu özetleri, ajan durumu ve
yapılandırma ayarları gibi birçok bilgiyi sağlar. Ayrıca, kullanıcılar
özel raporlar oluşturabilir, güvenlik olaylarını filtreleyebilir ve
sistemdeki ajanları yönetebilir.

**Wazuh ile entegrasyonlar**

Wazuh, diğer güvenlik araçlarıyla entegrasyon sağlamak için bir dizi
seçenek sunar. Örneğin, Wazuh\'u Elastic Stack ile birleştirerek geniş
kapsamlı bir güvenlik bilgi ve olay yönetimi çözümü elde edebilirsiniz.
Elastic Stack, Wazuh tarafından toplanan güvenlik verilerini
indekslemek, analiz etmek ve görselleştirmek için kullanılır. Bu
entegrasyon sayesinde, olayları derinlemesine inceleyebilir, güvenlik
trendlerini analiz edebilir ve daha kapsamlı bir güvenlik görünümü elde
edebilirsiniz.

Diğer entegrasyon seçenekleri arasında SIEM (Security Information and
Event Management) sistemleriyle entegrasyon, olayları e-posta veya anlık
bildirimler aracılığıyla yönetim ekibine iletmek ve Wazuh API\'sini
kullanarak özel entegrasyonlar oluşturmak yer alır. Bu entegrasyonlar,
Wazuh\'un mevcut güvenlik altyapınıza kolayca entegre edilebilmesini ve
daha etkili bir şekilde çalışabilmesini sağlar. 

**Wazuh\'un sürekli geliştirilmesi**

Wazuh, açık kaynaklı bir proje olup aktif bir topluluğa sahiptir. Bu
topluluk, sürekli olarak yeni özellikler ekler, hataları düzeltir ve
güvenlik imzalarını günceller. Bu da Wazuh\'un güncel kalmasını ve yeni
tehditlere karşı etkin bir şekilde korunmayı sağlar. Ayrıca,
kullanıcılar da katkıda bulunabilir, geri bildirimler sağlayabilir ve
yeni özellik taleplerinde bulunabilir. Bu şekilde, Wazuh\'un sürekli
gelişmesi ve güvenlik endüstrisindeki değişikliklere adapte olması
sağlanır. 

**Wazuh ajanlarını listeleme**

Yukarıdaki örnek kod, Wazuh sunucusuna bir GET isteği göndererek
ajanları listeler. İstek sonucunda, ajanların bilgilerini elde eder ve
her ajanın ID\'si, hostname\'i ve IP adresini ekrana yazdırır.

 

**Wazuh kuralı ekleme**

Yukarıdaki örnek kod, Wazuh sunucusuna bir POST isteği göndererek yeni
bir kural ekler. İstek sonucunda, kural başarıyla eklenirse, eklenen
kuralın ID\'sini ekrana yazdırır.

Bu örnekler, Wazuh\'un bazı kullanım senaryolarını göstermektedir.
İhtiyaçlarınıza göre bu kodları özelleştirebilir ve Wazuh API\'sini
kullanarak farklı işlemler gerçekleştirebilirsiniz. 

**Belirli bir ajanın günlüklerini almak**

Yukarıdaki örnek kod, belirli bir ajanın günlüklerini almak için Wazuh
sunucusuna bir GET isteği gönderir. İstek sonucunda, ajanın günlüklerini
elde eder ve her günlüğün ID\'si ve mesajını ekrana yazdırır.
