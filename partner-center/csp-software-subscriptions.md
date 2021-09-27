---
title: CSP üzerinden yazılım aboneliği satma
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: CSP programındaki iş ortaklarının, müşteriler için Azure ayrılmış örnekleri ve sunucu abonelikleri satın almak, yönetmek, satmak ve iptal etmek için Iş Ortağı Merkezi 'ni nasıl kullanabileceği hakkında bilgi edinin.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: fcd446cf38ee9e84122f59ece2db22c7e6129f83
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129073834"
---
# <a name="sell-software-subscriptions-through-the-cloud-solution-provider-csp-program"></a>Bulut Çözümü Sağlayıcısı (CSP) programı aracılığıyla yazılım abonelikleri satma

**Uygun roller**: yönetici Aracısı | Genel yönetici

Azure ayırmaları ve sunucu abonelikleri (Windows server ve SQL Server abonelikleri) sayesinde, CSP programındaki iş ortakları, yüksek düzeyde öngörülebilir ve kalıcı bulut iş yüklerini desteklemeye yönelik daha uygun maliyetli çözümler için hızlı büyümekte olan müşteri taleplerini daha iyi ele alabilir. 

Artık Azure ayırmaları ve sunucu aboneliklerini, Iş ortağı merkezi ve Azure portal aracılığıyla ticari müşteriler adına alabilir, sağlayabilir ve yönetebilir Azure Hibrit Avantajı.

Azure Hibrit Avantajı, Windows sunucusu lisanslarınızdan daha fazla değer almanıza ve sanal makinelerde yüzde 40 ' a varan tasarruf etmenize yardımcı olur. yazılım güvencesi kapsamındaki Windows Server veri merkezi ve standart sürüm lisanslarıyla avantajını kullanabilirsiniz. sürüme bağlı olarak, Azure 'da Windows Server sanal makinelerini çalıştırmak için lisanslarınızı dönüştürebilir veya yeniden kullanabilir ve daha düşük bir temel işlem ücreti (örneğin, Linux sanal makine ücretleri) ödeyebilirsiniz.

## <a name="azure-reservations-unavailable-markets"></a>Azure ayırmaları kullanılamayan pazarlar

>[!IMPORTANT]
>Azure ayırmaları **aşağıdaki pazarlarda kullanılamaz:**  
>  
> **Kullanılamayan pazarlar (alfabetik sırada)**
>
> |A-GI   | Gr-PAL  | PAP-Z |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | Aland Adaları     | Grönland     | Papua Yeni Gine     |
> | Amerikan Samoası     | Grenada     | Pitcairn Adaları     |
> | Andorra     | Guadeloupe     | Reunion     |
> | Anguilla     | Guam     | Saba   |
> | Antarktika     | Guernsey     | Saint Barthelemy   |
> | Antigua ve Barbuda       | Gine     | Saint Lucia   |
> | Aruba       | Gine-Bissau     | Saint Martin   |
> | Azerbaycan       | Guyana     | Saint Pierre ve Miquelon   |
> | Benin     | Haiti       | Saint Vincent ve Grenadinler     |
> | Butan     | Heard Adası ve McDonald Adaları       | Samoa     |
> | Bonaire     | Man Adası     | San Marino     |
> | Bouvet Adası     | Jan Mayen     | Sao Tome ve Principe   |
> | Britanya Hint Okyanusu Toprakları       | Jersey     | Seyşeller   |
> | Britanya Virjin Adaları     | Kiribati       | Sierra Leone   |
> | Burkina Faso     | Kosova     | Sint Eustatius     |
> | Burundi     | Laos     | Sint Maarten     |
> | Kamboçya     | Lesotho     | Solomon Adaları     |
> | Orta Afrika Cumhuriyeti     | Liberya     | Somali     |
> | Çad     | Madagaskar     | Güney Georgia ve Güney Sandwich Adaları     |
> | Çin     | Malavi     | Güney Sudan     |
> | Christmas Adası     | Maldivler     | Saint Helena, Ascension ve Tristan da Cunha     |
> | Cocos (Keeling) Adaları     | Mali     | Surinam     |
> | Komorlar     | Marshall Adaları     | Svalbard     |
> | Kongo Cumhuriyeti     | Martinique     | Svaziland     |
> | Kongo (KDC)     | Moritanya     | Timor-Leste   |
> | Cook Adaları     | Mayotte     | Togo   |
> | Cibuti     | Mikronezya     | Tokelau   |
> | Dominika     | Montserrat     | Tonga   |
> | Ekvator Ginesi     | Mozambik     | Turks ve Caicos Adaları   |
> | Eritre     | Myanmar     | Tuvalu   |
> | Falkland Adaları     | Nauru     | ABD'de Outlying Adaları   |
> | Fransız Guyanası     | Yeni Kaledonya     | Vanuatu   |
> | Fransız Polinezyası     | Nijer     | Vatikan   |
> | Fransız Güney Toprakları     | Niue     | Wallis veUçsuzuna   |
> | Gabon     | Norfolk Adası     | Yemen   |
> | Gambiya     | Kuzey Mariana Adaları     |    |
> | Cebelitarık     | Palau       |    |

