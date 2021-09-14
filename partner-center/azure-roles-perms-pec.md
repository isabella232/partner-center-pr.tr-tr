---
title: Roller, iş ortağı tarafından kazanılan kredi izinleri
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: İş ortaklarının iş ortağı tarafından kazanılan krediler (PEC) kazanabilecekleri roller ve izinler hakkında bilgi edinmek. Bunlar, iş rollerinden farklı İş Ortağı Merkezi.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ca9cd1b09c840531c3652f71afbd9c66f657f877
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248320"
---
# <a name="roles-and-permissions-required-to-earn-partner-earned-credit"></a>İş ortağı tarafından kazanılan krediyi kazanmak için gereken roller ve izinler

Aşağıdaki roller, bir iş ortağının iş ortağı tarafından kazanılan krediler için uygun olup olmadığını belirleyen izin düzeyleriyle eşler.

>[!Important]
>Bu roller ve izinler, bir kullanıcının bir kullanıcıyla birlikte çalışması gereken roller ve izinler ile İş Ortağı Merkezi.

|**Role**   |**Açıklama**   |**PEC uygun**   |
|-----------------|:------------------|:--------------|
|Sahip  |Kaynaklara erişim de dahil olmak üzere her şeyi siz yönetirsiniz.|Yes|
|Katılımcı |Kaynaklara erişim izni vermek dışında her şeyi siz yönetirsiniz.|Yes|
|Okuyucu|Her şeyi görüntülemeniz ama herhangi bir değişiklik yapmama|No|
|ACRDelete|acr delete|Yes|
|ACRImageSigner|acr image signer|Yes|
|ACRPull|acr pull|Yes|
|AcrPush|acr push|Yes|
|AcrQuarantineReader|acr karantina veri okuyucusu|No|
|AcrQuarantineWriter| acr karantina veri yazıcısı|Yes|
|API Management Hizmeti Katkıda Bulunanı|Hizmeti ve API'leri yönetebilir|Yes|
|API Management Hizmet Operatörü Rolü|Hizmeti yönetebilir ancak API'leri yönetemz|Yes|
|API Management Hizmet Okuyucusu Rolü|Hizmet ve API'lere salt okunur erişim|No|
|Uygulama Analizler Bileşeni Katkıda Bulunanı|Uygulama yönetimi Analizler yönetir|Yes|
|Uygulama Analizler Snapshot Debugger|Kullanıcıya Application Analizler Snapshot Debugger ile toplanan hata ayıklama anlık görüntülerini görüntüleme ve indirme izni Analizler Snapshot Debugger. Bu izinlerin Sahip veya Katkıda Bulunan rollerine dahil olmadığını unutmayın.|Yes|
Otomasyon İşLeci | Otomasyon Runbook'larını kullanarak İşleri Oluşturma ve Yönetme. | Yes | 
Otomasyon Operatörü | Otomasyon Operatörleri işleri başlatarak, durdurarak, askıya alabilir ve sürdürebilecek | Yes | 
Otomasyon Runbook İşleci | Runbook'un İşlerini oluşturabilecek runbook özelliklerini okuyun. | Yes | 
Avere Katkıda Bulunanı | Bir küme oluşturabilir ve Avere vFXT yönetebilir. | Yes | 
Avere İşleci | Kümeyi Avere vFXT için küme tarafından kullanılır | Yes | 
Azure Event Hubs Sahibi | Tüm kaynaklara tam Azure Event Hubs sağlar. | Yes | 
Azure Event Hubs Veri Alıcısı | Kaynaklara erişim izni Azure Event Hubs sağlar. | Yes | 
Azure Event Hubs Veri Göndereni | Bu kaynaklara erişim Azure Event Hubs sağlar. | Yes | 
Azure Kubernetes Service Küme Yöneticisi Rolü | Küme yöneticisi kimlik bilgisi eylemlerini listele. | Yes | 
Azure Kubernetes Service Kümesi Kullanıcı Rolü | Küme kullanıcı kimlik bilgisi eylemlerini listele. | Yes | 
Azure Haritalar Veri Okuyucusu (Önizleme) | Azure Haritalar hesabından eşlemeyle ilgili verileri okuma erişimi sağlar. | No | 
Azure Service Bus Veri Sahibi | Azure sanal ağ kaynaklarına tam Service Bus sağlar. | Yes | 
Azure Service Bus Veri Alıcısı | Azure sanal ağ kaynaklarına erişim Service Bus sağlar. | Yes | 
Azure Service Bus Veri Göndereni | Azure sanal ağ kaynaklarına Service Bus sağlar. | Yes | 
Azure Stack Kayıt Sahibi | Kayıtlarınızı yönetmenize Azure Stack sağlar. | Yes | 
Yedekleme Katkıda Bulunanı | Yedekleme hizmetini yönetmenize olanak sağlar, ancak kasa oluşturamanıza ve başkalarına erişim veresiniz | Yes | 
Yedekleme Operatörü | Yedeklemenin kaldırılması, kasa oluşturma ve başkalarına erişim verme dışında yedekleme hizmetlerini yönetmenize olanak sağlar | Yes | 
Yedekleme Okuyucusu | Yedekleme hizmetlerini görüntüleme, ancak değişiklik yapma | No | 
Faturalama Okuyucusu | Faturalama verilerine okuma erişimine izin verir | No | 
BizTalk Katılımcısı | BizTalk hizmetlerini yönetmenize olanak sağlar, ancak bu hizmetlere erişmenizi sağlar. | Yes | 
Blok Zinciri Üyesi Düğüm Erişimi (Önizleme) | Blok Zinciri Üyesi düğümlerine erişime izin verir | Yes | 
Şema Katkıda Bulunanı | Şema tanımlarını yönetebilir, ancak bunları atayamaz. | Yes | 
Şema İşleci | Mevcut yayımlanmış şemaları atayamaz, ancak yeni şemalar oluşturamaz. NOT: Bu yalnızca atama kullanıcı tarafından atanan yönetilen kimlikle yapılırsa çalışır. | Yes | 
CDN Uç Nokta Katkıda Bulunanı | Uç CDN yönetebilir, ancak diğer kullanıcılara erişim izni vere değildir. | Yes | 
CDN Uç Nokta Okuyucusu | Uç CDN görünümünde değişiklik yapabilirsiniz. | No | 
CDN Profil Katkıda Bulunanı | Kullanıcı CDN uç noktalarını yönetebilir, ancak diğer kullanıcılara erişim izni vere değildir. | Yes | 
CDN Profil Okuyucusu | Profiller CDN uç noktalarını görüntüleme, ancak değişiklik yapmama. | No | 
Klasik Ağ Katılımcısı | Klasik ağları yönetmenize izin verir, ancak bu ağlara erişebilirsiniz. | Yes | 
Klasik Depolama Hesabı Katkıda Bulunanı | Klasik depolama hesaplarını yönetmenize olanak sağlar, ancak bu hesaplara erişmenizi sağlar. | Yes | 
Klasik Depolama Hesap Anahtarı İşleci Hizmet Rolü | Klasik Depolama Hesap Anahtarı İşleçleri Klasik Hesaplarda anahtarları listeleye ve yeniden Depolama izin verilir | Yes | 
Klasik Sanal Makine Katılımcısı | Klasik sanal makineleri yönetmenize olanak sağlar, ancak bu sanal makinelere erişmenizi değil, bunların bağlı olduğu sanal ağı veya depolama hesabını yönetmenizi sağlar. | Yes | 
Bilişsel Hizmetler Katkıda Bulunanı | Bilişsel Hizmetler anahtarları oluşturmanızı, okumanızı, güncelleştirmenizi, silmenizi ve yönetmenizi sağlar. | Yes | 
Bilişsel Hizmetler Veri Okuyucusu (Önizleme) | Bilişsel Hizmetler verilerini okumana olanak sağlar. | No | 
Bilişsel Hizmetler Kullanıcısı | Bilişsel Hizmetler'in anahtarlarını okuma ve listelemenizi sağlar. | No | 
Cosmos DB Hesabı Okuyucusu Rolü | Azure veritabanı Cosmos verilerini okuyabilir. Azure veritabanı hesaplarını yönetmek için bkz. DocumentDB Cosmos Katkıda Bulunanı. | No | 
Cosmos DB İşleci | Azure veritabanı Cosmos yönetmenize olanak sağlar, ancak bu hesaplarda verilere erişmenizi sağlar. Hesap anahtarlarına ve bağlantı dizelerine erişimi önler. | Yes | 
CosmosBackupOperator | Bir hesap için Cosmos DB veritabanı veya kapsayıcı için geri yükleme isteği gönderebilirsiniz | Yes | 
Maliyet Yönetimi Katkıda Bulunanı | Maliyetleri görüntüleme ve maliyet yapılandırmasını yönetme (bütçeler, dışarı aktarmalar gibi) | Yes | 
Maliyet Yönetimi Okuyucusu | Maliyet verilerini ve yapılandırmasını (bütçeler, dışarı aktarmalar gibi) görüntüleme | No | 
Data Box Katkıda Bulunanı | Diğer kullanıcılara erişim vermek Data Box hizmet kapsamındaki her şeyi yönetmenize olanak sağlar. | Yes | 
Data Box Okuyucu | Sipariş veya sipariş Data Box ve başkalarına erişim verme dışında, hizmet hizmet yönetiminizi yönetmenize olanak sağlar. | No | 
Data Factory Katkıda Bulunanı | Veri fabrikalarının yanı sıra alt kaynakları da oluşturun ve yönetin. | Yes | 
Data Lake Analytics Geliştirici | Kendi işlerinizi göndermenize, izlemenize ve yönetmenize olanak sağlar, ancak hesap oluşturmanızı veya Data Lake Analytics sağlar. | Yes | 
Veri Temizleme | Analiz verilerini temizlebilirsiniz | Yes | 
DevTest Labs Kullanıcısı | Sanal makinelerinizi sanal makinenize bağlamanıza, başlatmanıza, yeniden başlatmanıza ve kapatmanıza olanak Azure DevTest Labs. | Yes | 
DNS Bölgesi Katkıda Bulunanı | Dns bölgelerini ve kayıt kümelerini Azure DNS ancak erişime sahip olanları denetlemenizi sağlar. | Yes | 
DocumentDB Hesabı Katkıda Bulunanı | Azure veritabanı Cosmos yönetebilir. Azure Cosmos DB eski adı DocumentDB'dir. | Yes | 
EventGrid EventSubscription Katkıda Bulunanı | EventGrid olay aboneliği işlemlerini yönetmenize olanak sağlar. | Yes | 
EventGrid EventSubscription okuyucusu | EventGrid olay aboneliklerini okumanızı sağlar. | No | 
HDInsight küme operatörü | HDInsight küme yapılandırmasını okuyup değiştirmenize izin verir. | Yes | 
HDInsight etki alanı Hizmetleri Katılımcısı | hdınsight için gereken etki alanı hizmetleri ile ilgili işlemleri okuyabilir, oluşturabilir, değiştirebilir ve silebilir Kurumsal Güvenlik Paketi | Yes | 
Intelligent Systems hesabı Katılımcısı | Akıllı sistem hesaplarını yönetmenizi sağlar ancak onlara yönelik erişimleri vermez. | Yes | 
Katkıda bulunan Key Vault | Anahtar kasalarını yönetmenize izin verir, ancak bunlara erişim sağlamaz. | Yes | 
Laboratuvar Oluşturucu | Azure Laboratuvar hesaplarınız kapsamında yönetilen Laboratuvarlarınızı oluşturmanıza, yönetmenize ve silmenize olanak sağlar. | Yes | 
Log Analytics Katkıda Bulunan | Log Analytics katkı, tüm izleme verilerini okuyabilir ve izleme ayarlarını düzenleyebilir. İzleme ayarlarını düzenlediğinizde VM 'lere VM uzantısının eklenmesi dahildir; Azure Depolama günlüklerin toplanmasını yapılandırabilmek için depolama hesabı anahtarlarını okuma; Otomasyon hesapları oluşturma ve yapılandırma; çözümler ekleme; ve Azure tanılama 'yı tüm Azure kaynaklarında yapılandırma. | Yes | 
Log Analytics Okuyucusu | Log Analytics okuyucu tüm izleme verilerini görüntüleyip arayabilir ve tüm Azure kaynaklarında Azure tanılama 'nın yapılandırılmasını görüntüleme dahil olmak üzere izleme ayarlarını görüntüleyebilir. | No | 
Mantıksal uygulama Katılımcısı | Mantıksal uygulamaları yönetmenize izin verir, ancak bunlara erişimi değiştirmeyin. | Yes | 
Logic App Işleci | Logic Apps 'i okumanızı, etkinleştirmenizi ve devre dışı bırakmanızı sağlar, ancak bunları düzenleyemez veya güncelleştiremez. | Yes | 
Yönetilen uygulama Işletmeni rolü | Yönetilen uygulama kaynakları üzerinde işlemleri okuyup gerçekleştirmenize olanak tanır | Yes | 
Yönetilen uygulamalar okuyucusu | Yönetilen bir uygulamadaki kaynakları okumanızı ve JıT erişimi isteğinizi yapmanızı sağlar. | No | 
Yönetilen kimlik Katılımcısı | Kullanıcı tarafından atanan kimlik oluşturma, okuma, güncelleştirme ve silme | Yes | 
Yönetilen kimlik Işleci | Kullanıcı tarafından atanan kimliği okuma ve atama | Yes | 
Yönetim grubu Katılımcısı | Yönetim grubu katılımcısı rolü | Yes | 
Yönetim grubu okuyucusu | Yönetim grubu okuyucusu rolü | No | 
Katkıda bulunan izleniyor | Tüm izleme verilerini okuyabilir ve izleme ayarlarını düzenleyebilir. Ayrıca bkz. Azure Izleyici ile roller, izinler ve güvenlik ile çalışmaya başlama. | Yes | 
Ölçümleri izleme Publisher | Azure kaynaklarında ölçüm yayımlamaya izin vermez | Yes | 
İzleme okuyucusu | Tüm izleme verilerini okuyabilir (ölçümler, Günlükler vb.). Ayrıca bkz. Azure Izleyici ile roller, izinler ve güvenlik ile çalışmaya başlama. | No | 
Ağ Katılımcısı | Ağları yönetmenizi sağlar ancak onlara yönelik erişimleri vermez. | Yes | 
Yeni relik APM hesabı Katılımcısı | New Relic Application Performance Management hesaplarını ve uygulamaları yönetmenize izin verir, ancak bunlara erişimi kalmaz. | Yes | 
Okuyucu ve veri erişimi | Her şeyi görüntülemenize izin verir, ancak bir depolama hesabını veya kapsanan kaynağı silmenize veya oluşturmanıza izin vermez. Ayrıca depolama hesabı anahtarlarına erişim aracılığıyla bir depolama hesabında bulunan tüm verilere okuma/yazma erişimi de sağlar. | Yes | 
Katkıda bulunan Redis Cache | Redsıs önbellekler yönetmenize izin verir, ancak bunlara erişimi olmaz. | Yes | 
Kaynak Ilkesi katılımcısı (Önizleme) | Önizle Kaynak ilkesi oluşturma/değiştirme, destek bileti oluşturma ve kaynakları/hiyerarşiyi okuma haklarıyla EA 'dan Kullanıcı geri alma. | Yes | 
Zamanlayıcı Iş koleksiyonları Katılımcısı | Zamanlayıcı iş koleksiyonlarını yönetmenizi sağlar, ancak bunlara erişimi kalmaz. | Yes | 
Katkıda bulunan Arama Hizmeti | Arama hizmetlerini yönetmenize izin verir, ancak bunlara erişim izni vermez. | Yes | 
Güvenlik Yöneticisi | Yalnızca güvenlik merkezi 'nde: güvenlik ilkelerini görüntüleyebilir, güvenlik durumlarını görüntüleyebilir, güvenlik ilkelerini düzenleyebilir, uyarıları ve önerileri görüntüleyebilir, uyarıları ve önerileri kapatabilir | Yes | 
Güvenlik Yöneticisi (eski) | Bu eski bir roldür. Lütfen bunun yerine Güvenlik Yöneticisi 'ni kullanın | Yes | 
Güvenlik okuyucusu | Yalnızca güvenlik merkezi 'nde: önerileri ve uyarıları görüntüleyebilir, güvenlik ilkelerini görüntüleyebilir, güvenlik durumlarını görüntüleyebilir, ancak değişiklik yapamaz | No | 
Site Recovery Katkıda Bulunanı | Kasa oluşturma ve rol atama dışında Site Recovery hizmetini yönetmenizi sağlar | Yes | 
Site Recovery Operatörü | Yük devretme ve yeniden çalışma ve diğer Site Recovery yönetim işlemlerini gerçekleştirmenize izin verir | Yes | 
Site Recovery Okuyucusu | Site Recovery durumunu görüntülemenize izin verir, ancak diğer yönetim işlemlerini gerçekleştirmenize izin vermez | No | 
Uzamsal bağlayıcı hesabı Katılımcısı | Hesabınızdaki uzamsal bağlantıları yönetmenizi sağlar, ancak onları silmez | Yes | 
Uzamsal bağlayıcı hesap sahibi | Hesabınızdaki uzamsal bağlayıcıları, silme dahil olmak üzere yönetmenizi sağlar | Yes | 
Uzamsal bağlayıcı hesap okuyucu | Hesabınızdaki uzamsal Tutturucuların özelliklerini bulmanıza ve okumanızı sağlar | No | 
SQL DB Katılımcısı | SQL veritabanlarını yönetmenizi sağlar ancak onlara erişim izni vermez. ayrıca, güvenlikle ilgili ilkeleri veya onların üst SQL sunucularını yönetemezsiniz. | Yes | 
SQL Yönetilen örnek Katılımcısı | SQL yönetilen örnekleri ve gerekli ağ yapılandırmasını yönetmenizi sağlar, ancak başkalarına erişim izni veremeyiz. | Yes | 
SQL Güvenlik Yöneticisi | SQL sunucularının ve veritabanlarının güvenlikle ilgili ilkelerini yönetmenizi sağlar, ancak bunlara erişemez. | Yes | 
SQL Server Mcý | SQL sunucuları ve veritabanlarını yönetmenizi sağlar, ancak bunlara yönelik erişimi, güvenlikle ilgili ilkeleri değil. | Yes | 
Depolama Hesabı Katılımcısı | Depolama hesaplarının yönetimine izin verir. Paylaşılan anahtar yetkilendirmesi aracılığıyla verilere erişmek için kullanılabilen hesap anahtarına erişim sağlar. | Yes | 
Depolama Hesap anahtarı operatörü hizmet rolü | Depolama hesabı erişim anahtarlarının listelenmesi ve yeniden oluşturulmasına izin verir. | Yes | 
Depolama Blob Verileri Katkıda Bulunanı | Azure Depolama kapsayıcıları ve bloblarını okuma, yazma ve silme. Belirli bir veri işlemi için hangi eylemlerin gerekli olduğunu öğrenmek için bkz. blob ve kuyruk verisi işlemlerini çağırma Izinleri. | Yes | 
Depolama Blob Verileri Sahibi | , posıx erişim denetimi atama dahil olmak üzere Azure Depolama blob kapsayıcılarına ve verilerine tam erişim sağlar. Belirli bir veri işlemi için hangi eylemlerin gerekli olduğunu öğrenmek için bkz. blob ve kuyruk verisi işlemlerini çağırma Izinleri. | Yes | 
Depolama Blob Verileri Okuyucusu | Azure Depolama kapsayıcıları ve bloblarını okuyun ve listeleyin. Belirli bir veri işlemi için hangi eylemlerin gerekli olduğunu öğrenmek için bkz. blob ve kuyruk verisi işlemlerini çağırma Izinleri. | No | 
Depolama Blob Delegator | Azure AD kimlik bilgileriyle imzalanan bir kapsayıcı veya blob için paylaşılan erişim imzası oluşturmak üzere kullanılabilen bir Kullanıcı temsili anahtarı alın. Daha fazla bilgi için bkz. Kullanıcı temsili SAS oluşturma. | Yes | 
Depolama Dosyası Verileri SMB Paylaşımı Katkıda Bulunanı | SMB üzerinden Azure Depolama dosya paylaşımlarında okuma, yazma ve silme erişimine izin verir | Yes | 
Depolama Dosyası Verileri SMB Paylaşımı Yükseltilmiş Katkıda Bulunanı | SMB üzerinden Azure Depolama dosya paylaşımlarında okuma, yazma, silme ve değiştirme için NTFS izin erişimine izin verir | Yes | 
Depolama Dosyası Verileri SMB Paylaşımı Okuyucusu | SMB üzerinden Azure dosya paylaşımında okuma erişimine izin verir | No | 
Depolama Kuyruk verileri Katılımcısı | Azure Depolama kuyruklarını ve sıra iletilerini okuyun, yazın ve silin. Belirli bir veri işlemi için hangi eylemlerin gerekli olduğunu öğrenmek için bkz. blob ve kuyruk verisi işlemlerini çağırma Izinleri. | Yes | 
Depolama Veri Iletisi Işlemcisini sıraya al | Azure Depolama kuyruğundan bir iletiyi göz atın, alın ve silin. Belirli bir veri işlemi için hangi eylemlerin gerekli olduğunu öğrenmek için bkz. blob ve kuyruk verisi işlemlerini çağırma Izinleri. | Yes | 
Depolama Veri Iletisi göndereni sıraya al | Azure Depolama kuyruğuna ileti ekleyin. Belirli bir veri işlemi için hangi eylemlerin gerekli olduğunu öğrenmek için bkz. blob ve kuyruk verisi işlemlerini çağırma Izinleri. | Yes | 
Depolama Veri okuyucuyu sıraya al | Azure Depolama kuyruklarını ve sıra iletilerini okuyun ve listeleyin. Belirli bir veri işlemi için hangi eylemlerin gerekli olduğunu öğrenmek için bkz. blob ve kuyruk verisi işlemlerini çağırma Izinleri. | No | 
Destek Isteği Katılımcısı | Destek istekleri oluşturmanızı ve yönetmenizi sağlar | Yes | 
Traffic Manager Mcý | Traffic Manager profillerini yönetmenizi sağlar, ancak bunlara kimlerin erişebileceğini denetlemenize izin vermez. | Yes | 
Kullanıcı Erişimi Yöneticisi | Azure kaynaklarına Kullanıcı erişimini yönetmenizi sağlar. | Yes | 
Sanal Makine Yöneticisi oturum açma | Portalda sanal makineleri görüntüleme ve yönetici olarak oturum açma | Yes | 
Sanal Makine Katılımcısı | Sanal makineleri yönetmenize izin verir, ancak bunlara bağlı oldukları sanal ağ veya depolama hesabına erişemez. | Yes | 
Sanal makine Kullanıcı oturumu açma | Portalda sanal makineleri görüntüleyin ve normal bir kullanıcı olarak oturum açın. | Yes | 
Web planı Katılımcısı | Web siteleri için Web planlarını yönetmenizi sağlar, ancak bunlara erişemez. | Yes | 
Web sitesi Katılımcısı | Web sitelerini yönetmenizi sağlar, ancak bunlara erişemez | Evet |

## <a name="next-steps"></a>Sonraki adımlar

- [İş ortağı kazanılmış kredi-CSP 'de yeni ticaret deneyiminde nasıl çalıştığına ilişkin genel bakış](partner-earned-credit.md)
