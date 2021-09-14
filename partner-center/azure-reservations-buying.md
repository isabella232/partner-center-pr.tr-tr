---
title: Müşteriler Microsoft Azure rezervasyonları satın alma
description: Bu hizmetlerde müşterileriniz adına Azure rezervasyonları satın almayı veya satın İş Ortağı Merkezi. Ayrıca Azure rezervasyonlarının kullanılamay olduğu pazarları listeler.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: 112296baffe38b81a1a0516e62fa31525d1e3b3d
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248336"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Microsoft Azure müşterileriniz adına rezervasyon satın İş Ortağı Merkezi

**Uygun roller:** Yönetici aracısı | Genel yönetici | Yardım masası aracısı | Satış aracısı | Kullanıcı yönetimi yöneticisi

Bu makalede, azure'da müşterileriniz adına Azure rezervasyonları satın alma veya satın alma İş Ortağı Merkezi. Ayrıca Azure rezervasyonlarının kullanıla olmadığı pazarları da tanımlar.
 
> [!NOTE]
> Bu makale yalnızca Bulut Çözümü Sağlayıcısı (CSP) programı iş ortakları için geçerlidir. Diğer abonelik türlerini (kullansanız öde, bireysel, Microsoft Müşteri Sözleşmesi veya Kurumsal Anlaşma abonelikler gibi) kullanan müşterilerin bu Azure rezervasyonları belgelerini [okuması gerekir.](/azure/cost-management-billing/reservations)

## <a name="before-you-begin"></a>Başlamadan önce

Müşterileriniz adına Azure rezervasyonları satın almadan önce aşağıdaki önemli bilgileri gözden geçirebilirsiniz. (Müşterilerin, onlar için satın aldığınız önceki Bir Azure aboneliğinden kendi Azure rezervasyonlarını satın alamalarını istiyor musunuz? Bkz. [Müşterilere kendi Azure rezervasyonlarını satın alma izni verme.)](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations)

- Müşteriniz yeni aboneliği imzalarsa Microsoft Müşteri Sözleşmesi (bkz. Microsoft Müşteri Sözleşmesi [onaylayın),](confirm-customer-agreement.md)Azure planı kapsamında Azure rezervasyonları satın alasanız gerekir. Daha fazla bilgi için Azure [planı satın alma makalelerini okuyun.](purchase-azure-plan.md)

- Müşteriler adına rezervasyon satın alamadan önce etkin bir Azure aboneliğine sahip olması gerekir
  
- SQL Veritabanı veya SUSE Linux yazılımı gibi yazılım aboneliği maliyetleri Azure rezervasyon fiyatlarına dahil değildir

- Konumunuz Brezilya değilse Microsoft'un sizin için ticari fiyatlandırması vergileri dahil değildir. Konumunuz Brezilya ise, uygun vergiler sizin için ticari fiyattır

- Satış ve yardım masası temsilcilerinin Azure aboneliğini müşteri adına satın al Azure portal ve dosya desteği isteklerinde (değişimler ve para iadeleri de dahil) yönetecekleri açık erişime ihtiyacı vardır  

- Dolaylı sağlayıcıysanız ve Azure portal aracılığıyla Azure rezervasyonları satın alıyorsanız, Kayıt İş Ortağı (dolaylı kurumsal bayi) Azure CSP aboneliğinden devralınmış olur.

- Azure rezervasyonları için Kayıt İş Ortağı, satın alma sonrası değiştirilemez. Mevcut rezervasyonu iptal edebilir ve yeni Kayıt İş Ortağı ile yeni bir rezervasyon satın alın.

- Müşteri Azure aboneliğini Doğrudan veya EA'dan CSP'ye aktarmayı istiyorsa rezervasyonlar aktarlanmaz.

## <a name="azure-reservations-unavailable-markets"></a>Azure rezervasyonları kullanılamayan pazarlar

> [!IMPORTANT]
> Azure **rezervasyonları aşağıdaki** pazarlarda kullanılamaz:  
>  
> **Kullanılamayan pazarlar (alfabetik sırada)**
>
> |A'dan Gi'ye   | Gr to Pal  | Pap'dan Z'ye |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | Åland Adaları     | Grönland     | Papua Yeni Gine     |
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
> | Bouvet Adası     | Jan Mayen     | Séo Tomé ve Préncipe   |
> | Britanya Hint Okyanusu Toprakları       | Jersey     | Seyşeller   |
> | Britanya Virjin Adaları     | Kiribati       | Sierra Leone   |
> | Burkina Faso     | Kosova     | Sint Eustatius     |
> | Burundi     | Laos     | Sint Maarten     |
> | Kamboçya     | Lesotho     | Solomon Adaları     |
> | Orta Afrika Cumhuriyeti     | Liberya     | Somali     |
> | Çad     | Madagaskar     | Güney Georgia ve Güney Sandwich Adaları     |
> | Çin     | Malavi     | Güney Sudan     |
> | Christmas Adası     | Maldivler     | St Helena, Ascension, Tristan da Cunha     |
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

iş ortağı merkezi 'nde müşterileriniz adına Microsoft Azure ayırmaları satın almak için aşağıdaki adımları izleyin. (Müşterilerin satın almış olduğunuz önceki bir Azure aboneliğinden kendi Azure ayırmalarını satın almasını ister misiniz? Bkz. [müşterilere kendi Azure ayırmalarını satın alma Izni verme](give-customers-permission.md).)

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

10. Müşterinin ayırmasını Azure portal yönetmek için **müşteriler** sayfasında müşteriyi bulun ve ardından müşterinin satırını genişletmek için aşağı oku seçin. müşterinin kaydını Azure portal açmak için **Microsoft Azure Yönetim Portalı** seçin.

## <a name="next-steps"></a>Sonraki adımlar

|**Hakkında bilgi için**   |**Bunu okuyun**    |
|:-----------------------------|:-----------------|
|CSP 'de Azure ayırmaları genel bakış  | [ayrılmış Microsoft Azure örnekleri satma](azure-reservations.md) |
|Azure ayırmalarını Iş Ortağı Merkezi 'nde yönetme | [Azure ayırmalarını Iş Ortağı Merkezi 'nde yönetme](azure-reservations-manage.md)
|Doğru VM boyutunu belirleme ve müşteri VM kullanımını doğrulama   |[Maksimum Azure ayırma kullanımı için VM boyutu](azure-usage.md)   |
|Iş Ortağı Merkezi API 'sini kullanarak Azure ayırmaları satın alma | [Azure ayrılmış VM örneklerini](/partner-center/develop/purchase-azure-reservations) Iş Ortağı Merkezi geliştirici belgelerinde satın alma   |
|Müşterilere kendi Azure ayırmalarını satın alma izni verme  | [Müşterilere kendi Azure ayırmalarını satın alma izni verin](give-customers-permission.md)  |