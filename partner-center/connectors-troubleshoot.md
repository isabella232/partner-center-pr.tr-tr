---
title: Ortak satış referans bağlayıcıları sorunlarını giderme
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ortak satış bağlayıcılarını kullanma hakkında sık sorulan soruların yanıtlarını öğrenin. Ortak satış bağlayıcıları sorunlarını giderme hakkında bu SSS bölümünü okuyun.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 49a2b6e5461dacbe87c34b36805a5c240c2e5fd1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148355"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Ortak satış referans bağlayıcıları sorunlarını giderme

**Için geçerlidir:** Dynamics 365 CRM | Salesforce CRM

**Uygun roller:** Referans yöneticisi | CRM'de sistem yöneticisi veya sistem özelleştiricisi

 ## <a name="questions-and-answers-about-pre-requisites"></a>Önkullar hakkında sorular ve yanıtlar

1. Ortamınız için bir deneme ortak satış referans bağlayıcısı çözümü kullanabilir misiniz?

Test/hazırlama ortamındaysanız deneme çözümünü tercih edin. Bağlayıcıların ücretli sürümü, AppSource'ta aylık 15 ABD doları olarak kullanılabilir. Ücretli bağlantıyla günde 10.000 API çağrısı alasınız. Bağlayıcılar, referans API'lerinin İş Ortağı Merkezi sarmalayıcılardır. Bağlayıcı çözümleri, İş Ortağı Merkezi  veya  CRM tarafındaki fırsatlarda Oluşturma veya Güncelleştirme olayı için her çalıştırısa, bir API çağrısı yapılır.

2. CRM ortamında bölümler oluşturmak için hangi role ihtiyacınız var?

Sistem yöneticisi veya sistem özelleştiricisi olan kullanıcılar değişiklikleri herkes için uygulayabilir. Ancak tüm uygulama kullanıcıları sistemi kişiselleştirenin ve hatta bazı özelleştirmelerini başkalarıyla paylaşabilir. 

3. İş ortağı satıcılarının iş ortaklarına özel rollere ihtiyacı İş Ortağı Merkezi?
 
İş ortağı satıcılarına "Referans yöneticisi" rolü atanmalı. Daha fazla bilgi için bkz. [İzinlere genel bakış.](create-user-accounts-and-set-permissions.md)

4. CRM ortamınıza ilk olarak hangi alanların ayarlanmış olması gerekir? 

• Para biriminiz konumunuza uygun olduğundan ve CRM ortamınızda doğru olduğundan emin olun. • Satış ekibiniz, CRM ortamınızda CRM kullanıcıları olarak listelenmiş olmalıdır.

5. Power otomatikleştirin ortam oluşturma için gerekenler ne gerekir?

Power otomatikleştir ortamını kullanmak için şunlar gerekir:

- Güç otomatikleştirme lisansı gereklidir.
- En az 1 GB depolama alanı gereklidir.

6.  Salesforce bağlayıcıları çözümünü kullanmak için bir Dynamics 365 aboneliğine ihtiyacınız var mı?

Salesforce bağlayıcı çözümü, diğer CRM sistemleriyle eşitlemeyi destekleyen "Dynamics Flow" türüdür. Çözüm, Dynamics 365 örneğine veya aboneliğine sahip olmanızı gerektirmez. Salesforce çözümünü yüklerken şirketinizdeki mevcut CD 'leri içeren bir açılır liste görüntülenebilir. Bu ortamı seçmeniz gerekir. Ayrıca, "oturum açan kullanıcıya bağlı bir Dynamics 365 organizasyonu bulamadık" hatasını alırsanız, bağlayıcı için yeni ortam oluşturmanız gerekir.

## <a name="questions-and-answers-about-configuration"></a>Yapılandırma ile ilgili sorular ve yanıtlar

1. Power otomatikleştir platformunda akışları etkinleştirirken aşağıdaki hatayla karşılaşırsanız ne yapmalısınız?

Hata: Azure Resource Manager Isteği şu hatayla başarısız oldu: ' {"Error": {"Code": "WorkflowTriggerNotFound", "Message": "iş akışı ' e14d00f1-1fdf-4b1b-AAAC-54a5064093d3 ' tetikleyici ' Manual ' bulunamadı."}} '. 

Bu sorun giderme adımlarını izleyin:

- CD bağlantısını silin ve ardından CD bağlantılarını yeniden oluşturun.
- Alt akışı kapatma ve açma 
- Çözümü silin ve çözümü yeniden yükleyin. 

