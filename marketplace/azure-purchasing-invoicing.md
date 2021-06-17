---
title: Yazılım ve çözüm satın alma Azure Market
description: Yazılım satın alma ve yönetim süreçlerini basitleştirerek kolaylaştıran araçlar hakkında bilgi Azure Market.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: f747c11ef4bfc9abe1035ffb3f059da59b6572ac
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276510"
---
# <a name="azure-marketplace-purchasing"></a>Azure Market satın alma

Azure Market satın alma, faturalama ve satın alma ilkesi yönetme sürecini basitleştiren ve kolaylaştıran çok sayıda araç ve özelik vardır.

## <a name="simplified-procurement"></a>Basitleştirilmiş tedarik

Azure Market farklı satın alma seçenekleriyle tedarik sürecini basitleştirmenize yardımcı olur. Azure hesabınızla ilişkili bir kredi kartı kullanarak ürün satın alırsanız, tüm satın almalar tek bir faturada birleştirilmiş olur ve tercihen kredi kartına faturalandırılır. Büyük bir müşteriysiniz, satın almak için bir Kurumsal Anlaşma. EA ile tüm yazılım satın almaları otomatik olarak Azure faturanıza dahil edilir. Faturanızda önce Azure kullanım ücretleri ve onun ardından Azure Market ücretleri yer alır.

Satın alma Azure Market, tek tek satıcı ilişkilerini ve faturalarını yönetme karmaşıklığını ortadan kaldırmış oluruz. Microsoft'tan hem satın aldığınız satın almaları hem de Azure ücretlerinizi içeren Azure Market birleştirilmiş aylık fatura alırsiniz.

## <a name="permission-to-purchase"></a>Satın alma izni

Doğru yazılım uygulamasını buladıktan sonra satın alma işlemlerini tamamlamak oldukça kolaydır. Ancak, Azure aboneliği içinde uygun izinlere ihtiyacınız olacak. Azure rol tabanlı [bir](/azure/role-based-access-control/overview) Access Control (RBAC) modeli üzerinde çalışma  yaptığı  için, hesabınız satın alma için abonelik sahibi veya katkıda bulunan izinlerine ihtiyaç gösterir.

Satın alma işlemi tamamlamadan önce kullanıcının Azure kiracısı için doğru yapılandırmaya sahip olduğundan emin olun. Bu, satın alma sırasında hataları önlemeye yardımcı olur.

Uygulama Azure Market deneyiminde Azure portal satın almak istediğiniz uygulamayı bulun ve Oluştur veya **Ayarla** + abone **ol'ı seçin.** Yeni çözümlerinizi kullanamadan önce bazı bilgileri tamamlamanız istenir.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Teklif Oluştur düğmesi.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="Ayarla + abone ol düğmesi.":::

Azure Market çevrimiçi mağazasından bir çözüm dağıtmak için ürün  açıklaması sayfasında Şimdi edinin'i seçin ve azure hesabı kimlik bilgilerinizle oturum açın.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Oturum Azure Market iletişim kutusu.":::

Oturum açma işlemi tamamlandıktan sonra satın alma işleminizi tamamlamak için Azure portal ürüne yönlendirilmesi gerekir.

## <a name="purchase-policy-management"></a>İlke yönetimi satın alma

Microsoft, azure abonelik yöneticisi olarak faturalama profiliniz aracılığıyla kullanıcı satın almalarını yönetmenize olanak sağlar. Üç seçenekten birini belirleyin:

- **Ücretsiz + Ücretli** – Kullanıcıların herhangi bir yazılım uygulamasını Azure Market sağlar.
- **Ücretsiz** – Kullanıcıların yalnızca sanal ağlardan ücretsiz yazılım Azure Market.
- **Hayır** – Kullanıcıların sanal ağlardan herhangi bir yazılım Azure Market.

Bu ayarlar, Azure aboneliğinize erişimi olan tüm kullanıcılar için geçerlidir ve bu sayede azure aboneliğiniz aracılığıyla IT tedarikini denetleme Azure portal.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Azure portal aracılığıyla IT tedarikini denetleme.":::

## <a name="cost-management"></a>Maliyet yönetimi

Ürün satın aldığınız Azure Market, maliyetleri yönetmenize yardımcı olacak içgörüler elde etmek istersiniz. Azure Maliyet Yönetimi satın aldığınız ürünlerle ilgili bilgileri görüntülemeye ilişkin ücretsiz bir araçtır. Maliyet Yönetimi'ne bakarak zaman içinde hangi hizmetlere para harcadığınız ve bu maliyetlerin ayar maliyetlerini nasıl takip ettiyebilirsiniz. Bütçe ayarlamaya ek olarak raporları zamanlamayı ve abonelik maliyetlerini analiz edebilirsiniz. Maliyetleri analiz etme ve Azure Maliyet Yönetimi bütçe oluşturma Microsoft Learn modülünü tamamlayarak daha [fazla bilgi Azure Maliyet Yönetimi.](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)

Azure Maliyet Yönetimi'nin altındaki maliyet analizi aracında Azure Market ücretlerinizi ve faturalarınızı görüntüleyebilirsiniz.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Satın Azure Maliyet Yönetimi içgörüler elde etmek için Azure Maliyet Yönetimi'i kullanın.":::

## <a name="purchase-validation-checks"></a>Satın alma doğrulama denetimleri

Teklif satın alma Azure Market farklı nedenlerle başarısız olabilir. Satın alma için komut satırı arabirimini (CLI) kullanmak hatalara neden olma olasılığı daha yüksek olacaktır çünkü teklifte kullanılabilir veya görünür olmayan bir teklif Azure Market. Satın almanın başarısız olmasına neden olan denetimler aşağıda ve ardından ve ardından ve bu denetimler yer amektedir:

1. Abonelik bir kuruluşa (EA) Kurumsal Anlaşma ve EA yöneticisi satın almaları devre Azure Market devre dışı bırakılmıştır.
1. EA yöneticisi yalnızca ücretsiz teklifler için satın almaları etkinleştirmiş ve teklif ücretli bir tekliftir.
1. Teklif markette bulunamıyor.
1. Bağımsız Yazılım Satıcısı (ISV), en azından bölgenize göre teklifi satmayı durdurdu.
1. Kullanmakta olduğu abonelik, teklifin kullanılabilir olduğu bir bölgedeki ödeme hesabına aittir.
1. Abonelik/ödeme hesabı geçerli bir ödeme aracıyla (geçerli bir kredi kartı gibi) ilişkilendirilmiştir.
1. Abonelik bir Bulut Çözümü Sağlayıcısı (CSP) ait ve ISV CSP aracılığıyla satmayı reddetti.
1. Abonelik için Özel Market etkindir ve teklif izin verilen teklifler listesinde yer almamaktadır.
1. Teklif, belirli müşteriler için Özel/Önizlemedir ve abonelik izin verilen müşteriler listesinde yer almamaktadır.

## <a name="next-steps"></a>Sonraki adımlar

- [Ödeme ve faturalama](billing-invoicing.md)