## <a name="buy-software-subscriptions-on-behalf-of-customers"></a>Müşteriler adına yazılım abonelikleri satın alma

Bir müşteri adına yazılım abonelikleri satın almak için:

> [!NOTE]
> İş Ortağı Merkezi önizleme arabirimi, mantıksal olarak gruplu çalışma alanları aracılığıyla daha verimli ve üretken bir kullanıcı deneyimi sağlar. Çalışma alanları arabirimi ve nasıl açabilirsiniz hakkında daha fazla bilgi edinmek için [bkz. İş Ortağı Merkezi.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Çalışma alanları görünümü](#tab/workspaces-view)

1. İş Ortağı Merkezi oturum [açın](https://partner.microsoft.com/dashboard) ve Müşteriler **kutucuğunu** seçin.

2. Listeden bir müşteri seçin.

3. Müşterinin ayrıntı sayfasında Ürün ekle'yi **seçin** ve ardından ekrandaki yönergeleri izleyerek siparişinizi oluşturun ve ödemenizi bekleyin. Avustralya ve Brezilya dışındaki tüm ticari fiyatlandırmalar vergiyi dışlar. Avustralya ve Brezilya için fiyat vergiyi içerir.

#### <a name="current-view"></a>[Geçerli görünüm](#tab/current-view)

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard) oturum açın.

2. Yeni İş Ortağı Merkezi Müşteriler'i **ve** ardından listeden bir müşteri seçin.

3. Müşterinin ayrıntı sayfasında Ürün ekle'yi **seçin** ve ardından ekrandaki yönergeleri izleyerek siparişinizi oluşturun ve ödemenizi bekleyin. Avustralya ve Brezilya dışındaki tüm ticari fiyatlandırmalar vergiyi dışlar. Avustralya ve Brezilya için fiyat vergiyi içerir.

* * *

## <a name="activate-and-manage-software-subscriptions"></a>Yazılım aboneliklerini etkinleştirme ve yönetme

Yazılımınızı satın aldıktan sonra siz veya müşterileriniz indirmeniz gerekir (İş Ortağı Merkezi kullanan iş ortakları; Microsoft 365 Yönetici Merkezi kullanan müşteriler). Bunu yapmak için aşağıdaki yordamı kullanın. Bağlantı kopyalama ve yazılım indirme ile ilgili riskleri anlamak önemlidir. Daha fazla bilgi için Yeni **Ticaret İş Ortağı Merkezi** Kılavuzu'nda müşteri yazılım indirmelerini ve lisans anahtarlarını almak İş Ortağı Merkezi bkz. Müşteri yazılım indirmelerini ve lisans anahtarlarını almak için İş Ortağı Merkezi [kullanma.](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)

> [!NOTE]
> Anahtarların ve indirmelerin bağlantısını İş Ortağı Merkezi için yönetici aracınız olması gerekir.

1. Müşterinizin ayrıntı sayfasından Yazılım'ı **seçin.** Müşteri adına satın aldığınız tüm yazılımların listesini görüntülenir.

2. Ürün **sürümü, dil** **,** **bit** ve Anahtarları ve indirmeleri **al'ı seçin.** 

3. **32** basamaklı ürünü bir açılır iletişim kutusunda görüntülemek için Anahtarı Al'ı seçin. Bunu kopyalayıp müşteriye gönderebilirsiniz. 

4. Bitleri **indirmek** için İndir'i seçin. 

5. Bit **indirme** bağlantısını müşteriye göndermek için Bağlantıyı Kopyala'ya tıklayın. 

6. Ayrıca Yazılım **siparişini** iptal edebilir ve %100 kredi (30 günlük iptal ilkesi süresi içinde yapıldı ise) alırsınız.

> [!NOTE]
> Yalnızca müşteriler ürün anahtarlarını görebilir ve Microsoft 365 Yönetici Merkezi'nde (Genel Yönetici rolü gereklidir) bilgileri indirebilir. bu bilgileri görmek İş Ortağı Merkezi iş ortaklarının bu bilgileri kullanmaları gerekir.

> [!NOTE]
> CSP satın almaları, Birden Çok Etkinleştirme Anahtarı (MAK) aracılığıyla etkinleştirilir. Anahtar Yönetim Merkezi (KMS) anahtarlara izin verilmez. 

## <a name="move-a-customers-on-premises-license-from-vl-to-csp-with-no-downtime"></a>Müşterinin şirket içi lisansını kapalı kalma süresine gerek kalmadan VL'den CSP'ye taşıma

CSP KMS anahtarları mevcut değildir ancak yine de müşterinizin şirket içi lisanslarını VL'den CSP'ye taşımaya ve satın alma kanalı değiştirme nedeniyle kapalı kalma süresini önlemeye devam edersiniz. KMS istemcilere dağıtır ve genellikle cihaz bu etkinleştirmeyi yenilemeye çalışmadan önce 180 gün boyunca etkin kalırlar. Bu, cihazın zaten etkinleştirildikten sonra herhangi bir sorun ortaya çıktığında bir süre çalıştırılamayacak olduğu anlamına gelir. 

Müşteri bu süre boyunca yeni MAK'yi el ile veya betikli bir şekilde (kullanarak) dağıtırsa `slmgr.vbs` kapalı kalma süresi oluşmaz. Müşteri bu süre boyunca yeni MAK'yi dağıtmaz ve lisansı daha sonra yenilemeye çalışırsa, cihaz yeniden etkinleştirilene kadar bazı işlevlerde sınırlı olabilir veya engellenmiş olabilir. 

Daha fazla bilgi için Bkz. Windows 10 [(Windows 10) -](/windows/deployment/volume-activation/activate-windows-10-clients-vamt#key-management-service-activation-renewal)Windows Dağıtım çalıştıran istemcileri etkinleştirme. Bu dağıtım türüyle ilgili yardım için bir Teknik Ön Satış [ve Dağıtım hizmetleri isteği gönderebilirsiniz.](/partner-center/technical-benefits#submit-a-technical-presales-and-deployment-services-request)

## <a name="server-subscription-download-and-license-keys-available-through-microsoft-365-admin-center-for-customers"></a>Müşteriler için Microsoft 365 Yönetici Center aracılığıyla kullanılabilen sunucu aboneliği indirme ve lisans anahtarları 

Müşterileriniz CSP sunucusu abonelik lisans anahtarlarını ve indirmelerini Microsoft 365 Yönetici Center'dan edinebilirsiniz. CsP sunucusu abonelik lisans anahtarlarını ve indirmelerini görmek için müşterinin Microsoft 365 Yönetici Center > Faturalama > Ürünleriniz > **sekmesine gitmeleri gerekir.** Diğer ayrıntılar için Faturalama altındaki [Yazılım Sekmesine bakın.](/microsoft-365/admin/whats-new-in-preview#billing--subscriptions)  

## <a name="view-activity-for-software-key-access-and-software-downloads"></a>Yazılım anahtarı erişimi ve yazılım indirmeleri için etkinliği görüntüleme

Denetim veya uyumluluk amacıyla, Sunucu aboneliği yazılım anahtarlarına erişen veya Sunucu aboneliği yazılımını indiren kullanıcıların listesini denetlemeniz gerekir. Bu bilgilere erişmek için aşağıdaki yordamı kullanın. 

> [!NOTE]
> Bu etkinlik günlüklerini görmek Genel yönetici yöneticisi, Referans yöneticisi veya Pazarlama içeriği yöneticisi olmak gerekir.

1. İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard)

2. Veri dişlisi Ayarlar simgesini ve **ardından** Hesap Ayarlar'ı ve ardından Etkinlik **günlüğü'lerini seçin.**

3. Görmek istediğiniz etkinliğin tarih aralığını girin. Etkinlik günlüğü, belirttiğiniz süre boyunca yazılım anahtarlarına erişen veya yazılımı indiren kullanıcıların listesini görüntüler.

## <a name="cancel-a-purchase"></a>Satın alma işlemini iptal etme

Yazılım satın alma tarihini takip edinen 30 gün içinde yazılım satın alma işlemini iptal edebilirsiniz. Bu ilk 30 günlük süre içinde iptal edersiniz, erken sonlandırma ücreti ödemezsiniz. 30 gün sonra artık satın alma işlemini iptal etmenize gerek yoktur. (Bu iptal kuralına yönelik önemli kısıtlamalar için bkz. Not. Yazılım satın alma işlemini iptal etmenizden sonra ne olduğu hakkında bilgi edinmek için bu adımlardan sonra önemli nota da bakın.)

> [!NOTE]
> Satın alma işlemini iptal etmek için aşağıdaki adımlar yalnızca belirli bir iptal penceresi içinde iptal için uygun olan yazılımlar için geçerlidir( örneğin, satın alma sonrasındaki ilk 30 gün içinde). Bu adımlar, Azure'daki bir SUSE Linux veya RedHat yazılım planı için de geçerli değildir. Şu anda, bir SUSE veya RedHat yazılım planını iptal veya değiştirme işlemi olamaz. SUSE Linux [veya](/azure/virtual-machines/linux/prepay-suse-software-charges) RedHat planlarını kullanma hakkında daha fazla bilgi.

Satın alma işlemini iptal etmek için aşağıdaki adımları izleyin:

> [!NOTE]
> İş Ortağı Merkezi önizleme arabirimi, mantıksal olarak gruplu çalışma alanları aracılığıyla daha verimli ve üretken bir kullanıcı deneyimi sağlar. Çalışma alanları arabirimi ve nasıl açabilirsiniz hakkında daha fazla bilgi edinmek için [bkz. İş Ortağı Merkezi.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Çalışma alanları görünümü](#tab/workspaces-view)

> [!NOTE]
> Satın alma işlemini iptal etmek için Yönetici aracısı olmak gerekir. Aşağıdaki adımlarda, İş Ortağı Merkezi panosunda satın alma işleminin nasıl iptal İş Ortağı Merkezi anlatılacak. Bunu api'sini kullanarak da [İş Ortağı Merkezi.](/partner-center/develop/cancel-software-purchases)

1. İptal işlemini başlatmadan önce aşağıdaki bilgilere sahip olduğundan emin olun:

    - Müşterinin adı, kiracı GUID'si veya etki alanı adı
    - İptal etmek istediğiniz ürünün adı
    - Sipariş Kimliği

2. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard) oturum açın.

3. Müşteriler **kutucuğunu** ve ardından listeden bir müşteri seçin.

4. Müşterinin ayrıntılar sayfasında Yazılım'ı  seçerek müşteri için satın alınan yazılımların listesini görebilirsiniz. 

5. İptal etmek istediğiniz yazılım satın alma işlemini bulun ve İptal'i **seçin.** Bir iletişim kutusu görüntülenir.

6. Sipariş numarası açılan listesinden iptal etmek istediğiniz doğru sipariş kimliği numarasını seçin. (Müşterinin Sipariş geçmişi sayfasından sipariş veya sipariş kimliği numarası hakkında daha fazla **bilgi edinebilirsiniz.)**

7. İptalle ilgili Önemli iletiyi okuduğunızı kabul **etmek için** onay kutusunu seçin. (Satın alma işlemini **iptal etmenizden** sonra ne olduğu hakkında daha fazla bilgi edinmek için aşağıdaki Önemli nota bakın.)

8. Satın alma **işleminizi** iptal etmek için Gönder'i seçin. Bir müşteri için birden çok siparişi iptal etmek için her biri benzersiz sipariş kimliği numarası olan 4- 6. adımları tekrar gerçekleştirmeniz gerekir.

Bir siparişi iptal etmek için İş Ortağı Merkezi da (Sipariş numarası açılan listesinin altında görünen) başka bilgiler de verilmiştir. Bu bilgiler şunları içerebilir:

- Belirli bir siparişi iptal etmeniz için kaç gün kaldı?

- İptal penceresini zaten geçmiş olup olmadığı ve artık siparişi iptal edip etmeyememe

- İptal isteğiniz hakkında daha fazla bilgiye ihtiyacımız olursa size bir müşteri destek isteği formu **bağlantısı verilmiştir.**

> [!IMPORTANT]
> Siparişi iptal etmenizden sonra iptal işleminizi onaylayan bir ileti görüntülenir. Ancak iptalin panoda görünür olması 15 dakikaya kadar İş Ortağı Merkezi olabilir.

#### <a name="current-view"></a>[Geçerli görünüm](#tab/current-view)

> [!NOTE]
> Satın alma işlemini iptal etmek için Yönetici aracısı olmak gerekir. Aşağıdaki adımlarda, İş Ortağı Merkezi panosunda satın alma işleminin nasıl iptal İş Ortağı Merkezi açık açıklamadır. Bunu api'sini kullanarak da [İş Ortağı Merkezi.](/partner-center/develop/cancel-software-purchases)

1. İptal işlemini başlatmadan önce aşağıdaki bilgilere sahip olduğundan emin olun:

    - Müşterinin adı, kiracı GUID'si veya etki alanı adı
    - İptal etmek istediğiniz ürünün adı
    - Sipariş Kimliği

2. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard) oturum açın.

