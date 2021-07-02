---
title: Azure portal'da SaaS teklifi satın alma
description: Azure portal'da SaaS teklifi bulma ve satın alma hakkında bilgi Azure portal.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/29/2021
ms.openlocfilehash: a124e4c5bb31a1fbb744bf2c5e1ea65a356bdd54
ms.sourcegitcommit: 1d09ccaaa54f167b0c63e99761172ebe84e89f2e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/02/2021
ms.locfileid: "113221449"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Azure portal'da SaaS teklifi satın Azure portal

Bu makalede, hizmet olarak yazılım (SaaS) teklifini arama, denmeye ve satın almaya ilgili farklı seçenekler ve gereksinimler Azure portal.

## <a name="create-a-saas-subscription"></a>SaaS aboneliği oluşturma

SaaS aboneliği satın almak için uygun bir Azure aboneliğine erişimi olan bir Azure kullanıcı hesabına ihtiyacınız vardır. Bu abonelik hem faturalama hem de satın alınan bulut kaynaklarınızı bölmek için kullanılacaktır. Azure abonelikleri hakkında daha fazla bilgi edinmek için [bkz. Ek Azure aboneliği oluşturma.](/azure/cost-management-billing/manage/create-subscription)

Aşağıdaki Azure portal Market bölümünde istediğiniz SaaS **teklifini** seçin.

Hizmet Olarak Yazılım aboneliği, tek tek bilgisayarlara yerel yükleme yerine çevrimiçi abonelik aracılığıyla belirli bir süre boyunca hizmet kullanma hakkı sağlar. Abonelik, kullanıcı başına lisans ücretine veya bulut tabanlı kaynak tüketimine göre tahakkuk eden bir veya daha fazla bulut platformu veya hizmeti kullanma sözleşmesidir. Bir kuruluşun birden çok SaaS aboneliği olabilir.

SaaS abonelikleri ile ilgili kısıtlamalar şunlardır:

- Öğrenci aboneliği yok.
- Abonelik Visual Studio Enterprise yoktur.
- Ücretsiz kredi aboneliği yoktur.
- Ücretli teklifler için bir ödeme aracı gereklidir.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS, Azure portal'de bulma Azure portal

Yeni bir Azure portal, aramanızı SaaS tekliflere odaklanmak için daraltmanın birkaç yolu vardır.

### <a name="narrowing-your-search"></a>Aramanızı daraltma

Giriş sayfasında, **Azure hizmetleri'nin altında** **+ Kaynak oluştur veya Market'i** **seçin.** Veya platformun herhangi bir **yerinde G + N** kısayolunu kullanın.

- Teklif Türü filtresini ve ardından  SaaS'yi seçerek sonuçları **SaaS tekliflerini daraltarak.**
- Belirli bir SaaS genel arama bulmak için üst gezinti alanında yer alan gezinti çubuğunu kullanın.

Market giriş [sayfası üst sayfasındaki](/marketplace/private-offers) başlığı seçerek bir Özel SaaS **teklifi** bulun. Tüm teklifler veya planlar tüm coğrafyalarda kullanılamaz ve bazıları yalnızca belirli kiracılar için görünebilir.

Filtrelenmiş görünüm, bir başlıkla temsil edilen kullanılabilir saaS tekliflerini gösterir. Ürün ayrıntıları sayfasını görmek için birini seçin. Aşağıdaki bölümleri içerir:

- Genel bakış – hizmet, pazarlama ve öğrenme malzemeleriyle ilgili ayrıntılar
- Planlar + Fiyatlandırma: Her teklif, farklı faturalama koşullarına ve fiyatlarına sahip en az bir plan içerir
- Kullanım Bilgileri + Destek – Publisher kimliği, Teklif Kimliği ve Plan Kimliği'ne dahildir
- Belirli Bir SaaS teklifinin Derecelendirmesi ve Gözden İncelemesi

## <a name="available-billing-models-plansskus-for-saas-offers"></a>SaaS teklifleri için kullanılabilir faturalama modelleri (planlar/SU'lar)

Her SaaS teklifinin bir veya daha fazla planı vardır. Her teklifle ilişkilendirilmiş bir fiyatlandırma modeli vardır: düz fiyat veya kullanıcı başına. Her plan fiyatı, sıfır dolar (listelenen tüm fiyatlar yalnızca örnek amaçlıdır ve gerçek maliyetleri yansıtmak için amaçlanmaz) yinelenen bir ücrettir. Bu ücret sabit ücret veya kullanıcı başına fiyattır. Kullanılabilir plan türleri:

- **Aylık planlar –** yinelenen aylık ücret; aylık yinelemede ödenen düz veya kullanıcı başına aylık ücret. Süre sona erdiğinde plan otomatik olarak yenilenir.
- **Yıllık planlar** – yinelenen yıllık ücret; yıllık yinelemede ödenen düz veya kullanıcı başına yıllık ücret. Süre sona erdiğinde plan otomatik olarak yenilenir.
- **Özel ölçümler:** Yinelenen ücretlere ek olarak sabit bir ücret planı, düz ücrete dahil edilen fazla kullanım için isteğe bağlı özel tarifeli boyutlar da içerebilir. Her boyut faturalanabilir birimi temsil eder. Bu, bant genişliği, biletler veya işlenen e-posta gibi tarifeli birimlerin kullanımına göre değişen değişken bir maliyettir. Bu boyutların kullanımınıza göre aylık olarak ücretlendirme yapılır. Fazla kullanımın yalnızca sabit ücrete dahil edilen tüm tarifeli birimleri kullandıktan sonra başlatıla olduğunu unutmayın.
- **Ücretsiz Deneme** – Bazı durumlarda, plan bir aylık deneme süresi içerir ve bu süre boyunca yazılımı ücretsiz olarak kullanabilirsiniz.  Deneme süresi sona erdiktan sonra planınıza göre ücret tahsil edileceksiniz. Deneme teklifleri özel sayaçlarla uyumlu değildir.

Bu fiyatlandırma modelleri hem Genel hem de Özel planlarda kullanılabilir.

## <a name="saas-purchase-experience"></a>SaaS satın alma deneyimi

1. Ürün sayfasında, İhtiyaçlarınızı karşılayacak bir plan seçin ve ayarlamaya ve abone **olmaya devam edin**
2. Satın alma işleminin bir parçası olarak Temel Bilgiler sekmesine yeniden **yönlendirilmesi** gerekir:
    1. Faturalama *için* hangi Aboneliği kullanmak istediğinizi tanımlayın. Kullanmakta olduğu Azure aboneliği için tanımlanmış geçerli bir satın alma yöntemi olmalıdır. Doğru izin düzeyine sahip olmalı veya bu aboneliğin altında doğru izin düzeyine sahip bir kaynak grubunuz olması gerekir. Ayrıca faturalama ülkesi, teklifin satın alına açık olduğu bir ülke de olabilir. Geçerli bir ödeme yöntemi olmayan Azure abonelikleri (örneğin MSDN aboneliği) yalnızca ücretsiz planlar satın almak için kullanılabilir
    1. SaaS kaynağının *ait olduğu* bir * Kaynak Grubu seçin veya oluşturun.
    1. SaaS *aboneliğini* daha sonra kolayca tanımlamak için bir Ad yazın. Satın almadan sonra adı değiştiremezsiniz.
    1. Plan **altında,** seçtiğiniz planı ürün ayrıntılı sayfasında (PDP) görebilirsiniz. PDP'de etkin bir seçim yaptıysanız varsayılan planı karşınız. Planı değiştir bağlantısını seçerek **seçiminizi değiştirebilirsiniz.** İlgili faturalama dönemi'ne ve ardından başka bir plan seçin. Yayımcı destekliyorsa, satın alma sonrasında planı değiştirebilirsiniz. Ancak, dönemi aylıktan yıllık veya yıllıktan aylık olarak değiştiremezsiniz.
    1. Fiyatlandırma modelinin kullanıcı başına olduğu *durumlarda* Kullanıcı sayısını belirtmeniz *gerekebilir.* Gördüğünüz fiyat, seçtiğiniz aboneliğe, plana ve terime göre değişir.
3. Etiketler **sekmesine** geçin - *Etiketler,* doğrudan bir kaynağa veya kaynak grubuna yerleştiril kullanıcılar tarafından tanımlanan anahtar/değer çiftleridir. Daha sonra SaaS kaynağınızı kolayca bulmak için etiketleri kullanabilirsiniz. Azure şu anda kaynak ve kaynak grubu başına en fazla 50 etiketi destekler. Etiketler, oluşturma sırasında bir kaynağa yer değiştirebilir veya var olan bir kaynağa eklenebilir.
4. Teklifi gözden **geçirmek ve ayrıntıları planlamak** için Gözden Geçir + Abone Ol'a devam edin.
    1. Yayımcının *Kullanım koşulları,* *Düzeltmeler* ve *Gizlilik ilkesi ile* ilgili daha fazla bilgi için Azure Market
    1. İletişim ayrıntılarınızı eklemeniz istenebilirsiniz
    1. Temel *Bilgiler ve Etiketler* ayrıntılarını *gözden* geçirme
5. Onaydan sonra Abone **ol'a tıklayın.**

## <a name="saas-subscription-and-configuration"></a>SaaS Aboneliği ve yapılandırması

Abone ol'ı seçerek "SaaS aboneliğiniz devam ediyor" iletisiyle ifade edin. Bu işlem birkaç dakika sürer, tamam olana kadar pencereyi kapatabilirsiniz.

