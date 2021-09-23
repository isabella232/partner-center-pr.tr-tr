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
ms.openlocfilehash: b9ce8fff5915d3d4bf42f699c5a0c9130e37814b
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/23/2021
ms.locfileid: "128322127"
---
# <a name="transfer-a-customers-azure-subscriptions-to-a-different-partner-without-converting-them-to-an-azure-plan"></a>Müşterinin Azure aboneliklerini bir Azure planına dönüştürmeden farklı bir ortağa aktarma

**Uygulama hedefi**: Iş Ortağı Merkezi | Microsoft Cloud for US Government için iş ortağı Merkezi

**Uygun roller**: genel yönetici

bu makalede, bir müşterinin geçerli Bulut Çözümü Sağlayıcısı (CSP) olan bir Azure aboneliğini başka bir CSP 'ye nasıl aktarabilmesi açıklanmaktadır.

bir [Azure aboneliğini başka bir ortağa aktarmak için](#transferring-azure-subscriptions-to-another-partner)birinci bölüm, bir müşterinin bir Bulut Çözümü Sağlayıcısı (CSP) Microsoft Azure aboneliğini diğerine nasıl aktarabileceğinizi açıklar.

Sonraki bölümde, Azure [planına dönüştürmeden önceki bir Azure teklif aboneliğini aktarma](#transferring-a-previous-azure-offer-subscription-without-converting-it-to-the-azure-plan)işlemi, yeni Azure planının nasıl sunulmakta olduğunu kısaca açıklar. Daha sonra, önceki Azure teklifinin bazı aboneliklerinin yeni Azure planına dönüştürülmeksizin başka bir CSP 'ye aktarılabileceği özel bir durum açıklanır.

Müşteri, geçerli hizmet sağlayıcısı ve yeni bir hizmet sağlayıcısının hepsi, bir [Müşteri aboneliğini yeni bir Azure hizmet sağlayıcısına aktarırken sorumluluklara](#responsibilities-when-transferring-a-customer-subscription-to-a-new-azure-service-provider)sahiptir. Bir müşteri, geçişi sorunsuz hale getirmek için geçerli iş ortağıyla yakından çalışmayı planlıyor olmalıdır.

 Azure aboneleri 'nin CSP iş ortaklarına ve aboneliklerine abonelik aktarmasına yardımcı olan üst düzey bilgiler, [aboneler ve CSP 'ler arasında Azure aboneliklerini aktarma](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)bölümünde bulunabilir.

Müşterilerin Azure aboneliklerini bir iş ortağından diğerine nasıl değiştirebilmeleri hakkında ek bilgiler, [müşterinin Azure aboneliklerini farklı bır CSP 'ye aktarma (bir Azure planı altında)](./transfer-azure-subscriptions-under-azure-plan.md)

## <a name="prerequisites"></a>Önkoşullar

- Bir aboneliğin aktarılması için bir CSP Iş ortağı bir müşteri ile satıcı ilişkisine sahip olmalıdır.  Daha fazla bilgi için bkz. [Iş Ortağı Merkezi 'nde bir müşteriden satıcı ilişkisi isteme](./request-a-relationship-with-a-customer.md).
- Bir iş ortağı bir aboneliği aktarmak için doğrudan sağlayıcı veya dolaylı bir sağlayıcı olmalıdır.
- aşağıdaki tekliflerle ilişkili abonelikler aktarılamaz: Azure planı, Office 365, Enterprise Mobility Suite ve Microsoft Dynamics CRM.
- Bir müşterinin bir aboneliği aktarabilmesi için bir iş ortağıyla aynı ülkede olması gerekir.
- Microsoft Cloud for US Government veya Microsoft Bulut almanya 'da çalışan iş ortaklarının bir müşterinin hizmetini veya aboneliğini yönetmek için izin istemesi gerekir. Daha fazla bilgi için bkz. [bir müşterinin hizmetini veya aboneliğini yönetme Izinleri alma](./customers-revoke-admin-privileges.md).

## <a name="transferring-azure-subscriptions-to-another-partner"></a>Azure aboneliklerini başka bir ortağa aktarma

Bir Azure aboneliğini bir CSP ortağından diğerine aktarmak, müşteri, geçerli iş ortağı ve çeşitli aşamalardaki yeni iş ortağı için eylem gerektiren çok adımlı bir işlemdir. Aşağıdaki tablo kimin ve ne zaman yaptığını açıklığa kavuşturmasına yardımcı olmak için bir sıralı diyagram olarak hazırlanmıştır.

### <a name="responsibilities-when-transferring-a-customer-subscription-to-a-new-azure-service-provider"></a>Bir müşteri aboneliğini yeni bir Azure hizmet sağlayıcısına aktarırken oluşan sorumluluklar

|Adım  |Müşteri  |Geçerli iş ortağı  |Yeni iş ortağı  |
|---------|---------|---------|---------|
|1     |[Müşteri Microsoft ve geçerli iş ortağını yazılı olarak bildirir](#step-1-customer-contacts-current-partner-in-writing)         |         |         |
|2     |         |[Aktarım isteğinde bulunan destek bileti oluştur](#step-2-current-provider-creates-azure-support-ticket-to-request-a-transfer)        |         |
|3     |         |[Tamamlanan aktarım formunu müşteriye gönder](#step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer)|         |
|4     |         |[Bulut Çözümü Sağlayıcısı form değişikliğini tamamlanma](#step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer)       |         |
|5     |[İnceleme, imzalama, & dönüş formu](#step-5-the-customer-and-new-partner-review--return-the-form)       |         |[İnceleme, imzalama, & dönüş formu](#step-5-the-customer-and-new-partner-review--return-the-form)         |
|6     |         |[Formu gözden geçirin ve hizmet isteğine ekleyin](#step-6-current-partner-reviews-form-and-attaches-it-to-the-service-request)        |         |
|7     |         |         |[Eski iş ortağını hesaptan kaldır](#step-7-new-partner-removes-old-partner-from-account)         |
|8     |         |         |[Eski erişim izinlerini kaldır](#step-8-new-partner-removes-outdated-access-permissions)         |

### <a name="steps-for-transferring-a-customer-subscription-to-a-new-azure-service-provider"></a>Bir müşteri aboneliğini yeni bir Azure hizmet sağlayıcısına aktarma adımları

#### <a name="step-1-customer-contacts-current-partner-in-writing"></a>1. Adım: müşteri, yazma sırasında geçerli iş ortağıyla iletişim kurar

Müşteri, abonelik aktarma isteğinde hem Microsoft 'un hem de geçerli CSP Iş ortağının yazma sırasında (yani, hiçbir şekilde değil) bilgilendirerek aktarım sürecini başlatır.

#### <a name="step-2-current-provider-creates-azure-support-ticket-to-request-a-transfer"></a>2. Adım: geçerli sağlayıcı bir aktarım istemek için Azure destek bileti oluşturuyor

Geçerli iş ortağı bir abonelik aktarımı istemek için bir Azure destek bileti oluşturur.

> [!NOTE]
> Bu, aktarım sürecini başlatan destek bileti oluşturmak için geçerli ortağın sorumluluğudur. Microsoft, müşteri veya yeni iş ortağı adına müdahale etmez.

**Aktarım isteğinde bulunan bir destek bileti oluşturmak için:**

1. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin, listeden müşteriyi seçin ve ardından **hizmet yönetimi**' ni seçin.
1. **Destek biletleri** bölümünde, **yeni bilet** ' ı seçin ve ardından **Microsoft Azure.**
1. [Azure Portal](https://portal.azure.com/) **Yeni destek isteği**' ni seçin.
1. destek isteğinin 1. adımında, sorun türü olarak **abonelik yönetimi** ' ni seçin, aktarılmasını istediğiniz abonelik kimliğini belirtin ve destek planı olarak **Bulut Çözümü Sağlayıcısı** seçin.
1. 2. adımda, **C-en az etkisi** ' nı seçin ve sorun türü olarak **diğer genel sorular** ' ı seçin.

#### <a name="step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer"></a>3. Adım: geçerli iş ortağı aktarım formunu tamamlar ve müşteriye gönderir

geçerli iş ortağı [Bulut Çözümü Sağlayıcısı form değişikliğini](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)indirir ve tamamlar, bu dosyayı imzalar ve ardından müşteriye gönderir.

#### <a name="step-4-current-partner-completes-current-partner-fills-in-the-change-of-cloud-solution-provider-form"></a>4. adım: geçerli iş ortağı, geçerli iş ortağını tamamlar Bulut Çözümü Sağlayıcısı değişiklik biçiminde doldurur

geçerli iş ortağı [Bulut Çözümü Sağlayıcısı formu değişikliğini](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)tamamlar, imzalar ve müşteriye gönderir.

*Bulut Çözümü Sağlayıcısı form değişikliğini* gerçekleştirmek için gereken bilgiler arasında:

- **Geçerli ortağın iletişim bilgileri ve MICROSOFT kimliği** (Iş Ortağı Merkezi menüsünde, **Hesap ayarları > kuruluş profili**) seçilerek bulunabilir.
- **Müşterinin MICROSOFT kimliği** (Iş Ortağı Merkezi menüsünde **müşteriler** ' i seçerek ve ardından Microsoft kimliklerini açığa çıkarmak için müşterinin listesini genişleterek bulabilirsiniz).
- Transfer edilecek **ABONELIK kimliği** (Iş Ortağı Merkezi menüsünde **müşteriler** ' i seçerek ve ardından müşterinin listesini genişleterek, **abonelikleri görüntüle**' yi seçerek ve ardından abonelik kimliğini açığa çıkarmak için seçili aboneliği genişleterek bulunabilir.

#### <a name="step-5-the-customer-and-new-partner-review--return-the-form"></a>5. Adım: müşteri ve yeni iş ortağı incelemesi & formu döndürür

Birlikte çalışarak, müşteri ve yeni iş ortağı:

1. Formu gözden geçirin, yeni iş ortağı hakkındaki bilgileri girin ve imzalayın.
1. Yeni müşterinin bir sözleşme anlaşması olduğunu onaylayın.
1. Formu geçerli ortağa geri gönderin.

#### <a name="step-6-current-partner-reviews-form-and-attaches-it-to-the-service-request"></a>6. Adım: geçerli iş ortağı İncelemeleri formu ve hizmet isteğine iliştirir

Geçerli iş ortağı formu aldığında şunları yapın:

- Formun hem iş ortağı yöneticileri için iletişim bilgilerini içerdiğinden emin olun. (Microsoft Desteği aktarımı doğrulamak için her iki yönetici ile de iletişim kurar.)
- bunların üç imzaya sahip olduğunu doğrulayın ve ardından tamamlanmış formu mevcut hizmet isteğine eklemek için **dosya Upload** seçeneğini kullanın. (Microsoft Destek Mühendisi, giriş ve tamamlamayı doğrulamak için sekiz iş saati içinde bu kişilerle iletişim kurar.)

#### <a name="step-7-new-partner-removes-old-partner-from-account"></a>7. Adım: yeni iş ortağı eski iş ortağını hesaptan kaldırır

Yeni iş ortağı, eski iş ortağını hesaptan kaldırmak için PowerShell 'deki Azure abonelik ayarlarını güncelleştirir.

> [!NOTE]
> İlk PowerShell cmdlet 'i, müşterinin **MICROSOFT kimliği** olarak Iş Ortağı Merkezi 'Nde görüntülenen **Kiracı kimliğini** gerektirir. Aşağıdaki yordam, cmdlet 'inde kullanılmak üzere müşterinin Microsoft KIMLIĞINI (kiracı KIMLIĞI) bulmayı açıklamaktadır.

***Bağlan-azaccount* PowerShell cmdlet 'inde kullanılmak üzere müşterinin Microsoft kimliğini (kiracı kimliği) bulmak için**:

1. Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.
1. Menüden **müşteriler** ' i seçin.
1. Görüntülenen listede müşteriyi bulun.
1. Müşterinin listesini genişletmek için aşağı oku seçin. Müşterinin *etki alanı adı* ve MÜŞTERININ **Microsoft kimliği** hakkındaki bilgileri görürsünüz.
1. Bu yordamı izleyen PowerShell cmdlet 'inde 16 basamaklı **MICROSOFT kimliğini** kullanın.

İlk PowerShell cmdlet 'i, yeni ortağı hesaba satıcı olarak ekler:

```powershell
Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
```

İkinci cmdlet, önceki CSP iş ortakları da dahil olmak üzere hesaptaki rolleri görüntüler:

```powershell
Get-AzRoleAssignment
```

#### <a name="step-8-new-partner-removes-outdated-access-permissions"></a>8. Adım: yeni iş ortağı eski erişim izinlerini kaldırır

   **Güncel olmayan erişim izinlerini kaldırmak için:**

   1. Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin.
   1. Müşteri listesinde müşteriyi bulun.
   1. Müşterinin şirket adına çift tıklayın. Müşteri **abonelikleri** sayfası görüntülenir.
   1. Müşteri ayrıntısı menüsünde **hizmet yönetimi**' ni seçin.
   1. **Microsoft Azure** altında **Microsoft Azure Yönetim Portalı**' yı seçin.

## <a name="transferring-a-previous-azure-offer-subscription-without-converting-it-to-the-azure-plan"></a>Önceki bir Azure teklifi aboneliğini Azure planına dönüştürmeden aktarma

Bu bölümde, yeni Azure planının nasıl tanıtılmakta olduğu kısaca açıklanmaktadır. Daha sonra, önceki Azure teklifinin bazı aboneliklerinin yeni Azure planına dönüştürülmeksizin başka bir CSP 'ye aktarılabileceği özel bir durum açıklanır.

> [!NOTE]
> Önceki Azure teklifi kapsamında satın alınan bir müşterinin Azure aboneliklerini yeni bir CSP 'ye aktarmak *ve Azure planına dönüştürmek* için (varsayılan eylem), bir [*Azure aboneliğini başka bir ortağa aktarma*](#transferring-azure-subscriptions-to-another-partner)hakkında daha fazla bilgi ve [*MÜŞTERININ Azure aboneliklerini farklı bir CSP 'ye aktarma (bir Azure planı altında)*](./transfer-azure-subscriptions-under-azure-plan.md)makalesini inceleyin.

### <a name="the-azure-plan-and-the-previous-azure-offer"></a>Azure planı ve önceki Azure teklifi

Microsoft, 2021 Temmuz sürümünde [Azure planı](./azure-plan-lp.md)olan yeni bir ticari deneyim sunmuştur. İş ortaklarının yeni özellikleri, önceki Azure teklifinden (MS-AZR-0145p) sunulan hizmetleri ve geçiş müşterilerine Azure planına ekleme süresi vermek için, önceki Azure teklifi sınırlı bir süre için kullanılabilir olmaya devam eder.

Önceki Azure teklifinden Azure planına geçiş üç aşamadan oluşur:

**1. aşama**: 2021 Temmuz 'da Azure planının kullanıma sunulmasından itibaren, tüm yenı Azure CSP program müşterileri Azure planına yerleştirildi. İş ortakları önceki Azure teklifini zaten satın almış olan müşterilerle Transact.

**2. aşama**: 1 Şubat 2022 ' de, teşvikleri ve iş ortağı kenar boşluğu fırsatı önceki Azure teklifinden kaldırılır.

**3. aşama**: henüz belirlenebileceği için, önceki Azure teklifi kullanımdan kaldırılacak ve yine de önceki Azure teklifinde bulunan müşteriler Azure planına geçirilecektir. (İş ortakları, tarihinden itibaren altı ay önce kullanımdan kaldırılacaktır.)

### <a name="transferring-subscriptions-without-conversion"></a>Abonelikler dönüştürme olmadan aktarılıyor

Bu bölümde, *Azure planına dönüştürmeden* önceki Azure teklifi kapsamında satın alınan bir aboneliğin yenı bir CSP sağlayıcısına aktarılmasında özel durum açıklanır.

Bir müşterinin önceki Azure teklifine yönelik aboneliği, önceki bölümde yer alarak [Azure aboneliklerini başka bir iş ortağına aktaran](#transferring-azure-subscriptions-to-another-partner)Azure planına dönüştürme olmadan yenı bir CSP ortağına aktarılabilir.

- Önceki Azure teklifi hala kullanılabilir.
- Hem geçerli ortağın hem de yeni ortağın, önceki Azure teklifine yönelik aboneliği olan bir müşterisi vardır.

Yalnızca geçerli ortağın önceki Azure teklifine abone olan bir müşterisi varsa, geçerli iş ortağı geçiş aracını kullanarak, aynı anda yeni Azure planına dönüştürülürken müşterinin aboneliğini yeni iş ortağına taşıyabilir.

> [!NOTE]
> Yalnızca Microsoft ile doğrudan faturalandırma ilişkisine sahip iş ortakları Geçiş aracına erişebilir. Dolaylı satıcıların geçiş aracını kullanması için dolaylı sağlayıcılarıyla çalışması gerekir.

## <a name="next-steps"></a>Sonraki adımlar

- [Azure aboneliklerini aktarma](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)
- [Azure aboneliklerini Azure planına aktarma](transfer-azure-subscriptions-under-azure-plan.md)
- [CSP abonelik aktarma formunu](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC) indirin
- [Çoklu iş ortağı desteği](multipartner.md) hakkında bilgi edinin
- [Çoklu kanallı destek](multichannel.md) hakkında bilgi edinin