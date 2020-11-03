---
title: Ortak satış başvuruları bağlayıcıları sorunlarını giderme
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ortak satış bağlayıcıları kullanma hakkında sık sorulan soruların yanıtlarını öğrenin. Ortak satış bağlayıcılarının sorunlarını giderme hakkında bilgi edinmek için bu SSS bölümüne bakın.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 988a696a8a0a0abb4d37e3915c76f905ec5b35b0
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/14/2020
ms.locfileid: "92531890"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Ortak satış başvuruları bağlayıcıları sorunlarını giderme

**Aşağıdakiler cihazlar için geçerlidir:**

- İş Ortağı Merkezi
- Dynamics 365 CRM
- Salesforce CRM

**Uygun roller**

- Başvuru Yöneticisi
- CRM 'de Sistem Yöneticisi veya sistem özelleştiricisi

 ## <a name="questions-and-answers-about-pre-requisites"></a>Ön koşullar hakkında sorular ve yanıtlar

1. Ortamınız için bir deneme ortak satışı başvuruları Bağlayıcısı çözümü kullanabilir miyim?

Test/hazırlama ortamındaysanız, deneme çözümünü kabul edebilirsiniz. Bağlayıcıların ücretli sürümü, AppSource 'ta ABD $15/ay 'da bulunabilir. Ücretli bağlantıyla, günde 10.000 API çağrısı elde edersiniz. Bağlayıcılar, Iş ortağı merkezi başvuru API 'lerinin en üstünde sarmalayıcılardır. Her iki Iş ortağı merkezi veya CRM tarafında fırsatlarda bir **oluşturma** veya **güncelleştirme** olayı için BAĞLAYıCı çözümleri çalıştırıldığında bir API çağrısı yapılır.

2. CRM ortamında bölüm oluşturmak için hangi rolü kullanmanız gerekir?

Sistem yöneticileri veya sistem özelleştiricileri olan kullanıcılar herkes için değişiklik uygulayabilir. Ancak tüm uygulama kullanıcıları, sistemi kişiselleştirebilir ve hatta bazı özelleştirmelerini başkalarıyla paylaşabilir. 

3. İş ortağı satıcıları iş ortağı merkezi 'nde çalışmak için özel rollere ihtiyaç duyuyor mu?
 
İş ortağı satıcılara "başvuru Yöneticisi" rolü atanmalıdır. Daha fazla bilgi için, şu [Izinlere genel bakış) bakın (oluşturma-Kullanıcı-hesaplar-ve-ayarla-izinler).

4. CRM ortamınızda ilk olarak hangi alanların ayarlanması gerekir? 

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

- Iş ortağı merkezi kimlik bilgilerinizi kullanarak Flow ortamında bir kez oturum açın (flow.microsoft.com).


3. Power otomatikleştir platformunda Iş ortağı merkezini CRM akışına etkinleştirirken aşağıdaki hatayı alırsanız ne yapmalısınız?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Oturum açma gerektiren hata iletisi":::

Bu sorun giderme adımlarını izleyin:

- Iş ortağı merkezini CRM akışına etkinleştirmeden önce aşağıdaki iki alt akışı etkinleştirin.
      - İş Ortağı Merkezi 'ne CRM Yardımcısı (Insider Preview)
      - İş Ortağı Merkezi Microsoft ortak-CRM 'ye başvuru güncelleştirmeleri satma (Insider Preview)

4. Akışı düzenlemeye çalıştığınızda akışla bağlantı ekleyemeyebilirsiniz ne yapmalısınız?

Akış çalışırken akışa bağlantı ekler ve her bir akışa ayrı olarak eklersiniz.  Bağlantı ekleme iletişim kutusu akışı düzenlerken otomatik olarak açılmazsa, akışların her birini ve alt adımını ayrı ayrı düzenleyebilirsiniz.

- Her bir akışı seçin ve tek tek düzenleyin.
- Akıştaki tüm adımları Genişlet 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Oturum açma gerektiren hata iletisi":::

