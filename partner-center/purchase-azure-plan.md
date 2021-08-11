---
title: Azure planı satın alma
ms.topic: how-to
ms.date: 07/21/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Azure planını kullanarak, tek veya birden çok Azure aboneliği satın almayı, Azure ayırmalarını, kaynakları yapılandırmayı ve abonelikleri görüntülemeyi veya eklemeyi öğrenin.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: af098c9ef57a9a40badded40cb457f8c8fd4855185ae6f10dfb71e51689994ea
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115693936"
---
# <a name="purchase-the-azure-plan-for-customers-and-access-the-latest-azure-services"></a>Müşteriler için Azure planı satın alın ve en son Azure hizmetlerine erişin

**Uygulama hedefi**: Iş Ortağı Merkezi 

**Uygun roller**: genel yönetici | Kullanıcı Yönetimi Yöneticisi | Satış Aracısı

Microsoft Müşteri Sözleşmesi kapsamında müşterileriniz için bir Azure planı satın aldığınızda, Kullandıkça Öde tarifesine en son Azure hizmetlerinin tam kataloğuna erişebilirsiniz. Bulut Çözümü Sağlayıcısı (CSP) iş ortakları, artık genel kullanıma sunulduğunda herhangi bir Azure hizmetine erişebiliyor. Bir iş ortağı, bir Azure planı kapsamında birden fazla Azure aboneliğine sahip olabilir. 

## <a name="countryregion-availability"></a>Ülke/bölge kullanılabilirliği

Azure için CSP 'deki yeni ticari deneyim Şu anda 137 ülkede kullanılabilir olacak şekilde zamanlandı. Bu [ülkelerin/bölgelerin](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)tam listesini görüntüleyin. 

## <a name="how-to-purchase-azure-plan"></a>Azure planı satın alma

Azure planını satın alma işlemi, başka bir abonelik satın almaya benzer. Temel fark, müşterinizin Microsoft Müşteri anlaşmasını imzaladığı konusunda emin olmak için siparişinizi gerçekten yerleştirmeniz gerekir.

1. **Segment Commercial**' i seçin, ardından "Microsoft Azure" yazın.
2. **Azure planı** altında, **Sepete Ekle**' yi seçin.

   :::image type="content" source="images/azure/Azurepurchase1.png" alt-text="Satınalma.":::

İş ortağı, müşterinin Microsoft Müşteri Anlaşması koşullarını gözden geçirdiğini ve kabul ettiğini onaylamalıdır. İş ortağının bunu nasıl Yapaacağı hakkında daha fazla bilgi için, [Microsoft Müşteri sözleşmesinin müşteri kabulünü Onayla](./confirm-customer-agreement.md)' yı okuyun. [Kaynak galerisinde](https://partner.microsoft.com/resources/collection/Microsoft-Customer-Agreement-in-the-CSP-program#/)diğer kaynaklar mevcuttur.

Daha sonra, Microsoft Müşteri anlaşmasını doğrudan Microsoft ile imzalamak için dijital olarak veya müşteriyi onaylayın. 

### <a name="to-invite-the-customer-to-sign-the-agreement-directly"></a>Müşteriyi anlaşmayı doğrudan imzalamak üzere davet etmek için 

1. Müşterinin **Hesap** sayfasında, **Microsoft Müşteri Sözleşmesi**' nin yanındaki **Güncelleştir** ' i seçin.

2. Müşteri şirketindeki, MCuA 'yi kabul eden kişinin bilgilerini doldurun.

3. **Kaydet ve devam et**’i seçin.  

CSP 'de Azure için sunulan yeni ticaret deneyiminin bir parçası olarak [Yeni bir Azure teklifi sunuyoruz](./azure-plan-lp.md). Önceki Azure teklifiyle ilgili önemli tarihler (MS-AZR-0145p) için [Teklif belgesine](https://go.microsoft.com/fwlink/p/?linkid=2164140)bakın.

**21 Temmuz 2021 *tarihinden önce* kaydolduysanız**
- Önceki Azure teklifini, daha önce satın almış olan müşteriler için sepetin sepetine ekleyebileceksiniz.
- 21 Temmuz 'dan önce kaydolduysanız *ve* 21 Temmuz 'dan sonra kaydolan müşteriler varsa, sepetinize önceki Azure teklifini ekleyemezsiniz.

**21 Temmuz 2021 *tarihinde veya bu tarihten sonra* kaydedilen iş ortakları**
- Önceki Azure teklifini sepetinize ekleyemeyeceksiniz.

Önceki Azure teklifini eklemeye çalışırsanız, ancak yukarıdaki iş ilkesi nedeniyle uygun olmayan durumlarda aşağıdaki hata ile karşılaşacaktır. 

