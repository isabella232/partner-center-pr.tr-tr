---
title: Azure Marketi 'nden yazılım ve çözüm satın alma
description: Azure Marketi 'nde yazılım satın alımları ve yönetimini kolaylaştıran ve kolaylaştıran araçlar hakkında bilgi edinin.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: de58fad7af7dd2cd6b8c98e5763557d54cc776a2
ms.sourcegitcommit: c46658f4d70004596e758fe4cd8671b6e9dadeab
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/20/2021
ms.locfileid: "98584206"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketi satın alma

Azure Marketi, satın alma ilkesi satın alma, faturalama ve yönetme sürecini kolaylaştıran ve kolaylaştırmaya yönelik çeşitli araçlara ve özelliklere sahiptir.

## <a name="simplified-procurement"></a>Basitleştirilmiş tedarik

Azure Market farklı satın alma seçenekleriyle tedarik sürecini basitleştirmenize yardımcı olur. Azure hesabınızla ilişkili bir kredi kartıyla ürün satın alırsanız, tüm satın alımlar tek bir faturada birleştirilir ve seçtiğiniz kredi kartına faturalandırılır. Büyük bir müşteriyseniz Kurumsal Anlaşma kullanarak satın alabilirsiniz. Bir EA ile, tüm yazılım satın alımları Azure faturanızda otomatik olarak eklenir. Faturanızda önce Azure kullanım ücretleri ve onun ardından Azure Market ücretleri yer alır.

Azure Marketi aracılığıyla satın aldığınızda, tek tek satıcı ilişkilerini ve faturalarını yönetme karmaşıklığını ortadan kaldırmış olursunuz. Azure Market satın alımlarınızı ve Azure ücretlerinizi içeren, Microsoft 'un sunduğu tek bir birleştirilmiş aylık faturanız alırsınız.

## <a name="permission-to-purchase"></a>Satın alma izni

Doğru yazılım uygulamasını bulduktan sonra, satın alma işlemi basit olur. Bununla birlikte, Azure aboneliği içinde uygun izinlere ihtiyacınız olacaktır. Azure, [rol tabanlı Access Control](/azure/role-based-access-control/overview) (RBAC) modeli üzerinde çalıştığından, satın alma yapmak için hesabınızın **sahip** veya **katkıda bulunan** izinlerinin olması gerekir.

Satın alma işlemini tamamlamadan önce, kullanıcının Azure kiracısında doğru yapılandırmaya sahip olduğundan emin olun. Bu, satın alma sırasında hataları önlemeye yardımcı olur.

Azure portal Azure Marketi deneyiminde satın almak istediğiniz uygulamayı bulun ve **Oluştur** veya **Ayarla + abone ol**' u seçin. Yeni çözümünüzü kullanabilmeniz için bazı bilgileri gerçekleştirmeniz istenecektir.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Teklif oluştur düğmesi.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="Ayarla + abone ol düğmesi.":::

Azure Marketi çevrimiçi mağazasından bir çözüm dağıtmak istiyorsanız, ürün açıklaması sayfasında **Şimdi al** ' ı seçin ve ardından Azure hesabı kimlik bilgilerinizle oturum açın.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Azure Marketi oturum açma iletişim kutusu.":::

Oturum açtıktan sonra, satın alımınızın tamamlanabilmesi için Azure portal ürüne yönlendirilirsiniz.

## <a name="purchase-policy-management"></a>Satın alma ilkesi yönetimi

Microsoft, Azure abonelik Yöneticisi olarak faturalandırma profiliniz aracılığıyla kullanıcı satın alımlarınızı yönetmenizi sağlar. Üç seçenekten birini belirleyin:

- **Ücretsiz + ücretli** – kullanıcıların herhangi bir Azure Market yazılım uygulaması almasına izin verir.
- **Ücretsiz** – kullanıcıların Azure Marketi 'nden yalnızca ücretsiz yazılım dağıtmaları için izin verir.
- **Hayır** : kullanıcıların Azure Marketi 'nden herhangi bir yazılım dağıtmalarını engeller.

Bu ayarlar, Azure aboneliğinize erişimi olan tüm kullanıcılar için geçerlidir. Bu, size Azure portal aracılığıyla BT satın alma özelliğini denetlemenize olanak tanır.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="BT tedarik Azure portal aracılığıyla denetleniyor":::

## <a name="cost-management"></a>Maliyet yönetimi

Ürünleri Azure Marketi 'nden satın alırken, maliyetleri yönetmenize yardımcı olan Öngörüler elde etmek istersiniz. Azure maliyet yönetimi, satın aldığınız ürünlerle ilgili bilgileri görüntülemek için ücretsiz bir araçtır. Maliyet yönetimi 'ni kullanarak, zaman içinde hangi hizmetlerin para harcadığınızı ve bu maliyetlerin ayarladığınız bütçelerle nasıl izlendiklerine ilişkin ayrıntıları görebilirsiniz. Bütçeleri ayarlamaya ek olarak, raporlar zamanlayabilir ve abonelik maliyetlerini çözümleyebilirsiniz. [Maliyetleri analiz etme ve Azure maliyet yönetimi ile bütçeler oluşturma](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)hakkında Microsoft Learn modülünü tamamlayarak Azure maliyet yönetimi hakkında daha fazla bilgi edinin.

Azure Maliyet Yönetimi'nin altındaki maliyet analizi aracında Azure Market ücretlerinizi ve faturalarınızı görüntüleyebilirsiniz.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Satın alınan ürünlerinizle ilgili Öngörüler elde etmek için Azure maliyet yönetimi 'ni kullanın.":::

## <a name="purchase-validation-checks"></a>Doğrulama denetimleri satın alma

Azure Marketi aracılığıyla bir teklif satın almak farklı nedenlerle başarısız olabilir. Bir satın alma için komut satırı arabirimi (CLı) kullanmanın, Azure Marketi 'nde kullanılamayan veya görünmeyen bir teklif satın almaya çalıştığınız için hatalara neden olma olasılığı yüksektir. Satın alma işlemi başarısız olmasına neden olabilecek denetimler aşağıda verilmiştir:

1. Abonelik bir Kurumsal Anlaşma (EA) ve EA yönetici tarafından devre dışı bırakılmış Azure Marketi satın almalara aittir.
1. EA Yöneticisi yalnızca ücretsiz teklifler için satın alma işlemlerini etkinleştirdi ve teklif ücretli bir tekliftir.
1. Teklif Market 'te bulunamadı.
1. Bağımsız yazılım satıcısı (ISV), teklifi en azından bölgenizde satmaya durdurdu.
1. Kullandığınız abonelik, teklifin kullanılamadığı bir bölgedeki faturalandırma hesabına aittir.
1. Abonelik/Faturalandırma hesabı geçerli bir ödeme gereci (örn. geçerli bir kredi kartı) ile ilişkilendirilmemiş.
1. Abonelik bir bulut çözümü sağlayıcısına (CSP) ait ve ISV, CSP aracılığıyla satış için reddedildi.
1. Özel Market abonelik için etkinleştirilmiştir ve teklif izin verilen teklifler listesinde değildir.
1. Teklif, belirli müşteriler için özel/önizlemedir ve abonelik izin verilen müşteriler listesinde değildir.

## <a name="next-steps"></a>Sonraki adımlar

- [Ödeme ve faturalama](billing-invoicing.md)