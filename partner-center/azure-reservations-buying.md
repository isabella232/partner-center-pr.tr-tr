---
title: Müşteriler için Microsoft Azure ayırmaları satın alın
description: Iş Ortağı Merkezi 'nde müşterileriniz adına Azure ayırmaları satın almayı veya satın almayı öğrenin. Ayrıca, Azure ayırmalarının kullanılamadığı pazarları listeler.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: 0e81a9561f3749aab281bb4ebd7cd0c38540ff31
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534616"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Iş Ortağı Merkezi 'nde müşterileriniz adına Microsoft Azure ayırmaları satın alın

**Uygun roller**

- Yönetim Aracısı
- Genel yönetici
- Yardım Masası Aracısı
- Satış Aracısı
- Kullanıcı Yönetimi Yöneticisi

Bu makalede, Iş Ortağı Merkezi 'nde müşterileriniz adına Azure ayırmaları satın alma veya satın alma işlemleri açıklanmaktadır. Ayrıca, Azure ayırmalarının kullanılamadığı pazarları tanımlar.
 
> [!NOTE]
> Bu makale yalnızca bulut çözümü sağlayıcısı (CSP) programındaki iş ortakları için geçerlidir. Diğer abonelik türleri (örneğin, Kullandıkça öde, bireysel, Microsoft Müşteri Sözleşmesi veya Kurumsal Anlaşma abonelikleri) kullanan müşteriler [Bu Azure ayırmaları belgelerini](/azure/cost-management-billing/reservations)okumalı olmalıdır.

## <a name="before-you-begin"></a>Başlamadan önce

Müşterileriniz adına Azure ayırmaları satın almadan önce aşağıdaki önemli bilgileri gözden geçirin. (Müşterilerin satın almış olduğunuz önceki bir Azure aboneliğinden kendi Azure ayırmalarını satın almasını ister misiniz? Bkz. [müşterilere kendi Azure ayırmalarını satın alma Izni verme](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations).)

- Müşteriniz yeni Microsoft Müşteri sözleşmesini imzaladığında (bkz [. Microsoft Müşteri sözleşmesinin müşteri kabulünü onaylama](confirm-customer-agreement.md)), Azure rezervasyonlarını Azure planı kapsamında satın almalısınız. Daha fazla bilgi için [satın alma Azure planını](purchase-azure-plan.md)okuyun.

- Müşteriler adına ayırmaları satın alabilmek için önce etkin bir Azure aboneliğine sahip olmaları gerekir
  
- SQL veritabanı veya SUSE Linux yazılımı gibi yazılım abonelik maliyetleri, Azure rezervasyon fiyatlarına dahil değildir

- Microsoft 'un ticari fiyatlandırmasına, konumunuz Brezilya dışında vergiler dahil değildir. Konumunuz Brezilya ise, sizin için ticari fiyat uygun vergileri içerir

- Satış ve yardım masası aracılarının Azure aboneliğine açık erişimi olması gerekir ve bu sayede, bu kullanıcı adına, değiş tokuş ve para iadesi dahil olmak üzere Azure portal ve dosya desteği taleplerini satın alabilir veya yönetebilir.  

- Dolaylı bir Sağlayıcıysanız ve Azure ayırmaları Azure portal aracılığıyla satın alırsanız, kayıt ortağı (dolaylı satıcı) seçtiğiniz Azure CSP aboneliğinden devralınır.

- Azure ayırmaları için kayıt ortağı, satın alma sonrası değiştirilemez. Mevcut ayırmayı iptal edebilir ve yeni kayıt ortağıyla yeni bir tane satın alabilirsiniz.

- Bir müşteri, bir Azure aboneliğini doğrudan veya EA 'dan CSP 'ye aktarmak isterse, ayırmalar aktarılmaz.

## <a name="azure-reservations-unavailable-markets"></a>Azure ayırmaları kullanılamayan pazarlar

> [!IMPORTANT]
> Azure ayırmaları **aşağıdaki pazarlarda kullanılamaz:**  
>  
> **Kullanılamayan pazarlar (alfabetik sırada)**
>
> |A-GI   | Gr-PAL  | PAP-Z |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | Bir i Adaları     | Grönland     | Papua Yeni Gine     |
> | Amerikan Samoası     | Grenada     | Pitcairn Adaları     |
> | Andorra     | Guadeloupe     | Reunion     |
> | Anguilla     | Guam     | Saba   |
> | Antarktika     | Guernsey     | Saint Barthélimy   |
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
> | Falkland Adaları     | Nauru     | ABD Küçük Harici Adaları   |
> | Fransız Guyanası     | Yeni Kaledonya     | Vanuatu   |
> | Fransız Polinezyası     | Nijer     | Vatikan   |
> | Fransız Güney Toprakları     | Niue     | Wallis ve Futuna   |
> | Gabon     | Norfolk Adası     | Yemen   |
> | Gambiya     | Kuzey Mariana Adaları     |    |
> | Cebelitarık     | Palau       |    |

## <a name="purchase-azure-reservations"></a>Azure ayırmaları satın alma

