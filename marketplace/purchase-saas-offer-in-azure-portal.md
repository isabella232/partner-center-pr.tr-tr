---
title: Azure portal bir SaaS teklifi satın alma
description: Azure portal bir SaaS teklifini bulmayı ve satın almayı öğrenin.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 08/05/2021
ms.openlocfilehash: 4f83d5c85f0316ad5c9d9ad75ca6519b5940146f
ms.sourcegitcommit: 38afe7e35e3dce4f35cf7352cc98e3d53e979a62
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/23/2021
ms.locfileid: "122752108"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Azure portal bir SaaS teklifi satın alma

Bu makalede, Azure portal bir hizmet olarak yazılım (SaaS) teklifi aramak, denemek ve satın almak için farklı seçenekler ve gereksinimler açıklanmaktadır.

## <a name="create-a-saas-subscription"></a>SaaS aboneliği oluşturma

SaaS aboneliği satın almak için uygun bir Azure aboneliğine erişimi olan bir Azure Kullanıcı hesabına ihtiyacınız vardır. Bu abonelik, faturalandırma için ve satın alınan bulut kaynaklarınızın compartmen'i için kullanılacaktır. Azure abonelikleri hakkında daha fazla bilgi edinmek için bkz. [ek bir Azure aboneliği oluşturma](/azure/cost-management-billing/manage/create-subscription).

Azure portal **Market** bölümünde istenen SaaS teklifini seçin.

Bir hizmet olarak yazılım aboneliği, belirli bir süre için tek bir bilgisayara yerel yükleme yerine çevrimiçi bir abonelik aracılığıyla bir hizmeti kullanma hakkını sağlar. Abonelik, bir veya daha fazla bulut platformu veya hizmeti kullanmak için bir anlaşmadır. Bu, ücretleri Kullanıcı başına lisans ücreti ya da bulut tabanlı kaynak tüketimine göre tahakkuk eder. Bir kuruluş birden çok SaaS aboneliğine sahip olabilir.

SaaS abonelikleriyle ilgili kısıtlamalar şunlardır:

- Öğrenci aboneliği yok.
- Visual Studio Enterprise aboneliği yok.
- Ücretsiz kredi aboneliği yok.
- Ücretli teklifler için bir ödeme aracı gereklidir.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS Azure portal ' de bulma sağlar

Azure portal olduğunuzda, aramanızı SaaS tekliflerine odaklanmak üzere daraltmak için birkaç yol vardır.

### <a name="narrowing-your-search"></a>Aramanızı daraltma

Giriş sayfasında, **Azure hizmetleri** altında **+ kaynak** veya **Market** oluştur ' u seçin. Ya da platformda herhangi bir yerde **G + N** kısayolunu kullanın.

- **Teklif türü** filtresini ve sonra **SaaS**'yi seçerek SaaS tekliflerle Sonuçları daraltın.
- Belirli bir SaaS teklifini bulmak için üst gezinti alanındaki genel arama çubuğunu kullanın.

**Market** giriş sayfasının en üstündeki başlık ' i seçerek [özel bir SaaS teklifi](./private-plans.md) bulun. Tüm olanaklar veya planlar tüm coğrafi bölgelerde kullanılamaz ve bazıları yalnızca belirli kiracılar için görünebilir.

Filtrelenmiş görünüm, bir başlığa göre temsil edilen her bir kullanılabilir SaaS teklifini gösterir. Ürün ayrıntıları sayfasını görmek için bir tane seçin. Aşağıdaki bölümleri içerir:

- Genel Bakış – hizmet, pazarlama ve öğrenme malzemeleri hakkındaki ayrıntılar
- Planlar + fiyatlandırma – her teklif, farklı fatura koşullarına ve fiyatlarına sahip en az bir plan içerir
- kullanım bilgileri + destek – Publisher kimliği, teklif kimliği ve Plan kimliği içerir
- Belirli SaaS teklifini derecelendirme ve gözden geçirme

## <a name="available-billing-models-plansskus-for-saas-offers"></a>SaaS teklifleri için kullanılabilir faturalandırma modelleri (planlar/SKU 'Lar)

Her SaaS teklifinin bir veya daha fazla planı olacaktır. Her teklifin ilişkili bir fiyatlandırma modeli vardır: sabit oran veya Kullanıcı başına. Her plan fiyatı, sıfır ABD Doları olabilen yinelenen ücrettir (listelenen tüm fiyatlar yalnızca örnek amaçlıdır ve gerçek maliyetlerin yansıtılmaya yönelik değildir). Bu ücret, sabit fiyat veya Kullanıcı başına fiyat ' dır. Kullanılabilir plan türleri:

- **Aylık planlar** – yinelenen aylık ücret; aylık tekrarda ödenen, sabit veya Kullanıcı başına aylık ücret. Dönem sona erdiğinde, plan otomatik olarak yenilenir.
- **Yıllık planlar** – yinelenen yıllık ücret; yıllık tekrarda ödenen, sabit veya Kullanıcı başına yıllık ücret. Dönem sona erdiğinde, plan otomatik olarak yenilenir.
- **Özel** ölçümler: Yinelenen ücretler ile birlikte, sabit bir fiyat planı, fazla kullanım için de sabit fiyata dahil olmayan isteğe bağlı özel ölçülen boyutları da içerebilir. Her boyut faturalandırılabilir bir birimi temsil eder. Bu, ölçülen birim kullanımına göre değişen bir değişken maliyettir: bant genişliği, Bilet veya işlenen e-posta. Aylık olarak bu boyutların tüketimine göre ücretlendirilirsiniz. Fazla kullanım tüketimi yalnızca sabit fiyata dahil edilen tüm ölçülen birimleri kullandığınızda başlar.
- **Ücretsiz deneme** : bazı durumlarda plan bir ayın deneme süresini içerir, bu da yazılımı ücretsiz olarak kullanabilirsiniz.  Deneme süresi bittikten sonra, planınıza göre ücretlendirilirsiniz. Deneme teklifleri özel ölçümlerle uyumlu değildir.

Bu fiyatlandırma modelleri hem genel hem de özel planlar için kullanılabilir.

## <a name="saas-purchase-experience"></a>SaaS satın alma deneyimi

1. Ürün sayfasında, gereksinimlerinizi karşılayan bir plan seçin ve **+ abone ol** ' u ayarlamaya devam edin
2. Satın alma sürecinin bir parçası olarak, **temel bilgiler** sekmesine yönlendirilirsiniz ve şunları yapmanız gerekir:
    1. Faturalandırma için kullanmak istediğiniz *aboneliği* tanımlayın. Kullandığınız Azure aboneliğinin Kendisi için tanımlanmış geçerli bir satın alma yöntemi olmalıdır. Doğru izinlere sahip olmanız veya bu aboneliğin altında doğru izin düzeyine sahip bir kaynak grubunuz olması gerekir. Ayrıca, faturalandırma ülkesi, teklifin satın alma için kullanılabildiği bir ülke olmalıdır. Azure abonelikleri geçerli bir ödeme yöntemi olmadan (örneğin, bir MSDN aboneliği) yalnızca ücretsiz planlar satın almak için kullanılabilir
    1. SaaS kaynağının ait olacağı bir **kaynak grubu* seçin veya oluşturun.
    1. Daha sonra kolayca tanımlamak için SaaS aboneliğine bir *ad* yazın. Satın aldıktan sonra adı değiştiremezsiniz.
    1. **Plan**' ın altında, ürün ayrıntılı sayfasında (PDP) seçtiğiniz planı görürsünüz. PDP 'de etkin bir seçim yaptıysanız, varsayılan planı görürsünüz. **Planı değiştir** bağlantısını seçerek seçiminizi değiştirebilirsiniz. İlgili faturalandırma terimini seçin ve ardından başka bir plan seçin. Yayımcı destekliyorsa, satın alma işleminden sonra planı değiştirebilirsiniz. Ancak, dönemi aylık veya yıllık olarak aylık olarak değiştiremeyeceksiniz.
    1. Fiyatlandırma modelinin *Kullanıcı başına* olduğu durumlarda *, kullanıcı sayısını belirtmeniz gerekebilir.* Gördüğünüz fiyat, seçtiğiniz abonelik, plan ve terime göre değişecektir.
3. **Etiketler** sekmesine geç- *Etiketler* , doğrudan bir kaynağa veya kaynak grubuna yerleştirilebilecek Kullanıcı tanımlı anahtar/değer çiftleridir. SaaS kaynağınızı daha sonra üzerinde kolayca bulmak için Etiketler ' i kullanabilirsiniz. Azure Şu anda kaynak ve kaynak grubu başına en fazla 50 etiketi desteklemektedir. Etiketler, oluşturma sırasında veya var olan bir kaynağa eklenen bir kaynağa yerleştirilebilir.
4. Teklif ve plan ayrıntılarını gözden geçirmek için ve **abone** olmaya devam edin.
    1. Yayımcının *kullanım koşulları*, *Düzeltme* ve *Gizlilik ilkesini* ve ayrıca Azure Marketi 'ni gözden geçirin
    1. İletişim bilgilerinizi eklemek isteyip istemediğiniz sorulabilir
    1. *Temel bilgiler* ve *Etiketler* ayrıntılarını gözden geçirin
5. Onay sonrasında **abone ol**' u seçin.

## <a name="saas-subscription-and-configuration"></a>SaaS aboneliği ve yapılandırması

