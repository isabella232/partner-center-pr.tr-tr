---
title: müşteriler için Microsoft Azure ayırmaları satın alın
description: Iş Ortağı Merkezi 'nde müşterileriniz adına Azure ayırmaları satın almayı veya satın almayı öğrenin. Ayrıca, Azure ayırmalarının kullanılamadığı pazarları listeler.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: 112296baffe38b81a1a0516e62fa31525d1e3b3d
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123959994"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>iş ortağı merkezi 'nde müşterileriniz adına Microsoft Azure ayırmaları satın alın

**Uygun roller**: yönetici Aracısı | Genel yönetici | Yardım Masası Aracısı | Satış Aracısı | Kullanıcı Yönetimi Yöneticisi

Bu makalede, Iş Ortağı Merkezi 'nde müşterileriniz adına Azure ayırmaları satın alma veya satın alma işlemleri açıklanmaktadır. Ayrıca, Azure ayırmalarının kullanılamadığı pazarları tanımlar.
 
> [!NOTE]
> bu makale yalnızca Bulut Çözümü Sağlayıcısı (CSP) programındaki iş ortakları için geçerlidir. diğer abonelik türleri (örneğin, kullandıkça öde, bireysel, Microsoft müşteri sözleşmesi veya Kurumsal Anlaşma abonelikleri) kullanan müşteriler [bu Azure ayırmaları belgelerini](/azure/cost-management-billing/reservations)okumalı olmalıdır.

## <a name="before-you-begin"></a>Başlamadan önce

Müşterileriniz adına Azure ayırmaları satın almadan önce aşağıdaki önemli bilgileri gözden geçirin. (Müşterilerin satın almış olduğunuz önceki bir Azure aboneliğinden kendi Azure ayırmalarını satın almasını ister misiniz? Bkz. [müşterilere kendi Azure ayırmalarını satın alma Izni verme](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations).)

- Müşteriniz yeni Microsoft Müşteri sözleşmesini imzaladığında (bkz [. Microsoft Müşteri sözleşmesinin müşteri kabulünü onaylama](confirm-customer-agreement.md)), Azure rezervasyonlarını Azure planı kapsamında satın almalısınız. Daha fazla bilgi için [satın alma Azure planını](purchase-azure-plan.md)okuyun.

- Müşteriler adına ayırmaları satın alabilmek için önce etkin bir Azure aboneliğine sahip olmaları gerekir
  
- SQL Veritabanı veya SUSE Linux yazılımı gibi yazılım abonelik maliyetleri, Azure rezervasyon fiyatlarına dahil değildir

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

## <a name="purchase-azure-reservations"></a>Azure rezervasyonları satın alma

Aşağıdaki adımları takip edin ve Microsoft Azure rezervasyonları müşterileriniz adına satın İş Ortağı Merkezi. (Müşterilerin, onlar için satın aldığınız önceki bir Azure aboneliğinden kendi Azure rezervasyonlarını satın alamalarını istiyor musunuz? Bkz. [Müşterilere kendi Azure rezervasyonlarını satın alma izni verme.)](give-customers-permission.md)

1. İş Ortağı Merkezi  menüsünden Müşteriler'i seçin.  

2. Müşteriler **sayfasında,** Azure rezervasyonları satın almak isteyen müşteriyi bulun ve ardından aşağı oku seçerek müşterinin satırı genişletin.  

3. Ürün **ekle'yi** ve ardından **Azure'ı seçin.** 

    a. Segment listesinden müşterinin pazar **segmentini** seçin.

    b. Ürün **Türü** listesinden **Rezervasyonlar'ı** seçin.

    c. Rezervasyon türü listesinden müşterinin istediği rezervasyon **türünü** seçin.

4. Azure rezervasyonlarının etkin bir Azure aboneliğiyle ilişkilendirilmiş olması gerekir. Müşteri aboneliği listesinden Azure rezervasyonlarını eklemek istediğiniz müşterinin **aboneliğini** seçin. 

   >[!IMPORTANT]
   >Müşterinin etkin bir Azure aboneliği yoksa Şimdi eklemek için **Azure'ı** seçin. 

