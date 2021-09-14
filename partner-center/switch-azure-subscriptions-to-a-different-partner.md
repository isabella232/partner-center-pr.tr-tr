---
title: Azure aboneliğini başka bir iş ortağına aktarma
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Müşterinin Azure abonelikleriyle Bulut Çözümü Sağlayıcısı program iş ortağını değiştirme hakkında bilgi edinin.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 07/21/2021
ms.openlocfilehash: 28e90ec4a699e2d8830f3695a30151e6b00e8cd1
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126249045"
---
# <a name="transfer-a-customers-azure-subscriptions-to-a-different-partner-without-converting-them-to-an-azure-plan"></a>Müşterinin Azure aboneliklerini Bir Azure planına dönüştürmeden farklı bir iş ortağına aktarma

**Için geçerlidir:** İş Ortağı Merkezi | İş Ortağı Merkezi için Microsoft Cloud for US Government

**Uygun roller:** Genel yönetici

Bu makalede, bir müşterinin bir Azure aboneliğini geçerli aboneliğinden (CSP) Bulut Çözümü Sağlayıcısı CSP'ye nasıl aktar olduğu açıklanmıştır.

İlk bölüm olan [Azure](#transferring-azure-subscriptions-to-another-partner)aboneliğini başka bir iş ortağına aktarma bölümünde, bir müşterinin Microsoft Azure aboneliğini bir Bulut Çözümü Sağlayıcısı (CSP) diğerine nasıl aktarabilirsiniz?

Bir sonraki bölüm olan Azure teklifi aboneliğini Azure planına dönüştürmeden aktarma bölümünde, yeni [Azure](#transferring-a-previous-azure-offer-subscription-without-converting-it-to-the-azure-plan)planının nasıl tanıtıldıkları kısaca açıklandı. Ardından, önceki Azure teklifine bazı aboneliklerin yeni Azure planına dönüştürülmeden başka bir CSP'ye aktarılamayacak şekilde özel bir durumu açıklar.

Müşteri aboneliğini yeni bir Azure hizmet sağlayıcısına aktarırken müşterinin, geçerli hizmet sağlayıcısının ve yeni bir hizmet [sağlayıcısının tüm sorumlulukları vardır.](#responsibilities-when-transferring-a-customer-subscription-to-a-new-azure-service-provider) Bir müşterinin geçişin sorunsuz bir şekilde devam etmek için geçerli iş ortağıyla yakın bir çalışma planlaması gerekir.

 Azure abonelerine CSP iş ortaklarının aboneliklerini aktarmalarına yardımcı olmak için üst düzey bilgiler, Aboneler ile CSP'ler arasında Azure aboneliklerini aktarma [sayfasında bulunabilir.](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)

Müşterilerin Azure aboneliklerini bir iş ortağından diğerine nasıl değiştir olduklarına ilişkin ek bilgiler müşterinin Azure aboneliklerini farklı bir [CSP'ye aktarma (Azure planı kapsamında)](/partner-center/transfer-azure-subscriptions-under-azure-plan) içinde bulunabilir

## <a name="prerequisites"></a>Önkoşullar

- CsP İş Ortağının, abonelik aktarılamadan önce müşteriyle kurumsal bayi ilişkisi olması gerekir.  Daha fazla bilgi için, [bkz. How to request a reseller relationship from a customer in İş Ortağı Merkezi](/partner-center/request-a-relationship-with-a-customer).
- Bir iş ortağının aboneliği aktarması için doğrudan sağlayıcı veya dolaylı sağlayıcı olması gerekir.
- Aşağıdaki tekliflerle ilişkili abonelikler aktaramaz: Azure planı, Office 365, Enterprise Mobility Suite ve Microsoft Dynamics CRM.
- Bir müşterinin aboneliği aktarması için iş ortağıyla aynı ülkede olması gerekir.
- Microsoft Cloud for US Government veya Microsoft Bulut Almanya'da faaliyet gösteren iş ortaklarının müşterinin hizmetini veya aboneliğini yönetmek için izin talep etmeleri gerekir. Daha fazla bilgi için [bkz. Müşterinin hizmetini veya aboneliğini yönetme izinlerini alma.](/partner-center/customers-revoke-admin-privileges)

## <a name="transferring-azure-subscriptions-to-another-partner"></a>Azure aboneliklerini başka bir iş ortağına aktarma

Bir Azure aboneliğini bir CSP iş ortağından diğerine aktarmak, müşterinin, geçerli iş ortağının ve yeni iş ortağının çeşitli aşamalarda eylemlerini gerektiren çok adımlı bir işlemdir. Aşağıdaki tablo, kimin ne zaman ne zaman ne yaptığını netleştirmeye yardımcı olmak için sıralı diyagram olarak tasarlanmıştır.

### <a name="responsibilities-when-transferring-a-customer-subscription-to-a-new-azure-service-provider"></a>Müşteri aboneliğini yeni bir Azure hizmet sağlayıcısına aktarırken sorumluluklar

|Adım  |Müşteri  |Geçerli iş ortağı  |Yeni iş ortağı  |
|---------|---------|---------|---------|
|1     |[Müşteri Microsoft'a ve mevcut iş ortağına yazılı olarak bilgi iletir](#step-1-customer-contacts-current-partner-in-writing)         |         |         |
|2     |         |[Aktarım isteği için destek bileti oluşturma](#step-2-current-provider-creates-azure-support-ticket-to-request-a-transfer)        |         |
|3     |         |[Tamamlanan aktarım formunu müşteriye gönderme](#step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer)|         |
|4     |         |[Form değişikliğini Bulut Çözümü Sağlayıcısı değiştirme](#step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer)       |         |
|5     |[İade formunu gözden geçirme, &, imzalama](#step-5-the-customer-and-new-partner-review--return-the-form)       |         |[İade formunu gözden geçirme, &, imzalama](#step-5-the-customer-and-new-partner-review--return-the-form)         |
|6     |         |[Gözden geçirme formu ve hizmet isteğine ekleme](#step-6-current-partner-reviews-form-and-attaches-it-to-the-service-request)        |         |
|7     |         |         |[Eski iş ortağını hesaptan kaldırma](#step-7-new-partner-removes-old-partner-from-account)         |
|8     |         |         |[Eski erişim izinlerini kaldırma](#step-8-new-partner-removes-outdated-access-permissions)         |

### <a name="steps-for-transferring-a-customer-subscription-to-a-new-azure-service-provider"></a>Müşteri aboneliğini yeni bir Azure hizmet sağlayıcısına aktarma adımları

#### <a name="step-1-customer-contacts-current-partner-in-writing"></a>1. Adım: Müşteri, geçerli iş ortağıyla yazılı olarak iletişime geçin

Müşteri, hem Microsoft'a hem de mevcut CSP İş Ortağına aboneliği aktarma isteğini yazılı olarak bildirerek (sözel olarak değil) aktarım işlemini başlatır.

#### <a name="step-2-current-provider-creates-azure-support-ticket-to-request-a-transfer"></a>2. Adım: Geçerli sağlayıcı Azure desteği isteği için bir bilet oluşturur

Geçerli iş ortağı, abonelik Azure desteği için bir bilet oluşturur.

> [!NOTE]
> Aktarım işlemini başlatan destek biletini oluşturmak geçerli iş ortağının sorumluluğundadır. Microsoft, müşteri veya yeni iş ortağı adına müdahale etmez.

**Aktarım isteği için bir destek bileti oluşturmak için:**

1. Hizmet İş Ortağı Merkezi Müşteriler'i **seçin,** listeden müşteriyi seçin ve ardından Hizmet **yönetimi'ne tıklayın.**
1. Destek **biletleri bölümünde Yeni** bilet'i **seçin ve** **Microsoft Azure.**
1. yeni [Azure portal](https://portal.azure.com/)Yeni destek **isteği'ne seçin.**
1. Destek isteğinin 1. Adım'sinde, sorun türü olarak Abonelik yönetimi'ne tıklayın, aktarılan abonelik kimliğini belirtin ve destek **planı olarak** Bulut Çözümü Sağlayıcısı'yi seçin. 
1. 2. Adımda **C-Minimum etki'yi seçin ve** sorun **türü olarak Diğer Genel** Sorular'ı seçin.

#### <a name="step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer"></a>3. Adım: Geçerli iş ortağı aktarım formunu tamamlar ve müşteriye gönderir

Geçerli iş ortağı Form [Değişikliği'Bulut Çözümü Sağlayıcısı indirir](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)ve tamamlar, imzalar ve müşteriye gönderir.

#### <a name="step-4-current-partner-completes-current-partner-fills-in-the-change-of-cloud-solution-provider-form"></a>4. Adım: Geçerli iş ortağı, geçerli iş ortağını tamamlar ve Bulut Çözümü Sağlayıcısı doldurur

Geçerli iş ortağı, [Bulut Çözümü Sağlayıcısı formunu tamamlar,](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)imzalar ve müşteriye gönderir.

Form değişikliği formunu tamamlamak için *gereken Bulut Çözümü Sağlayıcısı* arasında:

- **Geçerli iş ortağının iletişim bilgileri ve Microsoft kimliği** (Hesap ayarları'İş Ortağı Merkezi profili) seçerek > **kimliği.**
- **Müşterinin Microsoft Kimliği** (Müşteriler'i seçerek İş Ortağı Merkezi ve ardından  müşterinin listesini genişleterek Microsoft kimliğini ortaya çıkararak bu kimliği bulabilirsiniz).
- **Aktarilecek** Abonelik Kimliği (Müşteriler'i seçerek İş Ortağı Merkezi menüsünde bulunabilir ve  ardından müşterinin listesini genişleterek, Abonelikleri Görüntüle'yi seçerek ve ardından abonelik kimliğini ortaya çıkarmak için seçilen aboneliği genişleterek bulunabilir).

#### <a name="step-5-the-customer-and-new-partner-review--return-the-form"></a>5. Adım: Müşteri ve yeni iş & gözden geçirme formu

Müşteri ve yeni iş ortağı birlikte çalışma:

1. Formu gözden geçirme, yeni iş ortağıyla ilgili bilgileri doldurma ve imzalama.
1. Yeni müşterinin sözleşme anlaşması olduğunu onaylayın.
1. Formu geçerli iş ortağına geri gönderin.

#### <a name="step-6-current-partner-reviews-form-and-attaches-it-to-the-service-request"></a>6. Adım: Geçerli iş ortağı incelemeleri formu ve bunu hizmet isteğine ekleme

Geçerli iş ortağı formu aldığında:

- Formda her iki iş ortağı yöneticisi için de iletişim bilgileri olduğundan emin olun. (Microsoft Desteği doğrulamak için her iki yöneticiyle de iletişim sağlar.)
- Üç imzanın da olduğunu doğrulayın, ardından tamamlanan **formu mevcut hizmet isteğine Upload** dosya dosyası seçeneğini kullanın. (Microsoft destek mühendisi, makbuzu ve tamamlanmasını doğrulamak için sekiz iş saati içinde bu mühendisle iletişime devam ediyor.)

#### <a name="step-7-new-partner-removes-old-partner-from-account"></a>7. Adım: Yeni iş ortağı eski iş ortağını hesaptan kaldırır

Yeni iş ortağı, eski iş ortağını hesaptan kaldırmak için PowerShell'de Azure abonelik ayarlarını günceller.

> [!NOTE]
> İlk PowerShell cmdlet'i, müşterinin Kiracı Kimliğini gerektirir. Bu kimlik, İş Ortağı Merkezi microsoft kimliği **olarak görünür.** Aşağıdaki yordam, müşterinin microsoft kimliğinin (Kiracı Kimliği) cmdlet'inde nasıl kullanılabını açıklar.

**bir müşterinin Microsoft Kimliğini (Kiracı Kimliği) *Bağlan-AzAccount* PowerShell cmdlet'inde kullanmak üzere bulmak için:**

1. İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard)
1. Menüden **Müşteriler'i** seçin.
1. Görüntülenen listede müşteriyi bulun.
1. Müşterinin listesini genişletmek için aşağı oku seçin. Müşterinin Etki alanı adı ve müşterinin Microsoft *kimliği* hakkında bilgi **edinebilirsiniz.**
1. Bu yordamı izleyen PowerShell cmdlet'inde 16 basamaklı **Microsoft** Kimliğini kullanın.

İlk PowerShell cmdlet'i yeni iş ortağını hesaba kurumsal bayi olarak ekler:

```powershell
Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
```

İkinci cmdlet, önceki CSP iş ortakları da dahil olmak üzere hesapta rolleri görüntüler:

```powershell
Get-AzRoleAssignment
```

#### <a name="step-8-new-partner-removes-outdated-access-permissions"></a>8. Adım: Yeni iş ortağı, tarihin dışında erişim izinlerini kaldırır

   **Eski erişim izinlerini kaldırmak için:**

   1. Yeni İş Ortağı Merkezi Müşteriler'i **seçin.**
   1. Müşteri listesinde müşteriyi bulun.
   1. Müşterinin şirket adına çift tıklayın. Müşteri **Abonelikleri** sayfası görüntülenir.
   1. Müşteri ayrıntıları menüsünde Hizmet **yönetimi'ne tıklayın.**
   1. öğesinin **Microsoft Azure** öğesini seçin ve **Microsoft Azure Yönetim Portalı.**

## <a name="transferring-a-previous-azure-offer-subscription-without-converting-it-to-the-azure-plan"></a>Önceki bir Azure teklifi aboneliğini Azure planına dönüştürmeden aktarma

Bu bölümde yeni Azure planının nasıl tanıtıldıkları kısaca açıklandı. Ardından, önceki Azure teklifine bazı aboneliklerin yeni Azure planına dönüştürülmeden başka bir CSP'ye aktarılamayacak şekilde özel bir durumu açıklar.

> [!NOTE]
> Bir müşterinin önceki Azure teklifi kapsamında satın alınan Azure aboneliklerini yeni bir CSP'ye aktarmak ve azure planına dönüştürmek için (varsayılan eylemdir) önceki bölüme bakın Azure aboneliğini başka bir iş ortağına aktarma ve Müşterinin [*Azure*](#transferring-azure-subscriptions-to-another-partner)aboneliklerini farklı bir [*CSP'ye aktarma (Bir Azure*](/partner-center/transfer-azure-subscriptions-under-azure-plan)planı altında) makalesine bakın.

### <a name="the-azure-plan-and-the-previous-azure-offer"></a>Azure planı ve önceki Azure teklifi

Microsoft, Temmuz 2021'de yeni bir ticari deneyim olan [Azure](/partner-center/azure-plan-lp)planını tanıttı. İş ortaklarına hizmetleriyle yeni özellikleri dahil etmek ve müşterilerini önceki Azure teklifinden (MS-AZR-0145p) Azure planına geçiş yapmak için zaman vermek için önceki Azure teklifi sınırlı bir süre boyunca kullanılabilir olacak.

Önceki Azure teklifinden Azure planına geçiş üç aşamadadır:

**1.** Aşama: Azure planının Temmuz 2021'de tanıtılandan bu yana tüm yeni Azure CSP programı müşterileri Azure planına yerleştirilmiştir. İş ortakları, daha önce satın alan müşterilerle önceki Azure teklifini işlem yapmaya devam eder.

**2.** Aşama: Teşvikler ve iş ortağı marjı fırsatı 1 Şubat 2022'de önceki Azure teklifinden kaldırılacaktır.

**3.** Aşama: Henüz belirlenemeyen bir zamanda, önceki Azure teklifi kullanımdan kaldırılır ve önceki Azure teklifinin müşterileri Azure planına geçirilir. (İş ortaklarına, altı ay önce emeklilik tarihi bildirilecek.)

### <a name="transferring-subscriptions-without-conversion"></a>Abonelikleri dönüştürme olmadan aktarma

Bu bölümde, önceki Azure teklifi kapsamında satın alınan bir aboneliği Azure planına dönüştürmeden yeni bir CSP sağlayıcısına aktarma özel *durumu açıklandı.*

Bir müşterinin önceki Azure teklifine aboneliği, önceki bölümde yer alan Azure aboneliklerini başka bir iş ortağına aktarma bölümünde yer alan adımları kullanarak [Azure](#transferring-azure-subscriptions-to-another-partner)planına dönüştürme yapmadan yeni bir CSP iş ortağına aktarabilirsiniz. Aşağıdakiler:

- Önceki Azure teklifi hala kullanılabilir.
- Hem geçerli iş ortağının hem de yeni iş ortağının, önceki Azure teklifine aboneliği olan bir müşterisi var.

Yalnızca geçerli iş ortağının önceki Azure teklifine aboneliği olan bir müşterisi varsa, geçerli iş ortağı müşterinin aboneliğini yeni iş ortağına taşımak ve aynı zamanda bunu yeni Azure planına dönüştürmek için geçiş aracını kullanabilir.

> [!NOTE]
> Geçiş aracına yalnızca Microsoft ile doğrudan faturalama ilişkisi olan iş ortakları erişebilirsiniz. Dolaylı kurumsal bayilerin geçiş aracını kullanmak için dolaylı sağlayıcılarıyla birlikte çalışması gerekir.

## <a name="next-steps"></a>Sonraki adımlar

- [Azure aboneliklerini aktarma](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)
- [Azure planı kapsamındaki Azure aboneliklerini aktarma](transfer-azure-subscriptions-under-azure-plan.md)
- [CSP Abonelik Aktarımı formunu indirin](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)
- Çok iş [ortağı desteği hakkında bilgi](multipartner.md)
- Çok [kanallı destek hakkında bilgi](multichannel.md)