- Bağlantıları ilişkilendirmek ve bağlantı eklemek isteyen bir uyarı simgesi gördüğünüz adımları seçin. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Oturum açma gerektiren hata iletisi":::


5. Ortak satış başvuruları bağlayıcılar çözümünün akışları açık değilse ne yapmalısınız?

A. Power otomatikleştirmede akışları aşağıdaki sırayla düzenlemeniz ve doğru bağlantıları kullanacak şekilde güncelleştirmeniz gerekir:

- İş Ortağı Merkezi Web kancası kaydı (Insider Preview)
- Ortak satış başvurusu oluşturma-Salesforce 'a Iş Ortağı Merkezi 'ne (Insider Preview)
- İş Ortağı Merkezi Microsoft ortak-başvuru güncelleştirmelerini Salesforce 'a satma (Insider Preview)
- İş ortağı merkezini Salesforce 'a (Insider Preview)
- Salesforce-Iş Ortağı Merkezi (Insider Preview)
- Salesforce Iş Ortağı Merkezi (Insider Preview)
- Salesforce Microsoft çözümlerini Iş Ortağı Merkezi 'ne (Insider Preview)

 B. Her akış için **yalnızca kullanıcıları Çalıştır** seçeneğini belirleyin. **Yalnızca çalıştırma kullanıcısı tarafından sağlanarak** **bağlantı kullan** ' ı seçin.  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Oturum açma gerektiren hata iletisi":::


C. Bu yukarıda belirtilen akışlara aşağıdaki akışları etkinleştirin:

 - İş Ortağı Merkezi Microsoft ortak-başvuru güncelleştirmelerini Salesforce 'a satma (Insider Preview)

- Salesforce-Iş Ortağı Merkezi (Insider Preview)

    
D. Kalan tüm akışları etkinleştirin.

E. Flow Iş Ortağı Merkezi Web kancası kaydında **Çalıştır** ' ı seçin. **Iş Ortağı Merkezi** 'ndeki Ilk eylemden Salesforce akışına **http url 'sini** sağlayın. **Kaydolmak Için olaylar** bölümündeki tüm dört seçeneği seçin ve üzerine yazmak için **Evet** ' i seçin.

## <a name="questions-and-answers-about-runmaintenance"></a>Çalıştırma/bakım ile ilgili sorular ve yanıtlar

1. Güç otomatikleştirme akış yürütmesi sırasında oluşan hatalarda nasıl sorun giderilir?

Güç otomatikleştirebileceğiniz akışlarınızın beklenen şekilde çalıştığından emin olmak ve yürütme sırasında hataların sorunlarını gidermek için bkz. [akış başarısızlıklarını](/power-automate/fix-flow-failures)giderme.

2. Iş ortağı merkezi veya CRM ortamında düzgün şekilde eşitlenmemiş başvurular görürseniz ne yapmalısınız?
 
Başvuru eşitlemesinin durumunu belirlemek için **Denetim** ' i seçin. 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Oturum açma gerektiren hata iletisi":::

Aşağıdaki koşulların karşılandığından emin olun:

- Çözüm kimliği, fırsatın bir parçası olarak sağlanır.

- İki harfli ülke kodu gereklidir.

- Fırsat için Microsoft 'tan yardım seçiliyken müşteri iletişim bilgileri gereklidir.

3. Bir başvurunun çift yönlü olarak eşitlenmesini sağlamak mı istiyorsunuz?

Aşağıdaki adımları uygulayın:

- İş ortaklarının satıcıları, CRM bölümündeki **Iş Ortağı Merkezi Ile eşitlemeyi** etkinleştirdiklerinden emin olmalıdır.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Oturum açma gerektiren hata iletisi" olarak kapanmadığından emin olun.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşteri adaylarını yönetme](manage-leads.md)
 
- [Ortak satış fırsatlarını yönetme](manage-co-sell-opportunities.md)