Iş Ortağı Merkezi 'nde müşterileriniz adına Microsoft Azure ayırmaları satın almak için aşağıdaki adımları izleyin. (Müşterilerin satın almış olduğunuz önceki bir Azure aboneliğinden kendi Azure ayırmalarını satın almasını ister misiniz? Bkz. [müşterilere kendi Azure ayırmalarını satın alma Izni verme](give-customers-permission.md).)

1. Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin.  

2. **Müşteriler** sayfasında, Azure ayırmaları satın almak isteyen müşteriyi bulun ve ardından müşterinin satırını genişletmek için aşağı oku seçin.  

3. **Ürün Ekle** ' yi seçin ve ardından **Azure**' u seçin. 

    a. **Segment** listesinden müşterinin pazar segmentini seçin.

    b. Ürün **türü** listesinden **ayırmalar** ' ı seçin.

    c. Müşterinin rezervasyon **türü** listesinden istediği rezervasyon türünü seçin.

4. Azure ayırmaları etkin bir Azure aboneliğiyle ilişkilendirilmelidir. **Müşteri aboneliği** listesinden, Azure ayırmaları eklemek istediğiniz müşterinin aboneliğini seçin. 

   >[!IMPORTANT]
   >Müşterinin zaten etkin bir Azure aboneliği yoksa, şimdi bir tane eklemek için **Azure** ' ı seçin. 

5. Müşterilerinizin gereksinimlerini karşılayan sanal makinelerde Azure ayırmaları bulmak için filtreleri kullanın.  

6. Satın almak istediğiniz ayırmaları bulduktan sonra, müşterinin **Miktar** halinde ihtiyaç duyduğu ayrılmış örnek sayısını girin ve ardından **Sepete Ekle**' yi seçin.  

7. Gerekli tüm öğeleri sıraya ekleyinceye kadar 5 ve 6. adımları tekrarlayın. Siparişinizin doğru olduğunu doğrulamak için **gözden geçir** ' i seçin.  

8. **Siparişlerinizi gözden geçirin** sayfasında şunları yapabilirsiniz: 

    - Ayrılmış örnek miktarını doğrulayın veya değiştirin.

    - Rezervasyonun kapsamını seçin. Ayırma kapsamı bir aboneliği veya birden çok aboneliği (paylaşılan kapsamı) kapsayabilir. Ayırmayı tek bir aboneliğe göre kapsamınızda, rezervasyon iskontosu yalnızca bu aboneliğe uygulanır. Paylaşılan ' i seçerseniz, rezervasyon indirimi müşterinin faturalandırma bağlamındaki tüm aboneliklere uygulanır. 

      >[!NOTE] 
      >Ayırmanın kapsamını tek bir Azure aboneliğiyle sınırlandırmayı tercih ediyorsanız, aboneliğin vCPU kotasını artırmanız gerekebilir. Aboneliğin vCPU kotasını artırmak için Azure portal bir destek isteği oluşturmanız gerekir. İsteği oluşturmak için [Bu konudaki](/azure/azure-supportability/resource-manager-core-quotas-request) yönergeleri izleyin. 

      >[!NOTE]   
      >Müşteriniz Azure planının altındaysa, **kapsam** **paylaşılan** olarak ayarlanır. 

    - Sağlayıcı iş ortağıysanız, ürünle ilişkilendirmek istediğiniz Bayi ' ı seçin.
    
    - Azure rezervasyon, faturalandırma planı seçeneğini destekliyorsa, açılan menüden fatura sıklığını aylık olarak seçebilirsiniz. 
    - Azure rezervasyon, faturalandırma planı seçeneğini desteklemiyorsa faturalandırma sıklığınız varsayılan olarak bir kerelik faturalandırmaya göre yapılır. 

9. Siparişi satın almak için **satın al** ' ı seçin. Sipariş numaranız dahil olmak üzere siparişinizin ayrıntıları **Onayla** sayfasında görüntülenir. **Sipariş geçmişi** sayfanıza gitmek için **bitti** ' yi seçin. 

10. Müşterinin ayırmasını Azure portal yönetmek için **müşteriler** sayfasında müşteriyi bulun ve ardından müşterinin satırını genişletmek için aşağı oku seçin. **Microsoft Azure yönetim portalı** ' yi seçerek müşterinin kaydını Azure Portal açın.

## <a name="next-steps"></a>Sonraki adımlar

|**Hakkında bilgi için**   |**Bunu okuyun**    |
|:-----------------------------|:-----------------|
|CSP 'de Azure ayırmaları genel bakış  | [Ayrılmış Microsoft Azure örnekleri satma](azure-reservations.md) |
|Azure ayırmalarını Iş Ortağı Merkezi 'nde yönetme | [Azure ayırmalarını Iş Ortağı Merkezi 'nde yönetme](azure-reservations-manage.md)
|Doğru VM boyutunu belirleme ve müşteri VM kullanımını doğrulama   |[Maksimum Azure ayırma kullanımı için VM boyutu](azure-usage.md)   |
|Iş Ortağı Merkezi API 'sini kullanarak Azure ayırmaları satın alma | [Azure ayrılmış VM örneklerini](/partner-center/develop/purchase-azure-reservations) Iş Ortağı Merkezi geliştirici belgelerinde satın alma   |
|Müşterilere kendi Azure ayırmalarını satın alma izni verme  | [Müşterilere kendi Azure ayırmalarını satın alma izni verin](give-customers-permission.md)  |