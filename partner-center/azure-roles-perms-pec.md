---
title: Roller, iş ortağı kazanılmış kredi için izinler
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: İş ortaklarının iş ortağı kazanılmış kredilerin (PEC) kazanılabilecek roller ve izinler hakkında bilgi edinin. Bu rollerin iş ortağı merkezi 'nde çalışması farklıdır.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ca9cd1b09c840531c3652f71afbd9c66f657f877
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114840391"
---
# <a name="roles-and-permissions-required-to-earn-partner-earned-credit"></a>İş ortağı kazanılmış kredisi kazanmak için gereken roller ve izinler

Aşağıdaki roller, bir ortağın iş ortağı tarafından kazanılan krediler için uygun olup olmadığını tespit eden izin düzeylerine eşlenir.

>[!Important]
>Bu roller ve izinler, bir kullanıcının iş ortağı merkezi 'nde çalışması gereken roller ve izinlerle aynı değildir.

|**Role**   |**Açıklama**   |**PEC uygun**   |
|-----------------|:------------------|:--------------|
|Sahip  |Kaynaklara erişim dahil her şeyi yönetirsiniz.|Yes|
|Katılımcı |Kaynaklara erişim verme dışında her şeyi yönetirsiniz.|Yes|
|Okuyucu|Her şeyi görüntüleyebilir, ancak herhangi bir değişiklik yapamazsınız|No|
|ACRDelete|ACR silme|Yes|
|Acrimageimzalayan|ACR görüntü imzalayan|Yes|
|ACRPull|ACR çekme|Yes|
|AcrPush|ACR gönderimi|Yes|
|Acrquaranınereader|ACR karantina veri okuyucusu|No|
|AcrQuarantineWriter| ACR karantina veri yazıcısı|Yes|
|API Management hizmet Katılımcısı|Hizmeti ve API 'Leri yönetebilir|Yes|
|Hizmet Işletmeni rolü API Management|Hizmeti yönetebilir, ancak API 'Leri yönetemez|Yes|
|API Management hizmeti okuyucu rolü|Hizmet ve API 'lere salt okuma erişimi|No|
|Application Insights bileşeni katılımcısı|Application Insights bileşenlerini yönetir|Yes|
|Application Insights Snapshot Debugger|Application Insights Snapshot Debugger ile toplanan hata ayıklama anlık görüntülerini görüntülemek ve indirmek için kullanıcıya izin verir. Bu izinlerin sahip veya katkıda bulunan rollerine dahil edilmediğini unutmayın.|Yes|
Automation Iş Işleci | Otomasyon Runbook 'Larını kullanarak Iş oluşturun ve yönetin. | Yes | 
Otomasyon Operatörü | Automation Işleçleri, işleri başlatabilir, durdurabilir, askıya alabilir ve sürdürebilir | Yes | 
Otomasyon Runbook Işleci | Runbook 'un Işlerini oluşturabilmek için Runbook özelliklerini okuyun. | Yes | 
Avere Katılımcısı | , Bir avere vFXT kümesi oluşturabilir ve yönetebilir. | Yes | 
Avere Işleci | Kümeyi yönetmek için avere vFXT kümesi tarafından kullanılır | Yes | 
Azure Event Hubs veri sahibi | Azure Event Hubs kaynaklarına tam erişim sağlar. | Yes | 
Azure Event Hubs veri alıcısı | Azure Event Hubs kaynaklarına erişim izni verir. | Yes | 
Azure Event Hubs veri gönderici | Azure Event Hubs kaynaklarına erişim gönderilmesine izin verir. | Yes | 
Azure Kubernetes hizmet kümesi yönetici rolü | Küme Yöneticisi kimlik bilgisi eylemini listeleyin. | Yes | 
Azure Kubernetes hizmet kümesi Kullanıcı rolü | Küme kullanıcı kimlik bilgilerini Listele eylemi. | Yes | 
Azure Haritalar veri okuyucu (önizleme) | Azure haritalar hesabından ilgili harita okuma verilerine erişim izni verir. | No | 
Azure Service Bus veri sahibi | Azure Service Bus kaynaklarına tam erişim sağlar. | Yes | 
Azure Service Bus veri alıcısı | Azure Service Bus kaynaklarına erişim izni verir. | Yes | 
Azure Service Bus veri gönderici | Azure Service Bus kaynaklarına erişim izni verir. | Yes | 
Kayıt sahibini Azure Stack | Azure Stack kayıtlarını yönetmenizi sağlar. | Yes | 
Yedek Katılımcısı | Yedekleme hizmetini yönetmenizi sağlar, ancak kasaların oluşturamaz ve başkalarına erişim izni verebilir | Yes | 
Yedekleme Operatörü | Yedeklemenin kaldırılması, kasa oluşturma ve başkalarına erişim verme dışında yedekleme hizmetlerini yönetmenize olanak sağlar | Yes | 
Yedekleme Okuyucusu | Yedekleme hizmetlerini görüntüleme, ancak değişiklik yapma | No | 
Faturalama Okuyucusu | Faturalama verilerine okuma erişimine izin verir | No | 
BizTalk Katkıda Bulunanı | BizTalk hizmetlerini yönetmenize olanak sağlar, ancak bu hizmetlere erişmenizi sağlar. | Yes | 
Blok Zinciri Üyesi Düğüm Erişimi (Önizleme) | Blok Zinciri Üyesi düğümlerine erişime izin verir | Yes | 
Şema Katkıda Bulunanı | Şema tanımlarını yönetebilir, ancak bunları atayamaz. | Yes | 
Şema İşleci | Mevcut yayımlanmış şemaları atayamaz, ancak yeni şemalar oluşturamaz. NOT: Bu yalnızca atama kullanıcı tarafından atanan yönetilen kimlikle yapılırsa çalışır. | Yes | 
CDN Uç Nokta Katkıda Bulunanı | Uç CDN yönetebilir, ancak diğer kullanıcılara erişim izni vere değildir. | Yes | 
CDN Uç Nokta Okuyucusu | Uç CDN görünümünde değişiklik yapabilirsiniz. | No | 
CDN Profil Katkıda Bulunanı | Kullanıcı CDN uç noktalarını yönetebilir, ancak diğer kullanıcılara erişim izni vere değildir. | Yes | 
CDN Profil Okuyucusu | Uygulama CDN uç noktalarını görüntüleme, ancak değişiklik yapmama. | No | 
Klasik Ağ Katılımcısı | Klasik ağları yönetmenize olanak sağlar, ancak bu ağlara erişmenizi sağlar. | Yes | 
Klasik Depolama Hesabı Katkıda Bulunanı | Klasik depolama hesaplarını yönetmenize olanak sağlar, ancak bu hesaplara erişmenizi sağlar. | Yes | 
Klasik Depolama Hesap Anahtarı İşleci Hizmet Rolü | Klasik Depolama Hesap Anahtarı İşleçleri, Klasik HesapLarda anahtarları listeleye ve yeniden Depolama izin verilir | Yes | 
Klasik Sanal Makine Katılımcısı | Klasik sanal makineleri yönetmenize olanak sağlar, ancak bu sanal makinelere erişmenizi değil, bağlı olduğu sanal ağı veya depolama hesabını yönetmenizi sağlar. | Yes | 
Bilişsel Hizmetler Katkıda Bulunanı | Bilişsel Hizmetler anahtarları oluşturmanızı, okumanızı, güncelleştirmenizi, silmenizi ve yönetmenizi sağlar. | Yes | 
Bilişsel Hizmetler Veri Okuyucusu (Önizleme) | Bilişsel Hizmetler verilerini okumana olanak sağlar. | No | 
Bilişsel Hizmetler Kullanıcısı | Bilişsel Hizmetler'in anahtarlarını okuma ve listelemenizi sağlar. | No | 
Cosmos DB Hesabı Okuyucusu Rolü | Azure veritabanı Cosmos verilerini okuyabilir. Azure veritabanı hesaplarını yönetmek için bkz. DocumentDB Cosmos Katkıda Bulunanı. | No | 
Cosmos DB İşleci | Azure veritabanı Cosmos yönetmenize olanak sağlar, ancak bu hesaplarda verilere erişmenizi sağlar. Hesap anahtarlarına ve bağlantı dizelerine erişimi önler. | Yes | 
CosmosBackupOperator | Cosmos DB veritabanı veya hesap kapsayıcısı için geri yükleme isteği gönderebilirsiniz | Yes | 
Maliyet Yönetimi Katkıda Bulunanı | Maliyetleri görüntüleme ve maliyet yapılandırmasını yönetme (bütçeler, dışarı aktarmalar gibi) | Yes | 
Maliyet Yönetimi Okuyucusu | Maliyet verilerini ve yapılandırmasını görüntüleme (bütçeler, dışarı aktarmalar gibi) | No | 
Data Box Katkıda Bulunanı | Diğer kullanıcılara erişim vermek Data Box hizmet kapsamındaki her şeyi yönetmenize olanak sağlar. | Yes | 
Data Box Okuyucu | Sipariş veya sipariş Data Box ve başkalarına erişim verme dışında, Hizmet'i yönetmenize olanak sağlar. | No | 
Data Factory Katkıda Bulunanı | Veri fabrikalarının yanı sıra alt kaynakları da oluşturun ve yönetin. | Yes | 
Data Lake Analytics Geliştirici | Kendi işlerinizi göndermenize, izlemenize ve yönetmenize olanak sağlar, ancak hesap oluşturmanızı veya Data Lake Analytics sağlar. | Yes | 
Veri Temizleme | Analiz verilerini temizlebilirsiniz | Yes | 
DevTest Labs Kullanıcısı | Sanal makinelerinizi sanal makinenize bağlamanıza, başlatmanıza, yeniden başlatmanıza ve kapatmanıza olanak Azure DevTest Labs. | Yes | 
DNS Bölgesi Katkıda Bulunanı | Dns bölgelerini ve kayıt kümelerini Azure DNS ancak erişime sahip olanları denetlemenizi sağlar. | Yes | 
DocumentDB Hesabı Katkıda Bulunanı | Azure veritabanı Cosmos yönetebilir. Azure Cosmos DB eski adı DocumentDB'dir. | Yes | 
EventGrid EventSubscription Katkıda Bulunanı | EventGrid olay aboneliği işlemlerini yönetmenize olanak sağlar. | Yes | 
EventGrid EventSubscription Reader | EventGrid olay aboneliklerini okumana olanak sağlar. | No | 
HDInsight Küme İşleci | HDInsight küme yapılandırmalarını okuma ve değiştirmenizi sağlar. | Yes | 
HDInsight Etki Alanı Hizmetleri Katkıda Bulunanı | HDInsight Güvenlik Paketi için gereken Etki Alanı Hizmetleri ile ilgili işlemleri okuyabilir, Enterprise ve silebilir | Yes | 
Akıllı Sistemler Hesabı Katkıda Bulunanı | Akıllı Sistemler hesaplarını yönetmenize olanak sağlar, ancak bu hesaplara erişmenizi sağlar. | Yes | 
Key Vault Katkıda Bulunanı | Anahtar kasalarını yönetmenize olanak sağlar, ancak bu kasalara erişmenizi sağlar. | Yes | 
Laboratuvar Oluşturucusu | Azure Lab Hesapları altında yönetilen laboratuvarlarınızı oluşturmanıza, yönetmenize ve silmenize olanak sağlar. | Yes | 
Log Analytics Katkıda Bulunan | Log Analytics Katkıda Bulunanı tüm izleme verilerini okuyabilir ve izleme ayarlarını düzenleyebilir. İzleme ayarlarını düzenleme, VM uzantısını VM'lere eklemeyi içerir; Azure depolama hesabından günlük toplamayı yapılandırabilecek depolama hesabı anahtarlarını Depolama; Otomasyon hesaplarını oluşturma ve yapılandırma; çözüm ekleme; ve tüm Azure kaynaklarda Azure tanılamasını yapılandırma. | Yes | 
Log Analytics Okuyucusu | Log Analytics Okuyucusu tüm Azure kaynaklarda Azure tanılama yapılandırmasını görüntüleme de dahil olmak üzere tüm izleme verilerini görüntüleme ve aramanın yanı sıra izleme ayarlarını da görüntülemenizi sağlar. | No | 
Mantıksal Uygulama Katkıda Bulunanı | Mantıksal uygulamaları yönetmenize olanak sağlar, ancak erişimi değiştirmez. | Yes | 
Mantıksal Uygulama İşleci | Mantıksal uygulamaları okumanızı, etkinleştirmenizi ve devre dışı bırakmanızı sağlar, ancak bunları düzenlemenizi veya güncelleştirmenizi sağlar. | Yes | 
Yönetilen Uygulama İşleci Rolü | Yönetilen Uygulama kaynakları üzerinde eylemleri okumanız ve gerçekleştirmenizi sağlar | Yes | 
Yönetilen Uygulamalar Okuyucusu | Yönetilen bir uygulamada kaynakları okumanıza ve JIT erişimi isteğinde bulundurmanıza olanak sağlar. | No | 
Yönetilen Kimlik Katkıda Bulunanı | Kullanıcı Tarafından Atanan Kimlik Oluşturma, Okuma, Güncelleştirme ve Silme | Yes | 
Yönetilen Kimlik İşleci | Kullanıcı Tarafından Atanan Kimliği Okuma ve Atama | Yes | 
Yönetim Grubu Katkıda Bulunanı | Yönetim Grubu Katkıda Bulunanı Rolü | Yes | 
Yönetim Grubu Okuyucusu | Yönetim Grubu Okuyucusu Rolü | No | 
İzleme Katkıda Bulunanı | Tüm izleme verilerini okuyabilir ve izleme ayarlarını düzenleyebilir. Ayrıca bkz. Kullanmaya başlayın, izinler ve güvenlik özellikleriyle Azure İzleyici. | Yes | 
İzleme Ölçümleri Publisher | Ölçümleri Azure kaynaklarına göre yayımlamayı sağlar | Yes | 
İzleme Okuyucusu | Tüm izleme verilerini (ölçümler, günlükler vb.) okuyabilir. Ayrıca bkz. Kullanmaya başlayın, izinler ve güvenlik özellikleriyle Azure İzleyici. | No | 
Ağ Katılımcısı | Ağları yönetmenize olanak sağlar, ancak bu ağlara erişmenizi sağlar. | Yes | 
New Relic APM Hesabı Katkıda Bulunanı | Hesap ve New Relic Application Performance Management yönetmenize olanak sağlar, ancak bu hesaplara erişesiniz. | Yes | 
Okuyucu ve Veri Erişimi | Her şeyi görüntülemenizi sağlar, ancak depolama hesabını veya kaps bulunan kaynağı silmenizi veya oluşturmanızı sağlar. Ayrıca depolama hesabı anahtarlarına erişim yoluyla bir depolama hesabında yer alan tüm verilere okuma/yazma erişimi de sağlar. | Yes | 
Redis Cache Katkıda Bulunanı | Redis önbelleklerini yönetmenize olanak sağlar, ancak bu önbelleklere erişmenizi sağlar. | Yes | 
Kaynak İlkesi Katkıda Bulunanı (Önizleme) | (Önizleme) Kaynak ilkesi oluşturma/değiştirme, destek bileti oluşturma ve kaynakları/hiyerarşiyi okuma haklarına sahip OLAN, EA'dan doldurulmuş kullanıcılar. | Yes | 
Scheduler İş Koleksiyonları Katkıda Bulunanı | Scheduler iş koleksiyonlarını yönetmenize olanak sağlar, ancak bu koleksiyonlara erişmenizi sağlar. | Yes | 
Arama Hizmeti Katkıda Bulunanı | Arama hizmetlerini yönetmenize olanak sağlar, ancak bu hizmetlere erişmenizi sağlar. | Yes | 
Güvenlik Yöneticisi | Yalnızca Güvenlik Merkezi'nde: Güvenlik ilkelerini görüntüleme, güvenlik durumları görüntüleme, güvenlik ilkelerini düzenleme, uyarıları ve önerileri görüntüleme, uyarıları ve önerileri yok sayma | Yes | 
Güvenlik Yöneticisi (Eski) | Bu eski bir rol. Bunun yerine güvenlik yöneticisini kullanın | Yes | 
Güvenlik Okuyucusu | Yalnızca Güvenlik Merkezi'nde: Önerileri ve uyarıları görüntüleme, güvenlik ilkelerini görüntüleme, güvenlik durumları görüntüleme ama değişiklik yapma | No | 
Site Recovery Katkıda Bulunanı | Kasa oluşturma ve rol Site Recovery dışında bir hizmette yönetime olanak sağlar | Yes | 
Site Recovery Operatörü | Yük devretme ve yeniden çalışma işlemleri gerçekleştirmenizi sağlar, ancak diğer Site Recovery işlemleri gerçekleştirmemenizi sağlar | Yes | 
Site Recovery Okuyucusu | Yönetim durumunu görüntülemenizi Site Recovery diğer yönetim işlemlerini gerçekleştirmenizi sağlar | No | 
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