3. Yeni İş Ortağı Merkezi **Müşteriler'i** ve ardından listeden bir müşteri seçin.

4. Müşterinin ayrıntılar sayfasında Yazılım'ı  seçerek müşteri için satın alınan yazılımların listesini görebilirsiniz. 

5. İptal etmek istediğiniz yazılım satın alma işlemini bulun ve İptal'i **seçin.** Bir iletişim kutusu görüntülenir.

6. Sipariş numarası açılan listesinden iptal etmek istediğiniz doğru sipariş kimliği numarasını seçin. (Müşterinin Sipariş geçmişi sayfasından sipariş veya sipariş kimliği numarası hakkında daha fazla **bilgi edinebilirsiniz.)**

7. İptalle ilgili Önemli iletiyi okuduğunızı kabul **etmek için** onay kutusunu seçin. (Satın alma işlemini **iptal etmenizden** sonra ne olduğu hakkında daha fazla bilgi edinmek için aşağıdaki Önemli nota bakın.)

8. Satın alma **işleminizi** iptal etmek için Gönder'i seçin. Bir müşteri için birden çok siparişi iptal etmek için her biri benzersiz sipariş kimliği numarası olan 4- 6. adımları tekrar gerçekleştirmeniz gerekir.

Bir siparişi iptal etmek için İş Ortağı Merkezi da (Sipariş numarası açılan listesinin altında görünen) başka bilgiler de verilmiştir. Bu bilgiler şunları içerebilir:

