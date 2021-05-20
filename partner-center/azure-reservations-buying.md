---
title: Müşteriler Microsoft Azure rezervasyonları satın alma
description: Azure rezervasyonlarını müşteriler adına satın almayı veya satın almayı öğrenin İş Ortağı Merkezi. Ayrıca Azure rezervasyonlarının kullanılamay olduğu pazarları listeler.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: cd8a78edab25b94e678aafd61ca96e61a625fb07
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149545"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Microsoft Azure müşterileriniz adına rezervasyon satın İş Ortağı Merkezi

**Uygun roller:** Yönetici aracısı | Genel yönetici | Yardım masası aracısı | Satış aracısı | Kullanıcı yönetimi yöneticisi

Bu makalede, azure rezervasyonlarını müşteriler adına satın alma veya satın alma hakkında İş Ortağı Merkezi. Ayrıca Azure rezervasyonlarının kullanıla olmadığı pazarları da tanımlar.
 
> [!NOTE]
> Bu makale yalnızca Bulut Çözümü Sağlayıcısı (CSP) programı iş ortakları için geçerlidir. Diğer abonelik türlerini (kullansanız öde, bireysel, Microsoft Müşteri Sözleşmesi veya Kurumsal Anlaşma abonelikler gibi) kullanan müşterilerin bu Azure rezervasyonları belgelerini [okuması gerekir.](/azure/cost-management-billing/reservations)

## <a name="before-you-begin"></a>Başlamadan önce

Müşterileriniz adına Azure rezervasyonları satın almadan önce aşağıdaki önemli bilgileri gözden geçirebilirsiniz. (Müşterilerin, onlar için satın aldığınız önceki bir Azure aboneliğinden kendi Azure rezervasyonlarını satın alamalarını istiyor musunuz? Bkz. [Müşterilere kendi Azure rezervasyonlarını satın alma izni verme.)](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations)

- Müşteriniz yeni aboneliği imzalarsa Microsoft Müşteri Sözleşmesi (bkz. Microsoft Müşteri Sözleşmesi [onaylayın),](confirm-customer-agreement.md)Azure planı kapsamında Azure rezervasyonları satın alasanız gerekir. Daha fazla bilgi için Azure [Planı satın alma makalelerini okuyun.](purchase-azure-plan.md)

- Müşteriler adına rezervasyon satın alamadan önce etkin bir Azure aboneliğine sahip olması gerekir
  
- SQL Veritabanı veya SUSE Linux yazılımı gibi yazılım aboneliği maliyetleri Azure rezervasyon fiyatlarına dahil değildir

- Konumunuz Brezilya değilse Microsoft'un sizin için ticari fiyatlandırması vergileri dahil değildir. Konumunuz Brezilya ise, uygun vergiler sizin için ticari fiyattır

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
> | Falkland Adaları     | Nauru     | ABD harici Adaları   |
> | Fransız Guyanası     | Yeni Kaledonya     | Vanuatu   |
> | Fransız Polinezyası     | Nijer     | Vatikan   |
> | Fransız Güney Toprakları     | Niue     | Wallis ve Futuna   |
> | Gabon     | Norfolk Adası     | Yemen   |
> | Gambiya     | Kuzey Mariana Adaları     |    |
> | Cebelitarık     | Palau       |    |

## <a name="purchase-azure-reservations"></a>Azure rezervasyonları satın alma

Iş Ortağı Merkezi 'nde müşterileriniz adına Microsoft Azure ayırmaları satın almak için aşağıdaki adımları izleyin. (Müşterilerin satın almış olduğunuz önceki bir Azure aboneliğinden kendi Azure ayırmalarını satın almasını ister misiniz? Bkz. [müşterilere kendi Azure ayırmalarını satın alma Izni verme](give-customers-permission.md).)

1. Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin.  

2. Müşteriler **sayfasında,** Azure rezervasyonları satın almak isteyen müşteriyi bulun ve ardından aşağı oku seçerek müşterinin satırı genişletin.  

3. Ürün **ekle'yi** ve ardından **Azure'ı seçin.** 

    a. Segment listesinden müşterinin pazar **segmentini** seçin.

    b. Ürün **Türü** listesinden **Rezervasyonlar'ı** seçin.

    c. Rezervasyon türü listesinden müşterinin istediği rezervasyon **türünü** seçin.

4. Azure rezervasyonları etkin bir Azure aboneliğiyle ilişkili olması gerekir. Müşteri aboneliği listesinden Azure rezervasyonlarını eklemek istediğiniz müşterinin **aboneliğini** seçin. 

   >[!IMPORTANT]
   >Müşterinin etkin bir Azure aboneliği yoksa Şimdi eklemek için **Azure'ı** seçin. 

5. Müşterinizin gereksinimlerini karşılayacak sanal makinelerde Azure rezervasyonlarını bulmak için filtreleri kullanın.  

6. Satın almak istediğiniz rezervasyonları buluduktan sonra müşterinin ihtiyacı olacak ayrılmış örnek sayısını **Miktar** alanına girin ve sepete **ekle'yi seçin.**  

7. Gerekli tüm öğeleri siparişe ekleyene kadar 5. ve 6. adımları tekrarlayın. Siparişinizin **doğru** olduğunu doğrulamak için Gözden geçir'i seçin.  

8. Siparişlerinizi **gözden geçirme** sayfasında şunları sebilirsiniz: 

    - Ayrılmış örnek miktarını doğrulayın veya değiştirme.

    - Rezervasyonun kapsamını seçin. Rezervasyonun kapsamı bir aboneliği veya birden çok aboneliği (paylaşılan kapsam) kapsıyor olabilir. Rezervasyonun kapsamını tek bir abonelik olarak kapsamına asanız, rezervasyon indirimi yalnızca bu aboneliğe uygulanır. Paylaşılan'ı seçmeniz durumunda rezervasyon indirimi müşterinin faturalama bağlamındaki tüm aboneliklere uygulanır. 

      >[!NOTE] 
      >Rezervasyonun kapsamını tek bir Azure aboneliğiyle sınırlamayı tercih ediyorsanız aboneliğin vCPU kotasını artırmanız gerekir. Aboneliğin vCPU kotasını artırmak için abonelikte bir destek isteği oluşturmanız Azure portal. İsteği oluşturmak için [Bu konudaki](/azure/azure-supportability/resource-manager-core-quotas-request) yönergeleri izleyin. 

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
|Müşterilere kendi Azure ayırmalarını satın alma izni verme  | [Müşterilere kendi Azure rezervasyonlarını satın alma izni verme](give-customers-permission.md)  |