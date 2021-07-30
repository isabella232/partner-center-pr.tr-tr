---
title: Azure aboneliğini başka bir ortağa aktarma
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: müşterinin Azure abonelikleri ile ilişkili Bulut Çözümü Sağlayıcısı program ortağını değiştirme hakkında bilgi edinin.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 07/21/2021
ms.openlocfilehash: c1bc82e852c6777bc9e8c01a33b0976269e31b2f
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114843604"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Müşterinin Azure aboneliklerini başka bir iş ortağına aktarmayı öğrenin

**Uygulama hedefi**: Iş Ortağı Merkezi | Microsoft Cloud for US Government için iş ortağı Merkezi

**Uygun roller**: genel yönetici

bu makalede, bir müşterinin önceki Azure teklifini CSP 'de satın aldıklarında Microsoft Azure hizmetlerini bir Bulut Çözümü Sağlayıcısı (csp) ile diğerine nasıl geçtikleri açıklanmaktadır.

CSP ['deki önceki Azure teklifine](https://go.microsoft.com/fwlink/p/?linkid=2164140)yaptığımız değişikliklerin 1. aşamasından sonra, CSP programındaki iş ortakları ve müşteriler arasındaki mevcut tüm satıcı ilişkileri için, müşteri zaten satın almışsa, iş ortağı önceki Azure teklıfını (MS-azr-0145p) Transact 'a devam edebilir. İş ortakları ve müşteriler arasındaki mevcut tüm satıcı ilişkileri için, müşteri önceki Azure teklifini daha önce satın almamışsa, iş ortağı yalnızca yeni Azure teklifini kullanabilir.

- Hem **geçerli hem de gelecekteki iş ortağının bir müşteriyle birlikte etkin olan önceki Azure teklifi abonelikleri varsa**, bu belgede geçerli ve gelecekteki iş ortakları arasında açıklanan önceki Azure teklıfı (MS-azr-0145p) aktarımları, her iki iş ortağı etkin önceki Azure teklifi aboneliklerini koruduktan sonra, 1. aşama sonrasında kullanılabilir olmaya devam edecektir. Bu aktarım yeteneği, gelecekteki bir iş ortağı artık etkin bir önceki Azure teklifi aboneliğine sahip olmadığında veya CSP 'deki önceki Azure teklifi (MS-AZR-0145p), 3. aşamada kalıcı olarak devre dışı bırakıldığında sona erecek.

   > [!NOTE]
   > Bu senaryo için bir otomatik alet yok ve aşağıdaki işlem yararlanılabilir olmalıdır.

- **Yalnızca geçerli ortağın etkin bir önceki Azure teklifi (MS-AZR-0145p) aboneliği olan bir müşterisi varsa ve gelecekteki iş ortağı yoksa**, iş ortakları arasında önceki Azure teklifinin aktarımı artık 1. aşamadan sonra mümkün olmayacaktır. Gelecekteki iş ortağı müşteri için önceki bir Azure teklifi (MS-AZR-0145p) aboneliği oluşturmadığından, bu aktarım etkinleştirilmez. Bu durumda, bu geçiş aracı, aynı anda yeni bir Azure teklifi aboneliğine dönüştürülürken müşterinin Azure aboneliğini CSP 'deki iş ortakları arasında taşımak için kullanılabilir.

Bir müşterinin Azure hizmetlerini veya aboneliklerini önceki Azure teklifiyle (MS-AZR-0145p) farklı bir ortağa geçirmek için bu el ile adımları izleyin. Hem iş ortağının hem de müşterinin adımları tamamlaması gerekir.

> [!NOTE]  
> Şu anda yalnızca doğrudan veya dolaylı sağlayıcılar abonelikleri aktarabilir.
> Azure plan, Office 365, Enterprise Mobility Suite veya Microsoft Dynamics CRM abonelikleri ile ilişkili Bulut Çözümü Sağlayıcısı abonelikleri için iş ortaklarını değiştiremezsiniz.

## <a name="transfer-azure-subscriptions-to-another-partner-with-the-previous-azure-offer"></a>Önceki Azure teklifiyle Azure aboneliklerini başka bir ortağa aktarma

1. Bir Azure aboneliğini önceki Azure teklifiyle yeni bir ortağa aktarmak için, müşterinin işlemi başlatması ve yazılı kayıt ortağıyla iletişim kurabilmesi gerekir.

   > [!NOTE]
   > Bu, aktarım sürecini başlatan hizmet bileti oluşturmak için geçerli ortağın sorumluluğudur. Microsoft, müşteri veya yeni iş ortağı adına müdahale edemez. Müşteri, geçişi sorunsuz bir şekilde hareket etmek için geçerli iş ortağıyla yakından çalışmayı planlıyor olmalıdır.

2. Aboneliğin iş ortağının aşağıdaki görevleri yapması gerekir:

   Abonelik aktarımı istemek için Iş Ortağı Merkezi 'nden bir Azure hizmet bileti oluşturun:

   1. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin, listeden müşteriyi seçin ve ardından **hizmet yönetimi**' ni seçin.
   2. **Destek biletleri** bölümünde **yeni bilet** açılan listesini seçin ve **Microsoft Azure**' yi seçin.
   3. [Azure Portal](https://portal.azure.com) **Yeni destek isteği**' ni seçin.
   4. adım 1 ' de, sorun türü olarak **abonelik yönetimi** ' ni seçin, aktarılmasını istediğiniz abonelik kimliğini belirtin ve destek planı olarak **Bulut Çözümü Sağlayıcısı** seçin.
   5. 2. adımda, **C-en az etkisi** ' nı seçin ve sorun türü olarak **diğer genel sorular** ' ı seçin.
   6. [CSP abonelik aktarma formunu](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)indirin.

3. Abonelik için iş ortağı: [CSP abonelik aktarımı formunu](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)doldurup imzalayın ve müşteriye gönderin. 

   Formu tamamlayabilmeniz için aşağıdaki bilgilere ihtiyacınız vardır:

   - Geçerli ortağın iletişim bilgileri ve Microsoft KIMLIĞI. İş Ortağı Merkezi menüsünde **Hesap ayarları** &gt; **kuruluş profili**' ni seçin ve burada listelenen **Microsoft kimliği**, **kuruluş adı** ve **adresi** kullanın.
   - Müşterinin Microsoft KIMLIĞI. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve **Microsoft kimliklerini** görmek için müşterinin listesini genişletin.
   - Aktarılacak abonelik KIMLIĞI. Genişletilmiş müşteri listesinde, **abonelikleri görüntüle**' yi seçin ve ardından **abonelik kimliğini** görmek için seçilen aboneliği genişletin.

   > [!NOTE]
   > Abonelik aktarma işlemi, aktarılan aboneliğin **abonelik düzenleme** sayfasında göreceğiniz Iki abonelik kimliğiyle sonuçlanır: **1**-Iş Ortağı Merkezi abonelik kimliği Faturalandırma amacıyla kullanılır. **2**-özgün Azure abonelik kimliği korunur ve Azure yönetim portalı 'nda olduğu gibi Iş Ortağı Merkezi 'nde de görüntülenir. Bu KIMLIK, keşfi dosyanızda görünür.  **Destek biletlerini günlüğe kaydederken, her iki kimliği de kullanmanız gerekir.**

4. Abonelik için müşteri ve yeni iş ortağı:

   Formu gözden geçirin, yeni iş ortağı hakkındaki bilgileri girin ve imzalayın. Yeni müşterinin bir sözleşme anlaşması olduğunu onaylayın. Formu geçerli kayıt iş ortağına geri gönderin.

   *Önemli*: yeni CSP ortağının müşteriyle bir satıcı ilişkisi yoksa, abonelik aktarılmadan önce bir tane kurması gerekir. [Bunun nasıl yapılacağı hakkında daha fazla bilgi edinmek için burada bulabilirsiniz](request-a-relationship-with-a-customer.md).

   > [!NOTE]
   > Yeni CSP iş ortağı ve müşteri kiracının aynı ülkede olması gerekir. 

5. Geçerli iş ortağı:

   Formun hem iş ortağı yöneticileri için iletişim bilgilerini içerdiğinden emin olun. Microsoft Desteği, aktarımı doğrulamak için her iki yönetici ile iletişim kuracaktır. Üç imzaya de sahip olduğunuzdan emin olun. ardından, tamamlanmış formu mevcut hizmet isteğinize eklemek için **dosya Upload** seçeneğini kullanın. Microsoft Destek Mühendisi, giriş ve tamamlamayı doğrulamak için sekiz iş saati içinde size geri dönecek.

6. Yeni iş ortağı:

   Eski ortağı hesaptan kaldırmak için Azure abonelik ayarlarını güncelleştirin. Hangi rol atamalarının sağlandığını görmek için iki PowerShell cmdlet 'i çalıştırın.

   - Yeni iş ortağını hesaba satıcı olarak ekleyin:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     > [!NOTE]
     > Müşterinin **KIRACı kimliği** , Iş Ortağı Merkezi 'Nde MÜŞTERININ **Microsoft kimliği** olarak görünür. Belirli bir müşterinin Microsoft KIMLIĞINI (kiracı KIMLIĞI) bulmak için Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın. Ardından menüden **müşteriler** ' i seçin. Listedeki müşteriyi bulun. Müşterinin listesini genişletmek için aşağı oku seçin. Müşterinin *etki alanı adı* ve MÜŞTERININ **Microsoft kimliği** hakkındaki bilgileri görürsünüz. PowerShell commandlet 'teki 16 basamaklı **MICROSOFT kimliğini** kullanın.

   - Önceki CSP iş ortakları da dahil olmak üzere hesaptaki rolleri görüntüleyin:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Eski erişim izinlerini kaldır:

   1. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin.
   1. Listedeki müşteriyi bulun. Şirket adlarını seçin (çift tıklayın). Bu eylem, müşteri **abonelikleri** sayfasını açar.
   1. Müşteri ayrıntısı menüsünde **hizmet yönetimi**' ni seçin.
   1. **Microsoft Azure** altında **Microsoft Azure Yönetim Portalı** bağlantısını seçin.

## <a name="next-steps"></a>Sonraki adımlar

- [Azure aboneliklerini aktarma](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)
- [Azure aboneliklerini Azure planına aktarma](transfer-azure-subscriptions-under-azure-plan.md)
- [CSP abonelik aktarma formunu](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC) indirin
- [Çoklu iş ortağı desteği](multipartner.md) hakkında bilgi edinin
- [Çoklu kanallı destek](multichannel.md) hakkında bilgi edinin