2.  Power otomatikleştir platformunda bir Iş Ortağı Merkezi Bağlayıcısı eklenirken "oturum aç" hatası varsa ne yapmalısınız?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Oturum açma gerektiren hata iletisi":::

Bu sorun giderme adımını izleyin:

- Akış ortamında İş Ortağı Merkezi için kimlik bilgilerinizi kullanın (flow.microsoft.com).


3. Power Automate Platform'da CRM akışına İş Ortağı Merkezi etkinleştirirken aşağıdaki hatayı alırsanız ne Power Automate gerekir?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Güncelleştirme gerektiren hata iletisi":::

Şu sorun giderme adımlarını izleyin:

- CRM akışına yönelik akışı etkinleştirmeden önce aşağıdaki iki İş Ortağı Merkezi akışı etkinleştirin.
      - İş Ortağı Merkezi CRM ' e - Yardımcı (Insider Önizleme)
      - İş Ortağı Merkezi Microsoft'un CRM'ye Ortak Satış Referans Güncelleştirmeleri (Insider Önizlemesi)

4. Akışı düzenlemeye çalışmadan akışa bağlantı ekleye değilken ne yapacaksınız?

Akış çalışırken akışa bağlantılar ekler ve her akışa ayrı bağlantılar eklersiniz.  Bağlantı ekleme iletişim kutusu akışı düzenlerken otomatik olarak açılmazsa, akışların adımlarını ve alt adımlarını tek tek düzenleyebilirsiniz.

- Her akışı seçin ve ayrı ayrı düzenleyin.
- Akışta tüm adımları genişletin 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Bağlantı gereken adımlar":::

- Bağlantıları ilişkilendirmek ve bağlantı eklemek için bir uyarı simgesi gördüğünüz adımları seçin. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Akışı adım adım düzenleme":::


5. Ortak Satış Referansları Bağlayıcıları çözümünün akışları açık yoksa ne yapacaksınız?

A. Bu Power Automate, akışları aşağıdaki sırayla düzenlemeniz ve doğru bağlantıları kullanmak üzere güncelleştirmeniz gerekir:

- İş Ortağı Merkezi Web Kancası Kaydı (Insider Önizlemesi)
- Ortak satış başvurusu oluşturma-Salesforce 'a Iş Ortağı Merkezi 'ne (Insider Preview)
- İş Ortağı Merkezi Microsoft ortak-başvuru güncelleştirmelerini Salesforce 'a satma (Insider Preview)
- İş ortağı merkezini Salesforce 'a (Insider Preview)
- Salesforce-Iş Ortağı Merkezi (Insider Preview)
- Salesforce Iş Ortağı Merkezi (Insider Preview)
- Salesforce Microsoft çözümlerini Iş Ortağı Merkezi 'ne (Insider Preview)

 B. Her akış için **yalnızca kullanıcıları Çalıştır** seçeneğini belirleyin. **Yalnızca çalıştırma kullanıcısı tarafından sağlanarak** **bağlantı kullan** ' ı seçin.  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Bir akışı etkinleştirmek için":::


C. Bu yukarıda belirtilen akışlara aşağıdaki akışları etkinleştirin:

 - İş Ortağı Merkezi Microsoft ortak-başvuru güncelleştirmelerini Salesforce 'a satma (Insider Preview)

- Salesforce-Iş Ortağı Merkezi (Insider Preview)

    
D. Kalan tüm akışları etkinleştirin.

E. Flow Iş Ortağı Merkezi Web kancası kaydında **Çalıştır**' ı seçin. **Iş Ortağı Merkezi** 'ndeki Ilk eylemden Salesforce akışına **http url 'sini** sağlayın. **Kaydolmak Için olaylar** bölümündeki tüm dört seçeneği seçin ve üzerine yazmak için **Evet** ' i seçin.

## <a name="questions-and-answers-about-runmaintenance"></a>Çalıştırma/bakım ile ilgili sorular ve yanıtlar

1. Power otomatikleştirin akış yürütme sırasında hatalardan nasıl sorun giderilir?

Güç otomatikleştirebileceğiniz akışlarınızın beklenen şekilde çalıştığından emin olmak ve yürütme sırasında hataların sorunlarını gidermek için bkz. [akış başarısızlıklarını](/power-automate/fix-flow-failures)giderme.

