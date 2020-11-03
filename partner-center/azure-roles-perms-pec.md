---
title: Roller, iş ortağı kazanılmış kredi için izinler
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: İş ortaklarının iş ortağı kazanılmış kredilerin (PEC) kazanılabilecek roller ve izinler hakkında bilgi edinin. Bu rollerin iş ortağı merkezi 'nde çalışması farklıdır.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f48774cb830ceb575a84177efb57431afdcb9b25
ms.sourcegitcommit: 5fc28f6f81eaebb84e1faa71848afb504e181f37
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/11/2020
ms.locfileid: "92531418"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>İş ortağı kazanılmış kredisi kazanımak için uygun roller ve izinler

Aşağıdaki roller, bir ortağın iş ortağı tarafından kazanılan krediler için uygun olup olmadığını tespit eden izin düzeylerine eşlenir.

>[!Important]
>Bu roller ve izinler, bir kullanıcının iş ortağı merkezi 'nde çalışması gereken roller ve izinlerle aynı değildir.

|**Role**   |**Açıklama**   |**PEC uygun**   |
|-----------------|:------------------|:--------------|
|Sahip  |Kaynaklara erişim dahil her şeyi yönetirsiniz.|Evet|
|Katılımcı |Kaynaklara erişim verme dışında her şeyi yönetirsiniz.|Evet|
|Okuyucu|Her şeyi görüntüleyebilir, ancak herhangi bir değişiklik yapamazsınız|Hayır|
|ACRDelete|ACR silme|Evet|
|Acrimageimzalayan|ACR görüntü imzalayan|Evet|
|ACRPull|ACR çekme|Evet|
|AcrPush|ACR gönderimi|Evet|
|Acrquaranınereader|ACR karantina veri okuyucusu|Hayır|
|AcrQuarantineWriter| ACR karantina veri yazıcısı|Evet|
|API Management hizmet Katılımcısı|Hizmeti ve API 'Leri yönetebilir|Evet|
|Hizmet Işletmeni rolü API Management|Hizmeti yönetebilir, ancak API 'Leri yönetemez|Evet|
|API Management hizmeti okuyucu rolü|Hizmet ve API 'lere salt okuma erişimi|Hayır|
|Application Insights bileşeni Katılımcısı|Application Insights bileşenlerini yönetir|Evet|
|Application Insights Snapshot Debugger|Application Insights Snapshot Debugger ile toplanan hata ayıklama anlık görüntülerini görüntülemek ve indirmek için kullanıcıya izin verir. Bu izinlerin sahip veya katkıda bulunan rollerine dahil edilmediğini unutmayın.|Evet|
Automation Iş Işleci | Otomasyon Runbook 'Larını kullanarak Iş oluşturun ve yönetin. | Evet | 
Otomasyon Operatörü | Automation Işleçleri, işleri başlatabilir, durdurabilir, askıya alabilir ve sürdürebilir | Evet | 
Otomasyon Runbook Işleci | Runbook 'un Işlerini oluşturabilmek için Runbook özelliklerini okuyun. | Evet | 
Avere Katılımcısı | , Bir avere vFXT kümesi oluşturabilir ve yönetebilir. | Evet | 
Avere Işleci | Kümeyi yönetmek için avere vFXT kümesi tarafından kullanılır | Evet | 
Azure Event Hubs veri sahibi | Azure Event Hubs kaynaklarına tam erişim sağlar. | Evet | 
Azure Event Hubs veri alıcısı | Azure Event Hubs kaynaklarına erişim izni verir. | Evet | 
Azure Event Hubs veri gönderici | Azure Event Hubs kaynaklarına erişim gönderilmesine izin verir. | Evet | 
Azure Kubernetes hizmet kümesi yönetici rolü | Küme Yöneticisi kimlik bilgisi eylemini listeleyin. | Evet | 
Azure Kubernetes hizmet kümesi Kullanıcı rolü | Küme kullanıcı kimlik bilgilerini Listele eylemi. | Evet | 
Azure haritalar veri okuyucu (Önizleme) | Azure haritalar hesabından ilgili harita okuma verilerine erişim izni verir. | Hayır | 
Azure Service Bus veri sahibi | Azure Service Bus kaynaklara tam erişim sağlar. | Evet | 
Azure Service Bus veri alıcısı | Azure Service Bus kaynaklarına erişim izni verir. | Evet | 
Veri Göndericisini Azure Service Bus | Azure Service Bus kaynaklarına erişim izni verir. | Evet | 
Kayıt sahibini Azure Stack | Azure Stack kayıtlarını yönetmenizi sağlar. | Evet | 
Yedek Katılımcısı | Yedekleme hizmetini yönetmenizi sağlar, ancak kasaların oluşturamaz ve başkalarına erişim izni verebilir | Evet | 
Yedekleme Işletmeni | Yedekleme kaldırma, kasa oluşturma ve başkalarına erişim verme dışında yedekleme hizmetlerini yönetmenizi sağlar | Evet | 
Yedekleme okuyucusu | Yedekleme hizmetlerini görüntüleyebilir, ancak değişiklik yapamaz | Hayır | 
Faturalama Okuyucusu | Faturalandırma verilerine okuma erişimi sağlar | Hayır | 
BizTalk Katılımcısı | BizTalk hizmetlerini yönetmenizi sağlar ancak onlara erişim izni vermez. | Evet | 
Blok zinciri üye düğümü erişimi (Önizleme) | Blok zinciri üye düğümlerine erişim sağlar | Evet | 
Blueprint Katılımcısı | Şema tanımlarını yönetebilir, ancak atamazsınız. | Evet | 
Blueprint Işleci | Varolan yayımlanmış şemaları atayabilir, ancak yeni şemaları oluşturamaz. Not: Bu yalnızca atama Kullanıcı tarafından atanan yönetilen bir kimlikle yapıldığında geçerlidir. | Evet | 
CDN uç noktası Katılımcısı | CDN uç noktalarını yönetebilir, ancak diğer kullanıcılara erişim izni veremez. | Evet | 
CDN uç nokta okuyucusu | CDN uç noktalarını görüntüleyebilir, ancak değişiklik yapamaz. | Hayır | 
CDN profili Katılımcısı | CDN profillerini ve uç noktalarını yönetebilir, ancak diğer kullanıcılara erişim izni veremez. | Evet | 
CDN profili okuyucu | CDN profillerini ve uç noktalarını görüntüleyebilir, ancak değişiklik yapamaz. | Hayır | 
Klasik Ağ Katılımcısı | Klasik ağları yönetmenize izin verir, ancak bunlara erişemez. | Evet | 
Klasik depolama hesabı Katılımcısı | Klasik depolama hesaplarını yönetmenize izin verir, ancak bunlara erişimi kalmaz. | Evet | 
Klasik depolama hesabı anahtar operatörü hizmet rolü | Klasik depolama hesabı anahtar Işleçleri klasik depolama hesaplarında anahtarları listeleme ve yeniden oluşturma izni verilir | Evet | 
Klasik sanal makine Katılımcısı | Klasik sanal makineleri yönetmenizi sağlar ancak bunlara yönelik erişimi, bağlı oldukları sanal ağ veya depolama hesabı için değil. | Evet | 
Bilişsel hizmetler Katılımcısı | Bilişsel hizmetler için anahtar oluşturma, okuma, güncelleştirme, silme ve yönetme olanağı sağlar. | Evet | 
Bilişsel hizmetler veri okuyucu (Önizleme) | Bilişsel hizmetler verilerini okumanızı sağlar. | Hayır | 
Bilişsel hizmetler kullanıcısı | Bilişsel hizmetler 'in anahtarlarını okuyup listelemenizi sağlar. | Hayır | 
Cosmos DB hesabı okuyucu rolü | Azure Cosmos DB hesabı verilerini okuyabilir. Azure Cosmos DB hesaplarını yönetmek için DocumentDB hesabı katılımcısı konusuna bakın. | Hayır | 
Cosmos DB Işleci | Azure Cosmos DB hesaplarını yönetmenizi sağlar ancak içerdikleri verilere erişemez. Hesap anahtarlarına ve bağlantı dizelerine erişimi engeller. | Evet | 
CosmosBackupOperator | Bir Cosmos DB veritabanı veya bir hesabın kapsayıcısı için geri yükleme isteği gönderebilir | Evet | 
Maliyet yönetimi Katılımcısı | Maliyetleri görüntüleyebilir ve maliyet yapılandırmasını yönetebilir (örn. bütçeler, dışarı aktarmalar) | Evet | 
Maliyet yönetimi okuyucusu | Maliyet verilerini ve yapılandırmayı görüntüleyebilir (örneğin, bütçeler, dışarı aktarmalar) | Hayır | 
Katkıda bulunan Data Box | , Diğer kullanıcılara erişim izni hariç Data Box hizmeti altındaki her şeyi yönetmenizi sağlar. | Evet | 
Data Box okuyucu | Sipariş oluşturma veya düzenleme sırası ayrıntıları ve başkalarına erişim verme dışında Data Box hizmetini yönetmenizi sağlar. | Hayır | 
Katkıda bulunan Data Factory | Veri fabrikalarının yanı sıra bunların içindeki alt kaynakları oluşturun ve yönetin. | Evet | 
Data Lake Analytics geliştirici | Kendi işlerinizi göndermenize, izlemenize ve yönetmenize izin verir, ancak Data Lake Analytics Hesapları oluşturamaz veya silemezsiniz. | Evet | 
Veri Takiger | Analiz verilerini temizedebilir | Evet | 
DevTest Labs kullanıcısı | Azure DevTest Labs sanal makinelerinizi bağlamanıza, başlatmanıza, yeniden başlatmanıza ve kapatımanıza olanak sağlar. | Evet | 
DNS bölgesi Katılımcısı | Azure DNS, DNS bölgelerini ve kayıt kümelerini yönetmenizi sağlar, ancak bunlara kimlerin erişebileceğini denetlemenize izin vermez. | Evet | 
DocumentDB hesabı Katılımcısı | , Azure Cosmos DB hesaplarını yönetebilir. Azure Cosmos DB daha önce DocumentDB olarak bilinirdi. | Evet | 
EventGrid EventSubscription Katılımcısı | EventGrid olay aboneliği işlemlerini yönetmenizi sağlar. | Evet | 
EventGrid EventSubscription okuyucusu | EventGrid olay aboneliklerini okumanızı sağlar. | Hayır | 
HDInsight küme operatörü | HDInsight küme yapılandırmasını okuyup değiştirmenize izin verir. | Evet | 
HDInsight etki alanı Hizmetleri Katılımcısı | HDInsight için gereken etki alanı Hizmetleri ile ilgili işlemleri okuyabilir, oluşturabilir, değiştirebilir ve silebilir Kurumsal Güvenlik Paketi | Evet | 
Intelligent Systems hesabı Katılımcısı | Akıllı sistem hesaplarını yönetmenizi sağlar ancak onlara yönelik erişimleri vermez. | Evet | 
Katkıda bulunan Key Vault | Anahtar kasalarını yönetmenize izin verir, ancak bunlara erişim sağlamaz. | Evet | 
Laboratuvar Oluşturucu | Azure Laboratuvar hesaplarınız kapsamında yönetilen Laboratuvarlarınızı oluşturmanıza, yönetmenize ve silmenize olanak sağlar. | Evet | 
Log Analytics Katkıda Bulunan | Log Analytics katkı, tüm izleme verilerini okuyabilir ve izleme ayarlarını düzenleyebilir. İzleme ayarlarını düzenlediğinizde VM 'lere VM uzantısının eklenmesi dahildir; Azure depolama 'dan günlüklerin toplanmasını yapılandırabilmek için depolama hesabı anahtarlarını okuma; Otomasyon hesapları oluşturma ve yapılandırma; çözümler ekleme; ve Azure tanılama 'yı tüm Azure kaynaklarında yapılandırma. | Evet | 
Log Analytics Okuyucusu | Log Analytics okuyucu tüm izleme verilerini görüntüleyip arayabilir ve tüm Azure kaynaklarında Azure tanılama 'nın yapılandırılmasını görüntüleme dahil olmak üzere izleme ayarlarını görüntüleyebilir. | Hayır | 
Mantıksal uygulama Katılımcısı | Mantıksal uygulamaları yönetmenize izin verir, ancak bunlara erişimi değiştirmeyin. | Evet | 
Logic App Işleci | Logic Apps 'i okumanızı, etkinleştirmenizi ve devre dışı bırakmanızı sağlar, ancak bunları düzenleyemez veya güncelleştiremez. | Evet | 
Yönetilen uygulama Işletmeni rolü | Yönetilen uygulama kaynakları üzerinde işlemleri okuyup gerçekleştirmenize olanak tanır | Evet | 
Yönetilen uygulamalar okuyucusu | Yönetilen bir uygulamadaki kaynakları okumanızı ve JıT erişimi isteğinizi yapmanızı sağlar. | Hayır | 
Yönetilen kimlik Katılımcısı | Kullanıcı tarafından atanan kimlik oluşturma, okuma, güncelleştirme ve silme | Evet | 
Yönetilen kimlik Işleci | Kullanıcı tarafından atanan kimliği okuma ve atama | Evet | 
Yönetim grubu Katılımcısı | Yönetim grubu katılımcısı rolü | Evet | 
Yönetim grubu okuyucusu | Yönetim grubu okuyucusu rolü | Hayır | 
Katkıda bulunan izleniyor | Tüm izleme verilerini okuyabilir ve izleme ayarlarını düzenleyebilir. Ayrıca bkz. Azure Izleyici ile roller, izinler ve güvenlik ile çalışmaya başlama. | Evet | 
Ölçüm yayımcısını izleme | Azure kaynaklarında ölçüm yayımlamaya izin vermez | Evet | 
İzleme okuyucusu | Tüm izleme verilerini okuyabilir (ölçümler, Günlükler vb.). Ayrıca bkz. Azure Izleyici ile roller, izinler ve güvenlik ile çalışmaya başlama. | Hayır | 
Ağ Katılımcısı | Ağları yönetmenizi sağlar ancak onlara yönelik erişimleri vermez. | Evet | 
Yeni relik APM hesabı Katılımcısı | New Relic Application Performance Management hesaplarını ve uygulamaları yönetmenize izin verir, ancak bunlara erişimi kalmaz. | Evet | 
Okuyucu ve veri erişimi | Her şeyi görüntülemenize izin verir, ancak bir depolama hesabını veya kapsanan kaynağı silmenize veya oluşturmanıza izin vermez. Ayrıca depolama hesabı anahtarlarına erişim aracılığıyla bir depolama hesabında bulunan tüm verilere okuma/yazma erişimi de sağlar. | Evet | 
Katkıda bulunan Redis Cache | Redsıs önbellekler yönetmenize izin verir, ancak bunlara erişimi olmaz. | Evet | 
Kaynak Ilkesi katılımcısı (Önizleme) | Önizle Kaynak ilkesi oluşturma/değiştirme, destek bileti oluşturma ve kaynakları/hiyerarşiyi okuma haklarıyla EA 'dan Kullanıcı geri alma. | Evet | 
Zamanlayıcı Iş koleksiyonları Katılımcısı | Zamanlayıcı iş koleksiyonlarını yönetmenizi sağlar, ancak bunlara erişimi kalmaz. | Evet | 
Katkıda bulunan Arama Hizmeti | Arama hizmetlerini yönetmenize izin verir, ancak bunlara erişim izni vermez. | Evet | 
Güvenlik Yöneticisi | Yalnızca güvenlik merkezi 'nde: güvenlik ilkelerini görüntüleyebilir, güvenlik durumlarını görüntüleyebilir, güvenlik ilkelerini düzenleyebilir, uyarıları ve önerileri görüntüleyebilir, uyarıları ve önerileri kapatabilir | Evet | 
Güvenlik Yöneticisi (eski) | Bu eski bir roldür. Lütfen bunun yerine Güvenlik Yöneticisi 'ni kullanın | Evet | 
Güvenlik Okuyucusu | Yalnızca güvenlik merkezi 'nde: önerileri ve uyarıları görüntüleyebilir, güvenlik ilkelerini görüntüleyebilir, güvenlik durumlarını görüntüleyebilir, ancak değişiklik yapamaz | Hayır | 
Katkıda bulunan Site Recovery | Kasa oluşturma ve rol atama dışında Site Recovery hizmetini yönetmenizi sağlar | Evet | 
Site Recovery Işleci | Yük devretme ve yeniden çalışma ve diğer Site Recovery yönetim işlemlerini gerçekleştirmenize izin verir | Evet | 
Site Recovery okuyucu | Site Recovery durumunu görüntülemenize izin verir, ancak diğer yönetim işlemlerini gerçekleştirmenize izin vermez | Hayır | 
Uzamsal bağlayıcı hesabı Katılımcısı | Hesabınızdaki uzamsal bağlantıları yönetmenizi sağlar, ancak onları silmez | Evet | 
Uzamsal bağlayıcı hesap sahibi | Hesabınızdaki uzamsal bağlayıcıları, silme dahil olmak üzere yönetmenizi sağlar | Evet | 
Uzamsal bağlayıcı hesap okuyucu | Hesabınızdaki uzamsal Tutturucuların özelliklerini bulmanıza ve okumanızı sağlar | Hayır | 
SQL DB Katılımcısı | SQL veritabanlarını yönetmenizi sağlar ancak onlara yönelik erişimleri vermez. Ayrıca, güvenlikle ilgili ilkeleri veya bunların üst SQL sunucularını yönetemezsiniz. | Evet | 
SQL yönetilen örnek Katılımcısı | SQL yönetilen örnekleri ve gerekli ağ yapılandırmasını yönetmenizi sağlar, ancak başkalarına erişim izni veremeyiz. | Evet | 
SQL Güvenlik Yöneticisi | , SQL Server ve veritabanlarının güvenlikle ilgili ilkelerini yönetmenizi sağlar, ancak bunlara erişemez. | Evet | 
Katkıda bulunan SQL Server | SQL Server ve veritabanlarını yönetmenizi sağlar, ancak bunlara yönelik erişimleri ve güvenlikle ilgili ilkeleri yönetemez. | Evet | 
Depolama Hesabı Katılımcısı | Depolama hesaplarının yönetimine izin verir. Paylaşılan anahtar yetkilendirmesi aracılığıyla verilere erişmek için kullanılabilen hesap anahtarına erişim sağlar. | Evet | 
Depolama hesabı anahtar operatörü hizmet rolü | Depolama hesabı erişim anahtarlarının listelenmesi ve yeniden oluşturulmasına izin verir. | Evet | 
Depolama Blob Verileri Katkıda Bulunanı | Azure depolama kapsayıcıları ve bloblarını okuyun, yazın ve silin. Belirli bir veri işlemi için hangi eylemlerin gerekli olduğunu öğrenmek için bkz. blob ve kuyruk verisi işlemlerini çağırma Izinleri. | Evet | 
Depolama Blob Verileri Sahibi | , POSIX erişim denetimi atama dahil olmak üzere Azure depolama blob kapsayıcılarına ve verilerine tam erişim sağlar. Belirli bir veri işlemi için hangi eylemlerin gerekli olduğunu öğrenmek için bkz. blob ve kuyruk verisi işlemlerini çağırma Izinleri. | Evet | 
Depolama Blob Verileri Okuyucusu | Azure depolama kapsayıcıları ve bloblarını okuyun ve listeleyin. Belirli bir veri işlemi için hangi eylemlerin gerekli olduğunu öğrenmek için bkz. blob ve kuyruk verisi işlemlerini çağırma Izinleri. | Hayır | 
Depolama Blobu Delegator | Azure AD kimlik bilgileriyle imzalanan bir kapsayıcı veya blob için paylaşılan erişim imzası oluşturmak üzere kullanılabilen bir Kullanıcı temsili anahtarı alın. Daha fazla bilgi için bkz. Kullanıcı temsili SAS oluşturma. | Evet | 
Depolama Dosyası Verileri SMB Paylaşımı Katkıda Bulunanı | SMB üzerinden Azure depolama dosya paylaşımlarında okuma, yazma ve silme erişimine izin verir | Evet | 
Depolama Dosyası Verileri SMB Paylaşımı Yükseltilmiş Katkıda Bulunanı | SMB üzerinden Azure depolama dosya paylaşımlarında NTFS izin erişimini okuma, yazma, silme ve değiştirme sağlar | Evet | 
Depolama Dosyası Verileri SMB Paylaşımı Okuyucusu | SMB üzerinden Azure dosya paylaşımında okuma erişimine izin verir | Hayır | 
Depolama kuyruğu verileri Katılımcısı | Azure depolama kuyruklarını ve sıra iletilerini okuyun, yazın ve silin. Belirli bir veri işlemi için hangi eylemlerin gerekli olduğunu öğrenmek için bkz. blob ve kuyruk verisi işlemlerini çağırma Izinleri. | Evet | 
Depolama kuyruğu veri Iletisi Işlemcisi | Azure depolama kuyruğundan bir iletiyi göz atın, alın ve silin. Belirli bir veri işlemi için hangi eylemlerin gerekli olduğunu öğrenmek için bkz. blob ve kuyruk verisi işlemlerini çağırma Izinleri. | Evet | 
Depolama kuyruğu veri Iletisi gönderici | Bir Azure depolama kuyruğuna ileti ekleyin. Belirli bir veri işlemi için hangi eylemlerin gerekli olduğunu öğrenmek için bkz. blob ve kuyruk verisi işlemlerini çağırma Izinleri. | Evet | 
Depolama kuyruğu veri okuyucusu | Azure depolama kuyruklarını ve sıra iletilerini okuyun ve listeleyin. Belirli bir veri işlemi için hangi eylemlerin gerekli olduğunu öğrenmek için bkz. blob ve kuyruk verisi işlemlerini çağırma Izinleri. | Hayır | 
Destek Isteği Katılımcısı | Destek istekleri oluşturmanızı ve yönetmenizi sağlar | Evet | 
Katkıda bulunan Traffic Manager | Traffic Manager profillerini yönetmenizi sağlar, ancak bunlara kimlerin erişebileceğini denetlemenize izin vermez. | Evet | 
Kullanıcı Erişimi Yöneticisi | Azure kaynaklarına Kullanıcı erişimini yönetmenizi sağlar. | Evet | 
Sanal Makine Yöneticisi oturum açma | Portalda sanal makineleri görüntüleme ve yönetici olarak oturum açma | Evet | 
Sanal Makine Katılımcısı | Sanal makineleri yönetmenize izin verir, ancak bunlara bağlı oldukları sanal ağ veya depolama hesabına erişemez. | Evet | 
Sanal makine Kullanıcı oturumu açma | Portalda sanal makineleri görüntüleyin ve normal bir kullanıcı olarak oturum açın. | Evet | 
Web planı Katılımcısı | Web siteleri için Web planlarını yönetmenizi sağlar, ancak bunlara erişemez. | Evet | 
Web sitesi Katılımcısı | Web sitelerini yönetmenizi sağlar, ancak bunlara erişemez | Evet |