:::image type="content" source="images/add-products.png" alt-text="Ürün ekle ekranını gösteren ekran görüntüsü.":::

Iş Ortağı Merkezi API 'Leri ile yeni Azure planını bulmak için bkz. [Azure planı oluşturma](/partner-center/develop/create-azure-plan#get-the-catalog-item-for-azure-plan).

## <a name="review-and-buy"></a>Gözden geçirin ve satın alın

Azure planının eklendiğini görebileceğiniz **Ürün Ekle** sayfasına dönün. Satın **Alımızı** gözden geçirmek Için **gözden geçir** ' i seçin, 

> [!NOTE]
> bir müşteri için Azure planı satın aldıktan sonra, söz konusu müşteri için Microsoft Azure (0145p) satın alabilirsiniz. Azure planı aracılığıyla gelecekteki abonelikler oluşturmanız gerekecektir.

## <a name="purchase-azure-reservations-under-the-azure-plan"></a>Azure planı kapsamında Azure ayırmaları satın alma 
  
ayrıca, iş ortağı merkezi 'nde müşterileriniz adına Azure planı altında Microsoft Azure rezervasyonları satın alabilirsiniz. (Veya isterseniz, müşterilerinize satın aldığınız önceki bir abonelikten [kendi Azure ayırmalarını satın alma izni verebilirsiniz](give-customers-permission.md) .)

1. [Panonuzdaki](https://partner.microsoft.com/dashboard/)Iş Ortağı Merkezi menüsünden **müşteriler**' i seçin. Azure ayırmaları satın almak isteyen müşteriyi bulun ve ardından müşterinin satırını genişletmek için aşağı oku seçin.

2. **Ürün Ekle** ' yi seçin ve ardından **Azure**' u seçin. 

   - **Segment** listesinden müşterinin pazar segmentini seçin.
   - **Ürün türü** listesinden **ayırmalar** ' ı seçin.
   - Müşterinin rezervasyon **türü** listesinden istediği rezervasyon türünü seçin.

Azure ayırmaları etkin bir Azure planıyla ilişkilendirilmelidir. Müşteri aboneliği listesinden Azure ayırmaları eklemek istediğiniz Azure planını seçin. 

> [!IMPORTANT] 
> Müşterinin zaten etkin bir Azure planı yoksa, şimdi bir tane eklemek için Azure ' ı seçin. Daha fazla yönerge için bkz. [Azure ayırmaları alma](azure-reservations-buying.md#purchase-azure-reservations).

> [!NOTE]
> Bir ayırmanın kapsamı, şu anda Iş Ortağı Merkezi 'nde yalnızca **paylaşılan** olarak ayarlanabilir. tek abonelik kapsamını seçmek veya paylaşılan sunucudan tek bir aboneliğe güncelleştirmek için aşağıdaki yönergeleri kullanarak **Microsoft Azure yönetim portalı** ' na gidin. 

:::image type="content" source="images/azure/addprods1.png" alt-text="Paylaşılan kapsam ayırmaları ayarı.":::

Azure portal müşterinin ayırmasını yönetmek için: 

1. **Müşterilerden** yönetmek istediğiniz müşteriyi seçin. 

2. aşağı oku kullanarak müşterinin satırını genişletin ve **Microsoft Azure yönetim portalı**' nı seçin.  
 
## <a name="view-azure-subscriptions-under-the-azure-plan"></a>Azure planı kapsamındaki Azure aboneliklerini görüntüleme

**Abonelikler** sayfasında, kullanım tabanlı bölümünde **Azure planı ' nı genişleterek Ilişkili** Azure aboneliklerini Azure planı altında görebilirsiniz.

:::image type="content" source="images/azure/addprods2.png" alt-text="Azure aboneliklerinin listesini görüntüleyin."::: 

## <a name="add-subscriptions-and-configure-resources"></a>Abonelik ekleme ve kaynakları yapılandırma

Azure portal ' de müşteri için abonelik ekleyecek ve kaynakları yapılandıracaksınız. Ayrıca, müşterinizin ortamını iş yükü veya proje ile ayırabileceksiniz. Abonelikleri [Azure açık Thouse](https://azure.microsoft.com/services/azure-lighthouse/) ve Azure Portal aracılığıyla yönetmek mümkündür. 

Müşterinizin kaynaklarını ve aboneliklerini yönetmek için, (Aobo) ayrıcalıkları için **yönetici** olmanız gerekir. Erişiminizi yönetme hakkında daha fazla bilgi için [Azure planı kapsamındaki abonelikleri ve kaynakları yönetme](azure-plan-manage.md) makalesini okuyun

## <a name="next-steps"></a>Sonraki adımlar

- [Azure planına müşteri geçişleri](azure-plan-transition.md)

- [İş ortağı kazanılmış kredi-genel bakış](partner-earned-credit.md)