2. Iş ortağı merkezi veya CRM ortamında düzgün şekilde eşitlenmemiş başvurular görürseniz ne yapmalısınız?
 
Referans eşitleme durumunu belirlemek için Denetle'yi **seçin.** 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Referansları eşitleme":::

Aşağıdaki koşulların karşı olduğundan emin olmak:

- Çözüm kimliği, fırsatın bir parçası olarak sağlanır.

- İki harfli ülke kodu gereklidir.

- Fırsat için Microsoft'tan yardım seçildiğinde müşteri iletişim bilgileri gereklidir.

3. Bir referansın çift yönlü olarak eşitlenmesi nasıl sağlandı?

Aşağıdaki adımları uygulayın:

- İş ortağı satıcılarının CRM bölümünde İş Ortağı Merkezi **eşitle seçeneğini etkinleştirmiş** olduğundan emin olmalıdır.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Eşitleme'yi etkinleştirildiğinden emin olun":::

- Satış satıcılarının müşteri adayını kabul etmek için gelir ve kapanış tarihi sağlamaları gerekir.

- CRM Kimliği ortak satış  fırsatının oluşturma veya güncelleştirme aşamasında sağlanıyorsa ancak CRM'de bu kimliğin bulunduğu bir müşteri adayı fırsatı yoksayılırsa güncelleştirme veya oluşturma yoksayılır. 

- Referans para birimi alanını Salesforce ortamında yapılandırıldığından emin olmak. 

4. Bağlayıcının bağlantısı kesilirse ve referans eşitlemesini kaçırırsanız ne yapacaksınız?

Deneyebilirsiniz seçeneklerden birkaçı şunlardır:

- Referans yöneticisi rollerine sahip kullanıcı adı veya parolanın İş Ortağı Merkezi olup olmadığını kontrol edin.

- Eşitlenmemiş fırsata gidebilir, küçük bir güncelleştirme gerçekleştirip referansın eşitlenmiş olup olmadığını gözlemlersiniz.

- Akışlar çalıştırlı ve başarısız olmuşsa akışı seçin ve başarısız olan çalıştırmayı yeniden gönderin.

5. Erişim reddedildi hatalarına sahip olursanız ne yapacaksınız?

Uygun rollerin mevcut olduğundan emin olun

- Iş Ortağı Merkezi satıcı için başvuru Yöneticisi rolü 
 
- CRM örneğiniz üzerinde sistem yöneticisi veya sistem özelleştirici rolü

- Power otomatikleştirmenin akış hesabı kullanıcısının https://flow.microsoft.com önceden en az bir kez oturum açtığına sahip olduğundan emin olun

6. Ortak satış fırsatı oluştururken **müşteri hesabı ülke kodunun** eksik olduğunu görürseniz, ne yapmanız gerekir?

ISO 'nın iki harfli ülke kodunu CRM 'de müşteri hesabına eklemeniz gerekir.

7. Ortak satış fırsatı oluştururken **Çözüm Kimliği 'nin gerekli** olduğu hatayı görürseniz ne yapmanız gerekir?

Ortak satış başvurusu oluşturmak için, Microsoft ortak satış için kullanabileceğiniz bir çözüme ihtiyacınız vardır. 

8. Iş akışı hatası olmasa dahi, Iş Ortağı Merkezi 'nde oluşturulmuş ortak satış fırsatlarını gördüğünüzde ne yapmalısınız?

Şunları yapın:

- Iş Ortağı Merkezi 'nde yeni bir ortak satış sorunu oluşturduktan sonra, Dynamics 365 Flow Iş Ortağı Merkezi 'nin çağrılacağını (birden çok kez çağrılabilir) denetleyin.

- Akış çağrılırsa, tüm çağrılan Akışlar ' ı işaretleyin ve bu, CRM 'yi güncelleştiren akış çalıştırmasını belirler. Eylemleri izleyebilir ve CRM 'yi güncelleştirip güncelleştirmediğinizi veya bir sorunla karşılaştıysanız emin olabilirsiniz.

- CRM KIMLIĞIYLE doldurulup doldurulmadığını görmek için Iş Ortağı Merkezi 'nde **yeni anlaşmayı** denetleyin.

- Iş Ortağı Merkezi 'nde, anlaşmayı **kazanıldı** veya **kaybedildi** olarak kapanmadığından emin olun.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşteri adaylarını yönetme](manage-leads.md)
 
- [Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)
