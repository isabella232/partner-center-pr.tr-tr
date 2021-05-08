---
title: Azure Marketi 'nden yazılım ve çözüm satın alma
description: Azure Marketi 'nde yazılım satın alımları ve yönetimini kolaylaştıran ve kolaylaştıran araçlar hakkında bilgi edinin.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 04/15/2021
ms.openlocfilehash: cfe37f26ad685ca723336d8559d15d4a64048f4b
ms.sourcegitcommit: 2ad9e61fa5b9941f927ebf44c459b6c1bd055b9d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/08/2021
ms.locfileid: "109630092"
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

Azure Market çevrimiçi mağazasından bir çözüm dağıtmak için ürün  açıklaması sayfasında Şimdi edinin'i seçin ve azure hesabı kimlik bilgilerinizle oturum açın.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Oturum Azure Market iletişim kutusu.":::

Oturum açma işlemi tamamlandıktan sonra satın alma işleminizi tamamlamak için Azure portal ürüne yönlendirilmesi gerekir.

## <a name="purchase-policy-management"></a>İlke yönetimi satın alma

Microsoft, azure abonelik yöneticisi olarak faturalama profiliniz aracılığıyla kullanıcı satın almalarını yönetmenize olanak sağlar. Üç seçenekten birini belirleyin:

- **Ücretsiz + Ücretli** – Kullanıcıların herhangi bir yazılım uygulamasını Azure Market sağlar.
- **Ücretsiz** – Kullanıcıların yalnızca sanal ağlardan ücretsiz yazılım Azure Market.
- **Hayır** – Kullanıcıların sanal ağlardan herhangi bir yazılım Azure Market.

Bu ayarlar, Azure aboneliğinize erişimi olan tüm kullanıcılar için geçerlidir ve bu sayede azure aboneliğiniz aracılığıyla IT tedarikini denetleme Azure portal.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Azure portal aracılığıyla IT tedarikini denetleme":::

## <a name="cost-management"></a>Maliyet yönetimi

Ürün satın aldığınız Azure Market, maliyetleri yönetmenize yardımcı olacak içgörüler elde etmek istersiniz. Azure Maliyet Yönetimi satın aldığınız ürünlerle ilgili bilgileri görüntülemeye ilişkin ücretsiz bir araçtır. Maliyet Yönetimi'ne bakarak zaman içinde hangi hizmetlere para harcadığınız ve bu maliyetlerin ayar maliyetlerini nasıl takip ettiyebilirsiniz. Bütçe ayarlamaya ek olarak raporları zamanlamayı ve abonelik maliyetlerini analiz edebilirsiniz. Maliyetleri analiz etme ve Azure Maliyet Yönetimi bütçe oluşturma Microsoft Learn modülünü tamamlayarak daha [fazla bilgi Azure Maliyet Yönetimi.](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)

Azure Maliyet Yönetimi'nin altındaki maliyet analizi aracında Azure Market ücretlerinizi ve faturalarınızı görüntüleyebilirsiniz.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Satın Azure Maliyet Yönetimi içgörüler elde etmek için Azure Maliyet Yönetimi'i kullanın.":::

## <a name="purchase-validation-checks"></a>Satın alma doğrulama denetimleri

Teklif satın alma Azure Market farklı nedenlerle başarısız olabilir. Satın alma için komut satırı arabirimini (CLI) kullanmak hatalara neden olma olasılığı daha yüksek olacaktır çünkü teklifte kullanılabilir veya görünür olmayan bir teklif Azure Market. Satın alma işlemi başarısız olmasına neden olabilecek denetimler aşağıda verilmiştir:

1. Abonelik bir Kurumsal Anlaşma (EA) ve EA yönetici tarafından devre dışı bırakılmış Azure Marketi satın almalara aittir.
1. EA Yöneticisi yalnızca ücretsiz teklifler için satın alma işlemlerini etkinleştirdi ve teklif ücretli bir tekliftir.
1. Teklif Market 'te bulunamadı.
1. Bağımsız yazılım satıcısı (ISV) kullanım dışıdır (eski adıyla, daha önce bu teklif, bölgeniz).
1. Kullandığınız abonelik, teklifin kullanılamadığı bir bölgedeki faturalandırma hesabına aittir.
1. Abonelik/Faturalandırma hesabı geçerli bir ödeme gereci (örn. geçerli bir kredi kartı) ile ilişkilendirilmemiş.
1. Abonelik bir bulut çözümü sağlayıcısına (CSP) ait ve ISV, CSP aracılığıyla satış için reddedildi.
1. Özel Market abonelik için etkinleştirilmiştir ve teklif izin verilen teklifler listesinde değildir.
1. Teklif, belirli müşteriler için özel/önizlemedir ve abonelik izin verilen müşteriler listesinde değildir.

## <a name="next-steps"></a>Sonraki adımlar

- [Ödeme ve faturalama](billing-invoicing.md)