- Belirli bir siparişi iptal etmeniz için kaç gün kaldı?

- İptal penceresini zaten geçmiş olup olmadığı ve artık siparişi iptal edip etmeyememe

- İptal isteğiniz hakkında daha fazla bilgiye ihtiyacımız olursa size bir müşteri destek isteği formu **bağlantısı verilmiştir.**

> [!IMPORTANT]
> Siparişi iptal etmenizden sonra iptal işleminizi onaylayan bir ileti görüntülenir. Ancak iptalin panoda görünür olması 15 dakikaya kadar İş Ortağı Merkezi olabilir.

* * *

### <a name="post-cancellation-details"></a>İptal sonrası ayrıntıları

Satın alma işlemini iptal etmenizden sonra:

- tüm ilgili yazılım anahtarları ve indirme bağlantıları iptal edilir. Bu iptal, siz ve müşterinizin bu satın alma işlemiyle ilgili yazılım anahtarlarını ve indirme bağlantılarını artık kullana anlamına gelir. İptal edilen tüm yazılımların kullanımdan kaldırılamandan siz ve müşteriniz sorumludur. Ayrıca iptal edilen yazılımı kaldırmak ve ilgili yazılım indirmelerini ve bağlantılarını kaldırmak sizin sorumluluğundadır.

