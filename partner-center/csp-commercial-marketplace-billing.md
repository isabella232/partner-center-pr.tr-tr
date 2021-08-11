---
title: Ticari market ürünleri için faturalama
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Ticari marketten müşteriler için satın alınan ISV SaaS ürünleri veya abonelikleri için faturalamanın nasıl çalıştığını İş Ortağı Merkezi.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 88438321c52528983d0d9309cc93a6824a26d6d5ccb6ecd1512d66ec94ef2ecc
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115691013"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Ticari market ürün ve abonelikleri için faturalama İş Ortağı Merkezi


**Uygun roller:** Genel yönetici | Faturalama yöneticisi

CSP programında iş ortağı olarak, ticari İş Ortağı Merkezi ISV yayımcılarından lisans tabanlı SaaS ürünleri satın almak için İş Ortağı Merkezi'yi kullanabilirsiniz. Bunu yaptıktan sonra, bu tür satın almalar için bir faturaya erişin. Faturalama dönemi takvim ayı ilk gününde başlar ve takvim ayı son gününde sona erer. Faturalar, sonraki ayın 8. gününde kullanılabilir yapılır.

Faturalara panodan veya İş Ortağı Merkezi [API'leri](https://partner.microsoft.com/dashboard/) [kullanarak İş Ortağı Merkezi erişebilirsiniz.](/partner-center/develop/)

CSP programı iş ortakları, bu ürünleri İş Ortağı Merkezi'dan veya Azure portal'den (müşterinin önceden satın alınan CSP tarafından satın alınan Azure kiracısı kullanılarak) satın alan bir müşteri için satın alınan ISV ticari market çözümleri için faturalandırıldı.

>[!NOTE]
>Müşteriler kendi Azure AD kiracılarını (CSP programı içinde bir iş ortağından satın alınmayacak) kullanıyorsa, müşteriler doğrudan[(Microsoft AppSource](https://appsource.microsoft.com/) veya Azure Market) kendi ISV SaaS çözümlerini satın [alma tercihlerini](https://azuremarketplace.microsoft.com/)de kullanabilir. Bunu yaptıklarında doğrudan Microsoft'tan kendi faturalarını alırlar. Benzer şekilde, CSP programında bir iş ortağı müşteriye bir Azure aboneliği veya yeni Azure planı satar ve müşteriye (veya dolaylı kurumsal [bayiye)](/azure/role-based-access-control/built-in-roles) o kiracıya rol tabanlı erişim izni (Okuyucu'dan başka bir role atanarak) bu müşteri (veya dolaylı kurumsal bayi) ticari market tekliflerini CSP iş ortağına önceden onay veya bildirim olmadan da satın alır. Bu gibi durumlarda Microsoft, CSP programı iş ortaklarına müşterileri tarafından yapılan satın almalar hakkında doğrudan bilgi vermez. Ancak Microsoft, Azure aboneliği [Azure İzleyici](/azure/azure-monitor/platform/alerts-activity-log) uyarılar veya bildirimler ayarlamak için kullanabileceğiniz isteğe bağlı bir güvenlik kümesi mekanizması sunar.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Ticari market ürünleri için faturalama bilgilerine erişme

Bir fatura görüntülemeye hazır olduğunda, şirketinizin genel yöneticisi veya faturalama yöneticisi bir e-posta alır. Ticari market ürün satın almalarına yönelik en son fatura ve mutabakat dosyasına erişmek için:

1. İş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. Fatura menüsünden İş Ortağı Merkezi'yi **seçin.** 

    Faturalama sayfasının üst kısmında iki sekme **görüntülenir:** Yinelenen ve **Yinelenen ve tek kez satın almalar.** Her sekme, farklı market ürünleri için fatura ve mutabakat (mutabakat) dosyalarına erişmenizi sağlar:

    - **Yinelenen** sekme: Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro ve Microsoft Azure ile ilgili abonelikler için fatura ve mutabakat Microsoft Azure.

    - **Yinelenen ve tek kullanımlık satın almalar** sekmesi: Azure planı, Azure rezervasyonları, yazılım ve ticari market ürünleri için fatura ve mutabakat dosyalarını gösterir.
  
3. Yinelenen ve **bir kez satın almalar sekmesini** seçin. Bir müşteri için farklı bir para birimiyle abonelik satın yaptıysanız, her para birimi için bir sekme görüntülenir. Bu sayfadan birkaç şey yapabiliriz:

    - En son fatura ve mutabakat dosyasını görmek için Fatura veya Mutabakat **dosyası'ı seçin.**  (Bunu yapmak için en son fatura ve mutabakat dosyası verilerine erişmek için [api'İş Ortağı Merkezi de kullanabilirsiniz.](/partner-center/develop/)

    - Önceki faturaları ve mutabakat dosyalarını görmek için aşağıdaki Faturalama geçmişi **satırına** bakın.

    - En son hesap etkinliğine göre istediğiniz zaman tahmini hesap bakiyenizi veya faturanızı kontrol etmek için Tahminler başlığı altında bir **bağlantı** seçin.  

    >[!NOTE]
    > Faturanızı ayın 8. gününde yayınlaya kadar vergiler ve diğer geçerli ücretler ve krediler dahildir. Bu, son tutarın faturalama döneminde gördüğünüzden farklı olabileceği anlamına gelir.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Ticari market ürünleri için faturalar ve mutabakat dosyaları hakkında daha fazla bilgi

Bu bölümde, üçüncü taraf ISV yayımcılarından müşteriler için satın alınan ticari market SaaS abonelikleri için fatura ve mutabakat dosyaları hakkında daha fazla bilgi sunulmaktadır.

İş Ortağı Merkezi menüsündeki Faturalama seçeneğinden Yinelenen  ve tek kez satın almalar'ı seçerek hem Microsoft (birinci taraf) hem de ISV (üçüncü taraf) satın almaları ile ilgili ücretler için faturalara ve mutabakat dosyalarına erişim elde edersiniz.  Bu satın almalar aşağıdakilerle ilişkili olabilir:

- SaaS abonelikleri (Microsoft veya ISV yayımcılarından)

- Azure planı

- Azure rezervasyonları

- Diğer abonelik tabanlı yazılımlar (Microsoft veya ISV yayımcılarından)

Bu satın alma örnekleri arasında SUSE Linux yazılımı (yazılım aboneliği) veya Azure ISV SaaS ürün aboneliği yer alır.

>[!NOTE]
> Fatura ve mutabakat dosyalarını okuma hakkında daha fazla bilgi için bkz. Faturalamaya [genel bakış.](billing.md)

### <a name="tips-on-reading-your-invoice"></a>İpuçları okumaya devam edin

Üçüncü taraf BIR ISV yayımcısı tarafından lisans tabanlı SaaS ürünü satın aldığınız zaman, faturanıza yalnızca lisans ücreti için ücret yansıtılacaktır. ISV'nin SaaS ürünü temel Alınan Azure altyapı kaynaklarını kullandığında (veya kullandığında) bile bu doğrudur. Bunun nedeni, müşterinizin BIR ISV SaaS ürününün Azure altyapısı kullanım ücretlerinin doğrudan ISV'ye faturalandırılatır. (ISV'ler kendi Azure kullanımları günlük olarak derecelendirilmiş fatura mutabakat dosyasında ilişkili Azure tüketim ücretlerini görebilir.)

Faturanız birkaç sayfa içerir:

- **Faturanın 1. sayfası:** CSP programı iş ortağının faturalama ayrıntılarına ilişkin özet bir genel bakış içerir. Buna faturalama dönemi ücretlerinin özeti, fatura numarası, ödeme koşulları (Net 60 gün) ve havaleyle veya çekle ödemeye yönelik ödeme yöntemleri dahildir.

- **Faturanın 2. Sayfası (ve sonraki sayfalar):** Ticari marketten yapılan birinci taraf Microsoft satın almaları ve üçüncü taraf ISV (lisans tabanlı) satın alma ücretlerinin ayrıntıları. ISV lisans tabanlı satın almaları her ürün adının **Publisher** satıra göre tanımlayabilirsiniz. İlişkili mutabakat dosyası, belirli fatura ücretleri için daha fazla faturalama ayrıntısı sunar.

- **Faturanın son sayfası:** IsV'den lisans tabanlı market ürünleri için ücret aldıysanız, bu son sayfada ISV yayımcısı adı ve adresi hakkında daha fazla ayrıntı görüntülenir.

### <a name="tips-on-reading-your-reconciliation-file"></a>İpuçları dosyanızı okumaya devam edin

Yinelenen **ve bir defalık satın alma mutabakat** dosyası, faturanıza yansıtacak ek ayrıntıları içeren birkaç sütun içerir. **PublisherName sütunu,** satın almanın Microsoft'tan mı yoksa üçüncü taraf BIR ISV yayımcısı mı olduğunu gösterir.

Mutabakat dosyanıza bazı ücretler 0 ABD doları maliyetle görünebilir. Bunun nedeni bir ISV "ücretsiz deneme" teklifi (genellikle 30 veya 60 gün) veya Kendi Lisansını Getir teklifi olabilir.

Ücretsiz deneme ISV teklifleri için:

- Ücretsiz deneme süresi, ISV'nin lisans tabanlı SaaS ürününün bu süre boyunca maliyetini kapsar. Ayrıca ilgili SaaS ürününün ilişkili Azure altyapısı kullanımı için de ücret ödemezsiniz.  Ancak, kullanım tabanlı bir ISV teklifi kullanıyorsanız, ücretsiz deneme, temel Alınan Azure altyapısı kullanımının maliyetini dahil değildir. Bu durumda, Azure altyapısı kullanım ücretleri ayrı bir Azure mutabakat dosyasında görünür.

- Müşteriniz için bir ISV'nin ücretsiz deneme sürümüne uygun ürününü satın aldığınız ve dağıtarak, müşteri ISV yayımcısı tarafından otomatik olarak ücretsiz deneme sürümüne kaydedilir. Ücretsiz deneme süresi, ISV yayımcısı tarafından tanımlanan sürenin ardından otomatik olarak sona erer. Süre sona erdikten sonra müşteri ücret tahsil edilecektir. Bu, mutabakat dosyasında deneme sürümüne uygun bir ürün için iki satır gösterebilirsiniz: Deneme süresi ve ücretli teklifi takip edecek olan (deneme süresi sona erinceye kadar 0 ABD doları maliyet görüntülenir). Deneme sona erdiğinde, ücretli teklifi gösteren satır ücretleri göstermeye başlar. 

Her sütunun neyi temsil ettiği hakkında daha fazla bilgi için [bkz. Mutabakat dosyalarınızı kullanma.](use-the-reconciliation-files.md) Ayrıca [bkz. İş Ortağı Merkezi'da faturalama türleri](./billing-basics.md)

## <a name="next-steps"></a>Sonraki adımlar

- [Müşteriler için ticari market ürünlerini yönetme](csp-commercial-marketplace-manage.md)
- [Ticari market ürünlerine yönelik destek hakkında bilgi alın](csp-commercial-marketplace-support.md)