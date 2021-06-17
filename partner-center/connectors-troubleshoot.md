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
ms.openlocfilehash: bb7a227624c548a29046b80d3bd5fa363a4aee2f
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276951"
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

• Para biriminizin konumunuz için uygun olduğundan ve CRM ortamınıza uygun olduğundan emin olun. • Satış takımınız CRM ortamınıza CRM kullanıcıları olarak listelenmiş olmalı.

5. Ortam oluşturmak için hangi önk Power Automate gerekir?

Ortam ortamını Power Automate için aşağıdakiler gerekir:

- Bir Power Automate lisansı gereklidir.
- En az 1 GB depolama gereklidir.

6.  Salesforce Bağlayıcıları çözümünü kullanmak için Dynamics 365 aboneliğine ihtiyacınız var mı?

Salesforce Bağlayıcısı çözümü, diğer CRM sistemleriyle eşitlemeyi destekleyen "Dynamics Flow" türündedir. Çözüm için Dynamics 365 örneğine veya aboneliğe sahip olmak gerekli değildir. Salesforce çözümünü yüklerken, şirketiniz içinde var olan CDS ortamına sahip bir açılan liste görünebilir. Bu ortamı seçmeniz gerekir. Ayrıca, "Oturum alıkan kullanıcıya bağlı bir Dynamics 365 kuruluşu bulamadı" hatasını alırsanız bağlayıcı için yeni bir ortam oluşturmanız gerekir.

## <a name="questions-and-answers-about-configuration"></a>Yapılandırmayla ilgili sorular ve yanıtlar

1. Power Automate Platform'da akışları etkinleştirirken aşağıdaki hatayla karşılaşıyorsanız ne Power Automate gerekir?

Hata: Azure Resource Manager isteği şu hatayla başarısız oldu: '{"error":{"code":"WorkflowTriggerNotFound","message":"'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' tetikleyicisi 'manual' bulunamadı."}}'. 

Şu sorun giderme adımlarını izleyin:

- CDS bağlantısını silin ve ardından CDS bağlantılarını yeniden oluşturun.
- Alt akışı kapatma ve açma 
- Çözümü silin ve çözümü yeniden yükleyin. 

2.  Power Automate Platform'da bir İş Ortağı Merkezi bağlayıcısı eklerken "Oturum açma" hatasıyla karşılaşıyorsanız ne Power Automate gerekir?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Oturum açma gerektiren hata iletisi.":::

Bu sorun giderme adımını izleyin:

- Akış ortamında İş Ortağı Merkezi için kimlik bilgilerinizi kullanın (flow.microsoft.com).


3. Power Automate Platform'da CRM akışına İş Ortağı Merkezi etkinleştirirken aşağıdaki hatayı alırsanız ne Power Automate gerekir?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Güncelleştirme gerektiren hata iletisi.":::

Şu sorun giderme adımlarını izleyin:

- CRM akışına yönelik akışı etkinleştirmeden önce aşağıdaki iki İş Ortağı Merkezi akışı etkinleştirin.
      - İş Ortağı Merkezi CRM ' e - Yardımcı (Insider Önizleme)
      - İş Ortağı Merkezi Microsoft'un CRM'ye Ortak Satış Referans Güncelleştirmeleri (Insider Önizlemesi)

4. Akışı düzenlemeye çalışmadan akışa bağlantı ekleye değilken ne yapacaksınız?

Akış çalışırken akışa bağlantılar ekler ve her akışa ayrı olarak eklersiniz.  Bağlantı ekleme iletişim kutusu akışı düzenlerken otomatik olarak açılmazsa, akışların adımlarını ve alt adımlarını tek tek düzenleyebilirsiniz.

- Her akışı seçin ve ayrı ayrı düzenleyin.
- Akışta tüm adımları genişletin 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Bağlantı gereken adımlar.":::

- Bağlantıları ilişkilendirmek ve bağlantı eklemek için bir uyarı simgesi gördüğünüz adımları seçin. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Akışı adım adım düzenleyin.":::


5. Ortak Satış Referansları Bağlayıcıları çözümünün akışları açık yoksa ne yapacaksınız?

A. Bu Power Automate, akışları aşağıdaki sırayla düzenlemeniz ve doğru bağlantıları kullanmak üzere güncelleştirmeniz gerekir:

- İş Ortağı Merkezi Web Kancası Kaydı (Insider Önizlemesi)
- Ortak Satış Referansı Oluşturma - İş Ortağı Merkezi salesforce (Insider Önizleme)
- İş Ortağı Merkezi Microsoft Ortak Satış Referans Güncelleştirmelerini Salesforce'a (Insider Önizleme) yönlendirme
- İş Ortağı Merkezi'a (Insider Önizleme)
- Salesforce'tan İş Ortağı Merkezi 'a (Insider Önizleme)
- Salesforce Opportunity to İş Ortağı Merkezi (Insider Preview)
- İş Ortağı Merkezi için Salesforce Microsoft Solutions (Insider Önizleme)

 B. Akışın her biri için Yalnızca kullanıcıları **çalıştır seçeneğini** belirleyin. Yalnızca **çalıştıran kullanıcı** tarafından **sağlanan yerine Bağlantıyı kullan'ı seçin.**  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Akışı etkinleştirmek için.":::


C. Aşağıda belirtilen akışları etkinleştirin:

 - İş Ortağı Merkezi Microsoft Ortak Satış Referans Güncelleştirmelerini Salesforce'a (Insider Önizleme) yönlendirme

- Salesforce'tan İş Ortağı Merkezi 'a (Insider Önizleme)

    
D. Kalan tüm akışları etkinleştirin.

E. Web Kancası İş Ortağı Merkezi akışında Çalıştır'ı **seçin.** **İş Ortağı Merkezi'de Salesforce akışına ilk eylemden http URL'sini** girin.  Kaydolmak için Olaylar altında dört **seçeneğin de hepsini seçin ve Üzerine** Yaz için **evet'i** seçin.

## <a name="questions-and-answers-about-runmaintenance"></a>Çalıştırma/Bakım hakkında sorular ve yanıtlar

1. Akış yürütme sırasındaki hataları Power Automate giderin?

Akış akışlarının beklediğiniz Power Automate olduğundan emin olmak ve yürütme sırasındaki hataları gidermek için [bkz. Akış hatalarını düzeltme.](/power-automate/fix-flow-failures)

2. İş Ortağı Merkezi VEYA CRM ortamında düzgün eşitlenmemiş referanslar görüyorsanız ne yapacaksınız?
 
Referans eşitleme durumunu belirlemek için Denetle'yi **seçin.** 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Referansları eşitleme.":::

Aşağıdaki koşulların karşı olduğundan emin olmak:

- Çözüm kimliği, fırsatın bir parçası olarak sağlanır.

- İki harfli ülke kodu gereklidir.

- Fırsat için Microsoft'tan yardım seçildiğinde müşteri iletişim bilgileri gereklidir.

3. Bir referansın çift yönlü olarak eşitlenmesi nasıl sağlandı?

Aşağıdaki adımları uygulayın:

- İş ortağı satıcılarının CRM bölümünde İş Ortağı Merkezi **eşitle seçeneğini etkinleştirmiş** olduğundan emin olmalıdır.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Eşitle'yi etkinleştirdikten emin olun.":::

- Satış satıcılarının müşteri adayını kabul etmek için gelir ve kapanış tarihi sağlamaları gerekir.

- CRM Kimliği ortak satış  fırsatının oluşturma veya güncelleştirme aşamasında sağlanıyorsa ancak CRM'de bu kimliğin bulunduğu bir müşteri adayı fırsatı yoksayılırsa güncelleştirme veya oluşturma yoksayılır. 

- Referans para biriminin Salesforce ortamında yapılandırıldığından emin olmak. 

4. Bağlayıcının bağlantısı kesilirse ve referans eşitlemesini kaçırırsanız ne yapacaksınız?

Deneyebilirsiniz seçeneklerden birkaçı şunlardır:

- Iş Ortağı Merkezi kullanıcısı için başvuru yöneticisi rollerine sahip kullanıcı adının veya parolanın dolup dolmadığını denetleyin.

- Eşitlenmemiş fırsata gidebilir, küçük bir güncelleştirme yapabilir ve başvurunun eşitlenip eşitlenmediğini gözlemleyebilirsiniz.

- Akışlar çalıştırılmışsa ve başarısız olursa, akışı seçip başarısız olan çalıştırmayı yeniden gönderebilirsiniz.

5. Erişim reddedildi hatalarını aldığınızda ne yapmalısınız?

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