Abone ol ' u seçtiğinizde, "SaaS aboneliğiniz devam ediyor" iletisini alırsınız. Bu işlem birkaç dakika sürer, bitene kadar pencereyi kapatmayın.

Abonelik tamamlandığında, SaaS aboneliğinizin tamamlandığını ve hesabınızı, satın alımınızın tadını yararlanmaya başlayacak şekilde yapılandırmanız gerektiğini belirten bir ileti. Ayrıca, yeni aboneliği etkinleştirmenizi isteyen bir e-posta alacaksınız. SaaS hesabını yapılandırabilecek kimse değilseniz, bu e-postayı ilgili kişiye iletin.

İşlemi tamamlayıp SaaS kullanmaya başlamak için aboneliğinizi yapılandırmaya başlamanız gerekir. **Hesabı Şimdi Yapılandır** düğmesini seçerek Publisher 'ın Web sitesine yönlendirilecektir.

Ayrıca, üstbilginin sağ üst köşesindeki ' zil ' simgesini seçerek abonelik durumunuzu kontrol edebilirsiniz.

Yapılandırma işlemini *30 gün* içinde tamamlamazsanız, bu SaaS aboneliği otomatik olarak *silinir*. Faturalama, hesabınız yayımcının Web sitesinde yapılandırıldıktan sonra başlayacaktır.

İşlem sırasında karşılaşabileceğiniz hata iletileri:

- *Seçilen planın plan adı* ücretsiz bir abonelikte satın alınamıyor
  - Hesabınızı yükseltin, https://aka.ms/UpgradeFreeSub daha fazla ayrıntı için bkz..

- Geçerli bir kredi kartı veya Azure aboneliğinizle ilişkili bir ödeme yöntemi bulamadığı için satın alma başarısız oldu.
  - Farklı bir Azure aboneliği kullanın veya bu abonelik için geçerli kredi kartını veya ödeme yöntemini bir veya daha sonra yeniden deneyin.

- *Teklifin yayımcısı tarafından* sunulan teklif *teklifi adı* *SEÇILI planının plan adı* , BT yöneticiniz tarafından ayarlanan kurallar uyarınca satın alma için kullanılamaz.
  - BT yöneticinize başvurun.

- *Bir* teklifin yayımcısı tarafından *Seçilen teklif planı tarafından seçilen* *Plan adı* , kiracının BT Yöneticisi tarafından yapılan özel Market ayarları nedeniyle satın alma için kullanılamaz.
  - BT yöneticinize başvurun

- İstenen faturalandırma dönemi boş veya geçersiz olduğundan satın alma başarısız oldu.
  - Farklı bir plan/fatura dönemi satın almayı deneyin.

- Oturumunuz, yasal anlaşmada oturum açmanızı doğrulayamadığından başarısız oldu.
  - Retry. Hata devam ederse, satın almayı farklı Azure aboneliği kullanarak yapmayı deneyin veya desteğe başvurun.

- Yayımcı *publisherID* Ile teklif *OfferId* 'si satın alma başarısız oldu. Bu teklif şu anda satın alma için kullanılabilir değil.
  - Daha sonra tekrar deneyin. Bu hata iletisini almak için bir saatten sonra lütfen desteğe başvurun.  

- Yayımcı *publisherID* Ile teklif *OfferId* planının plan *PlanID* 'si satın alınamadı. Bu plan şu anda satın alma için kullanılabilir değil.
  - Daha sonra tekrar deneyin. Bu hata iletisini almak için bir saatten sonra lütfen desteğe başvurun.

- Nesne kimliği *ObjectID* olan istemci *e-posta adresinin* , kapsam ResourceGroup üzerinde eylem *deploymentvalidationaction* gerçekleştirme yetkilendirmesi yok *; DeploymentScope* veya kapsam geçersiz.  
  - Azure aboneliğinde/kaynak grubunda doğru izinleriniz yoksa, bu iletiyi alırsınız.  
    Erişim yakın zamanda verildiyse, lütfen kimlik bilgilerinizi yenileyin.  
    Kaynakları bir kaynak grubuna dağıtmak için en az katkıda bulunan erişiminizin olması gerekir. **Kaynak grupları** altında erişim durumunuzu denetleyip **Access Control**. ' Sahip ' ne olduğunu, sizi ' katkıda bulunan ' olarak atamayı istemediğinizi gösterir.

- Bu satın alma için kullanılan abonelik Market satın alımlara izin vermez.  
  - Lütfen farklı bir abonelik kullanın veya yöneticinizden bu aboneliğin tanımını değiştirmesini isteyin ve yeniden deneyin.

## <a name="next-steps"></a>Sonraki adımlar

- Market 'te zaten bir teklif satın aldıysanız [faturalandırma ve faturalama](billing-invoicing.md) ' ya gidin.
- [Özel planlar](private-plans.md) hakkında daha fazla bilgi edinin