5. Müşterinizin gereksinimlerini karşılayacak sanal makinelerde Azure rezervasyonlarını bulmak için filtreleri kullanın.  

6. Satın almak istediğiniz rezervasyonları buluduktan sonra müşterinin ihtiyacı olacak ayrılmış örnek sayısını **Miktar** alanına girin ve sepete **ekle'yi seçin.**  

7. Gerekli tüm öğeleri siparişe ekleyene kadar 5. ve 6. adımları tekrarlayın. Siparişinizin **doğru** olduğunu doğrulamak için Gözden geçir'i seçin.  

8. Siparişlerinizi **gözden geçirme** sayfasında şunları sebilirsiniz: 

    - Ayrılmış örnek miktarını doğrulayın veya değiştirme.

    - Rezervasyonun kapsamını seçin. Rezervasyonun kapsamı bir aboneliği veya birden çok aboneliği (paylaşılan kapsam) kapsıyor olabilir. Rezervasyonun kapsamını tek bir abonelik olarak kapsamına asanız, rezervasyon indirimi yalnızca bu aboneliğe uygulanır. Paylaşılan'ı seçmeniz durumunda rezervasyon indirimi müşterinin faturalama bağlamındaki tüm aboneliklere uygulanır. 

      >[!NOTE] 
      >Rezervasyonun kapsamını tek bir Azure aboneliğiyle sınırlamayı tercih ediyorsanız aboneliğin vCPU kotasını artırmanız gerekir. Aboneliğin vCPU kotasını artırmak için abonelikte bir destek isteği Azure portal. İsteği oluşturmak [için bu konudaki](/azure/azure-supportability/resource-manager-core-quotas-request) yönergeleri izleyin. 

      >[!NOTE]   
      >Müşteriniz Azure planı kapsamında ise **Kapsam, Paylaşılan** olarak **ayarlanır.** 

    - Sağlayıcı iş ortağıysanız ürünle ilişkilendirmek istediğiniz kurumsal bayiyi seçin.
    
    - Azure rezervasyonunuz Faturalama planı seçeneğini destekliyorsa açılan menüden faturalama sıklığını aylık olarak seçebilirsiniz. 
    - Azure rezervasyonunuz Faturalama planı seçeneğini desteklemezse faturalama sıklığınız varsayılan olarak bir kez faturalama olur. 

9. Siparişi **satın almak** için Satın Al'ı seçin. Sipariş numaranız da dahil olmak üzere siparişinizin ayrıntıları Onayla **sayfasında** görüntülenir. **Bitti'yi** seçerek Sipariş **geçmişi sayfanıza** gidin. 

10. Müşterinin rezervasyonunu Azure portal için Müşteriler sayfasında müşteriyi bulun ve  aşağı oku seçerek müşterinin satırı genişletin. **Microsoft Azure Yönetim Portalı'ı** seçerek müşterinin kaydını Azure portal.

## <a name="next-steps"></a>Sonraki adımlar

|**Hakkında bilgi için**   |**Bunu okuyun**    |
|:-----------------------------|:-----------------|
|CSP'de Azure rezervasyonları genel bakış  | [Ayrılmış Microsoft Azure Satış](azure-reservations.md) |
|Azure rezervasyonlarını İş Ortağı Merkezi | [Azure rezervasyonlarını İş Ortağı Merkezi](azure-reservations-manage.md)
|Doğru VM boyutunu belirleme ve müşteri VM kullanımını doğrulama   |[Maksimum Azure rezervasyon kullanımı için VM boyutlandırması](azure-usage.md)   |
|İş Ortağı Merkezi API'sini kullanarak Azure rezervasyonları satın alma | [İş Ortağı Merkezi geliştirici](/partner-center/develop/purchase-azure-reservations) belgelerinde Azure Ayrılmış VM Örnekleri satın alma   |
|Müşterilere kendi Azure rezervasyonlarını satın alma izni verme  | [Müşterilere kendi Azure rezervasyonlarını satın alma izni verme](give-customers-permission.md)  |