Abonelik tamamlandıktan sonra, SaaS aboneliğinizin tamam olduğunu ve satın alma işlemlerinizin keyfini çıkararak hesabı yapılandırmanız gerektiğini iletin. Ayrıca yeni aboneliği etkinleştirmenizi istediğiniz bir e-posta da alırsınız. SaaS hesabını yapılandıracak kişi siz değilsanız, bu e-postayı ilgili kişiye iletin.

Süreci tamamlamak ve SaaS'ı kullanmaya başlamak için aboneliğinizi yapılandırmaya başlamanız gerekir. Hesabı şimdi yapılandır **düğmesini seçerek** sizi yayımcının web sitesine yönlendirecek.

Üst bilginin sağ üst köşesindeki 'zil' simgesini seçerek de abonelik durumunu kontrol edebilirsiniz.

Yapılandırma işlemini *30* gün içinde tamamlarsanız, bu SaaS aboneliği otomatik olarak *silinir.* Faturalandırma, hesabınız yayımcının web sitesinde yapılandırıldığında başlar.

İşlem sırasında karşı karşıya olabileceğiniz hata iletileri:

- Seçilen *planın plan adı* ücretsiz abonelikte satın alınamaz
  - Daha fazla ayrıntı için https://aka.ms/UpgradeFreeSub bkz. hesabı yükseltin.

- Geçerli bir kredi kartı veya Azure aboneliğiniz ile ilişkili bir ödeme yöntemi bulamadımız için satın alma işlemi başarısız oldu.
  - Bu abonelik için farklı bir Azure aboneliği kullanın veya geçerli kredi kartını veya ödeme yöntemini ekleyin/güncelleştirin ve yeniden deneyin.

- Teklifin *yayımcısı tarafından teklif* *teklifi* adı olarak seçilen planın plan *adı,* IT Yöneticiniz tarafından ayarlanmış kurallara göre satın almak için kullanılamaz.
  - IT Yöneticinize ulaşın.

- Teklifin *yayımcısı tarafından* seçilen teklif  planının plan adı, kiracının IT Yöneticisi tarafından yapılan özel market ayarları nedeniyle satın alma için kullanılamaz. 
  - IT Yöneticinize ulaşın

- İstenen faturalama dönemi boş veya geçersiz olduğundan satın alma başarısız oldu.
  - Farklı bir plan / faturalama dönemi satın alma denemesi.

- Yasal anlaşmada imzalama işleminizi doğrulayamamız nedeniyle satın alma işlemi başarısız oldu.
  - Yeni -den deneme. Hata devam ederse, farklı Azure aboneliğini kullanarak satın alma denemesi yapmaya veya de destekle iletişime geçin.

- Publisher *PublisherID* *tarafından teklif offerID* satın alma işlemi başarısız oldu. Bu teklif şu anda satın alma için kullanılamaz.
  - Daha sonra tekrar deneyin. Bir saat sonra bu hata iletisini almaya devam ediyorsanız lütfen de destekle iletişime geçin.  

- Publisher *PublisherID* *tarafından teklif* *offerID planID'lerinin* satın alma işlemi başarısız oldu. Bu plan şu anda satın alma için kullanılamaz.
  - Daha sonra tekrar deneyin. Bir saat sonra bu hata iletisini almaya devam ediyorsanız lütfen de destekle iletişime geçin. 

- *ObjectID* *nesne kimliğine* sahip istemci e-posta adresinin ResourceGroup kapsamı üzerinde *DeploymentValidationAction eylemi* gerçekleştirme *yetkisi yoktur; DeploymentScope* veya kapsam geçersiz.  
  - Azure aboneliği/Kaynak Grubu üzerinde doğru izinlere sahip değilsanız bu iletiyi alırsınız.  
    Erişim kısa süre önce verildi ise lütfen kimlik bilgilerinizi yenileyin.  
    Kaynakları bir kaynak grubuna dağıtmak için en azından Katkıda Bulunan erişiminizin olması gerekir. Kaynak Grupları altında erişim durumunu **kontrol edin ve** sonra Access Control.  Bu, sizi 'Katkıda Bulunan' olarak atamak istediğiniz 'Sahip'in kim olduğunu gösterir.

- Bu satın alma için kullanılan abonelik, Market satın almalarına izin vermez.  
  - Lütfen farklı bir abonelik kullanın veya yöneticinizden bu abonelik için tanımı değiştirmesini ve yeniden denemesini sorun.

## <a name="next-steps"></a>Sonraki adımlar

- Markette zaten bir teklif satın aldıysanız [Faturalama'ya gidin](/marketplace/billing-invoicing)
- Özel planlar seçenekleri hakkında daha fazla [bilgi de öğrenebilirsiniz.](/marketplace/private-offers)