- İptal edilen öğe müşterinin Yazılım ayrıntıları sayfasında görünmeye devam eder ancak etkinleştirme anahtarı kullanılamaz.

- sonraki aylık faturanıza iptal edilen sipariş için bir kredi görüntülenir. Kalıcı yazılım %100 kredi alır ve yazılım abonelikleri, prokratılmış kredi alır.

### <a name="submit-a-customer-support-request-to-cancel-a-purchase"></a>Satın alma işlemini iptal etmek için müşteri desteği isteği gönderme

İş Ortağı Merkezi aracılığıyla yazılım satın alma işlemini iptal etmeye çalıştıysanız ancak daha fazla bilgi sağlamanız ve bir müşteri destek isteği formunu doldurmanız söylense, bu adımlar size yardımcı olabilir:

1. Satın alma işlemini **iptal et penceresinden** müşteri desteği isteği bağlantısını seçerek Sorun bildir **İş Ortağı Merkezi** açılır.

2. Ayrıntılar **altında,** Sorun türü listesinde, müşteriler adına **CSP Satın Alma/Para İadesi'ne tıklayın.**

3. Etki ve Başlık alanlarını doldurun.

4. Açıklama alanında aşağıdaki bilgileri girin:

    - Müşteri kiracı GUID'si veya etki alanı adı
    - Sipariş Kimliği veya Abonelik Kimliği
    - Para iadesi nedeni
    - İstenen tutar

5. Kişi alanına adınız, e-posta adresinizi ve telefon numarasını girin.

6. Herhangi bir nedenle dosya eklemeniz gerekirse Dosya **ekle'yi seçin.** Bu adım isteğe bağlıdır.

7. Bitirdikten sonra Gönder'i **seçin.**

## <a name="next-steps"></a>Sonraki adımlar

- [İş Ortağı Merkezi aracılığıyla sipariş ve karşılama kılavuzu](https://partner.microsoft.com/resources/detail/guide-to-ordering-and-fulfillment-through-partner-center-pdf)
- [Müşterilere İş Ortağı Merkezi ticari market ürünlerine satış yapmak için abonelikleri kullanma](sell-marketplace-products.md)
- [Azure aboneliklerini müşterilere İş Ortağı Merkezi](assign-azure-subscriptions.md)
