---
title: Müşteriler Microsoft Azure rezervasyonları satın alma
description: Azure rezervasyonlarını müşteriler adına satın almayı veya satın almayı İş Ortağı Merkezi. Ayrıca Azure rezervasyonlarının kullanılamay olduğu pazarları listeler.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: 112296baffe38b81a1a0516e62fa31525d1e3b3d
ms.sourcegitcommit: 90bf27df911b428b1222f483c32ba6367870e7c5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/04/2021
ms.locfileid: "115102430"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Microsoft Azure müşterileriniz adına rezervasyon satın İş Ortağı Merkezi

**Uygun roller:** Yönetici aracısı | Genel yönetici | Yardım masası aracısı | Satış aracısı | Kullanıcı yönetimi yöneticisi

Bu makalede, azure rezervasyonlarını müşteriler adına satın alma veya satın alma hakkında İş Ortağı Merkezi. Ayrıca Azure rezervasyonlarının kullanıla olmadığı pazarları da tanımlar.
 
> [!NOTE]
> Bu makale yalnızca Bulut Çözümü Sağlayıcısı (CSP) programı iş ortakları için geçerlidir. Diğer abonelik türlerini (kullansanız öde, bireysel, Microsoft Müşteri Sözleşmesi veya Kurumsal Anlaşma abonelikler gibi) kullanan müşterilerin bu Azure rezervasyonları belgelerini [okuması gerekir.](/azure/cost-management-billing/reservations)

## <a name="before-you-begin"></a>Başlamadan önce

Müşterileriniz adına Azure rezervasyonları satın almadan önce aşağıdaki önemli bilgileri gözden geçirebilirsiniz. (Müşterilerin, onlar için satın aldığınız önceki Bir Azure aboneliğinden kendi Azure rezervasyonlarını satın alamalarını istiyor musunuz? Bkz. [Müşterilere kendi Azure rezervasyonlarını satın alma izni verme.)](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations)

- Müşteriniz yeni aboneliği imzalarsa Microsoft Müşteri Sözleşmesi (bkz. Microsoft Müşteri Sözleşmesi [onaylayın),](confirm-customer-agreement.md)Azure planı kapsamında Azure rezervasyonları satın alasanız gerekir. Daha fazla bilgi için Azure [planı satın alma makalelerini okuyun.](purchase-azure-plan.md)

- Müşteriler adına rezervasyon satın alamadan önce etkin bir Azure aboneliğine sahip olması gerekir
  
- SQL Veritabanı veya SUSE Linux yazılımı gibi yazılım aboneliği maliyetleri Azure rezervasyon fiyatlarına dahil değildir

- Konumunuz Brezilya değilse Microsoft'un sizin için ticari fiyatlandırması vergileri dahil değildir. Konumunuz Brezilya ise, uygun vergiler sizin için ticari fiyattır

- Satış ve yardım masası temsilcilerinin Azure aboneliğini müşteri adına satın al Azure portal ve dosya desteği isteklerinde (değişimler ve para iadeleri dahil) yönetecekleri açık erişime sahip ihtiyaçları vardır  

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
> | Falkland Adaları     | Nauru     | ABD'de Outlying Adaları   |
> | Fransız Guyanası     | Yeni Kaledonya     | Vanuatu   |
> | Fransız Polinezyası     | Nijer     | Vatikan   |
> | Fransız Güney Toprakları     | Niue     | Wallis veUçsuzuna   |
> | Gabon     | Norfolk Adası     | Yemen   |
> | Gambiya     | Kuzey Mariana Adaları     |    |
> | Cebelitarık     | Palau       |    |

## <a name="purchase-azure-reservations"></a>Azure rezervasyonları satın alma

Aşağıdaki adımları takip edin ve Microsoft Azure müşteri adına rezervasyon satın İş Ortağı Merkezi. (Müşterilerin, onlar için satın aldığınız önceki Bir Azure aboneliğinden kendi Azure rezervasyonlarını satın alamalarını istiyor musunuz? Bkz. [Müşterilere kendi Azure rezervasyonlarını satın alma izni verme.)](give-customers-permission.md)

1. İş Ortağı Merkezi  menüsünden Müşteriler'i seçin.  

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

    - Rezervasyonun kapsamını seçin. Rezervasyonun kapsamı bir veya birden çok aboneliği (paylaşılan kapsam) kapsıyor olabilir. Rezervasyonun kapsamını tek bir abonelik olarak kapsamına asanız, rezervasyon indirimi yalnızca bu aboneliğe uygulanır. Paylaşılan'ı seçmeniz durumunda rezervasyon indirimi müşterinin faturalama bağlamındaki tüm aboneliklere uygulanır. 

      >[!NOTE] 
      >Rezervasyonun kapsamını tek bir Azure aboneliğiyle sınırlamayı tercih ediyorsanız aboneliğin vCPU kotasını artırmanız gerekir. Aboneliğin vCPU kotasını artırmak için abonelikte bir destek isteği oluşturmanız Azure portal. İsteği oluşturmak [için bu konudaki](/azure/azure-supportability/resource-manager-core-quotas-request) yönergeleri izleyin. 

      >[!NOTE]   
      >Müşteriniz Azure planı kapsamında ise **Kapsam, Paylaşılan** olarak **ayarlanır.** 

    - Sağlayıcı iş ortağıysanız ürünle ilişkilendirmek istediğiniz kurumsal bayiyi seçin.
    
    - Azure rezervasyonunuz Faturalama planı seçeneğini destekliyorsa açılan menüden faturalama sıklığını aylık olarak seçebilirsiniz. 
    - Azure rezervasyonunuz Faturalama planı seçeneğini desteklemezse, faturalama sıklığınız varsayılan olarak bir kez faturalama olur. 

9. Siparişi **satın almak** için Satın Al'ı seçin. Sipariş numaranız da dahil olmak üzere siparişinizin ayrıntıları Onayla **sayfasında** görüntülenir. Sipariş **geçmişi** sayfanıza gitmek için **Bitti'yi** seçin. 

10. Müşterinin rezervasyonunu Azure portal için Müşteriler sayfasında müşteriyi bulun  ve aşağı oku seçerek müşterinin satırı genişletin. **Microsoft Azure Yönetim Portalı'yi** seçerek müşterinin kaydını Azure portal.

## <a name="next-steps"></a>Sonraki adımlar

|**Hakkında bilgi için**   |**Bunu okuyun**    |
|:-----------------------------|:-----------------|
|CSP'de Azure rezervasyonları genel bakış  | [Ayrılmış Microsoft Azure Satış](azure-reservations.md) |
|Azure rezervasyonlarını İş Ortağı Merkezi | [Azure rezervasyonlarını İş Ortağı Merkezi](azure-reservations-manage.md)
|Doğru VM boyutunu belirleme ve müşteri VM kullanımını doğrulama   |[Maksimum Azure rezervasyon kullanımı için VM boyutlandırması](azure-usage.md)   |
|İş Ortağı Merkezi API'sini kullanarak Azure rezervasyonları satın alma | [Geliştirici Azure Ayrılmış VM Örnekleri](/partner-center/develop/purchase-azure-reservations) belgelerinde İş Ortağı Merkezi satın alma   |
|Müşterilere kendi Azure rezervasyonlarını satın alma izni verme  | [Müşterilere kendi Azure rezervasyonlarını satın alma izni verme](give-customers-permission.md)  |