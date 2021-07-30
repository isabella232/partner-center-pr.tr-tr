---
title: Müşterinin yönetici ayrıcalıklarını alma
ms.topic: how-to
ms.date: 12/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Müşterinin hizmetini veya aboneliğini kendi adına yönetmek için ihtiyacınız olan izinleri alın. İzinlerin nasıl ver edildiğini, iptal edildiğini ve yönetil olduğunu öğrenin.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: fafd9e2c13abb1f4b9b12e5839662b27c4852452
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114842108"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Müşterinin hizmetini veya aboneliğini yönetmek için izinler alma

**Uygun roller:** Yönetici aracısı | Satış aracısı

Müşterinin hizmetini veya aboneliğini kendi adına yönetmek için, müşterinin size bu hizmet için yönetici izinleri ataması gerekir. Müşteriden yönetici izinleri almak için bir kurumsal bayi ilişkisi isteği e-postası gönderin. Müşteri isteğinizi onay verdikten sonra hizmetin yönetici portalında oturum açma ve hizmeti müşteri adına yönetme yetkisine sahip olur. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Bir müşteriyi, bir kurumsal bayi ilişkisi kurması için davet etme

1.  **Müşteriler'i** ve ardından Kurumsal **bayi ilişkisi isteğide bulun'ı seçin.**

2.  Sonraki sayfada taslak e-posta iletisini gözden geçirin. Taslak iletiyi varsayılan e-posta uygulamanızda açabilir veya iletiyi panonuza kopyalayıp bir e-postaya yapıştırabilirsiniz. 

    >[!IMPORTANT]
    >E-postanın metnini düzenleyebilirsiniz ama bağlantıyı eklemeyi unutmayın çünkü bu müşteriyi doğrudan hesabınıza bağlayacak kişiselleştirilmiş bir bağlantıdır. 
    
3.  Bu **adımı** tamamlandıktan sonra Bitti'yi seçin.

4.  E-postayı müşterinize gönderin.

5.  Müşteri daveti kabul ettikten sonra Müşteriler  sayfanıza görünür ve siz de müşteri için hizmeti orada s sağlama ve yönetmeye devam edebilirsiniz.

6.  Müşterinin hesabını, hizmetlerini, kullanıcılarını ve lisanslarını yönetmek için, adının yanındaki aşağı oku seçerek müşterinin kaydını genişletin ve ardından yönetmek istediğiniz hizmetin yönetici portalını seçin.

>[!IMPORTANT]  
>Müşteriler, bir hizmetin yönetim portalında yönetici izinlerini yeniden ayalar veya kaldırabilir. Bununla birlikte, yönetici izinlerinizi kaldırmanın, artık microsoft'a kendi adına bir hizmet isteği açamazsınız anlamına geldiğini müşteriye bildirmeniz gerekir. Müşteriyle sözleşmenizi yeniden anlaşmadan müşterinin adına bu tür hizmet isteklerini açamazsiniz.

Müşterileriniz, hangi iş ortaklarının kiracılarında yönetici ayrıcalıklarına sahip olduğunu yönetici portalının Office 365 bulabilir. Bunu yapmak için:

1. Müşterinin genel yönetici olarak Office 365 oturum açması gerekir.

2. İş   >  **Ayarlar'ı seçin.**

3. İş **ortağı ilişkileri** sayfasında müşteri, birlikte çalışmakta olduğu iş ortaklarının ve kiracısına yönetici ayrıcalıkları verilmiş olan iş ortaklarının listesini görebilir.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Müşteriler bir iş ortağının yönetici temsilcisi ayrıcalıklarını yönetebilir 

Müşteriniz, yönetici temsilcisi ayrıcalıklarınızı kiracılarından kaldırmaya karar verir ancak abonelik ve lisans yenileme amacıyla ilişkinizi korur. Müşteriler, iş ortağı Office 365 yönetim merkezinin **İş** ortağı ilişkileri sayfasında kendi hesaplarında Office 365 ve izinleri yönetir. Bu sayfada müşteriler şunları olabilir:

- Hangi iş ortaklarıyla bir ilişkisi olduğunu ve hangi iş ortaklarının yönetici ayrıcalıklarına sahip olduğunu görme

- Bir iş ortağının temsilci ile yönetim ayrıcalıklarını kiracıdan kaldırma

Bir iş ortağından temsilcili yönetim ayrıcalıklarını kaldırmak için:

1. İş **ortağı ilişkileri sayfasında,** ilgili iş ortağını seçin.
2. Ayrıntılar bölmesinde Yönetici temsilcisini **kaldır'ı seçin.**
3. Onay bölmesinde Kaldır'ı **seçin.**

>[!IMPORTANT]  
>İş ortağına Azure AD rol atamaları örtülü olarak gerçekleştirilen bir işlemdir. Azure AD Portal/PowerShell/Graph kullanarak Azure AD rollerinin üyelerini listeye eklemeye çalışsanız iş ortağı döndürülecek değildir. İş ortaklarının Azure AD rollerine atandığı hakkında bilgi için Office 365 Admin Portal'daki İş ortağı ilişkileri sayfasına bakarak iş ortağına temsilcili yönetim ayrıcalığı verilip verilmedi olduğunu bulmanız gerekir.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Azure AD'de yönetici ayrıcalıkları temsilcisi 

İş ortağının Azure AD kiracısı yönetim temsilcisi için kullanılan Yönetici Aracıları ve Yardım Masası Aracıları olmak için iki güvenlik grubu vardır. Müşteri bir iş ortağına temsilci ile yönetim ayrıcalığı izni verdi mi:

- Yönetici Aracısı grubu, müşterinin Azure AD kiracısında Genel Yönetici rolüne atanır.

- Yardım Masası Aracısı grubu, müşterinin Azure AD kiracısında Yardım Masası Yöneticisi rolüne atanır.

Atanan dizin rollerine bağlı olarak, her iki grubun üyeleri de müşteri adına iş ortağı kimlik bilgilerini ve yöneticiyi kullanarak müşterinin Azure AD kiracısı ve O365 hizmetlerinde oturum açın.

Müşteriniz yönetici temsilcisi ayrıcalıklarını kaldırırsa Azure AD rol atamaları kaldırılır ve artık müşterinin Azure AD kiracısını yönetemeyeceksiniz.

### <a name="azure-subscriptions-and-resource-management"></a>Azure abonelikleri ve kaynak yönetimi

Her Azure aboneliğinin kendi kaynak yönetimi rolleri kümesi vardır. CSP iş ortağının müşterinin Azure aboneliğini yönetemeden önce iş ortağının Azure aboneliği altında bir veya daha fazla role atanmaları gerekir. Özellikle:

- Müşteri bir kurumsal bayi davetini kabul edin ve bir iş ortağına temsilcili yönetim ayrıcalığı verdi mi, iş ortağı müşteri kiracısı altındaki mevcut Azure aboneliklerine otomatik olarak erişim elde etmez.

- CSP iş ortağı müşteri için yeni bir Azure aboneliği sağlarken, CSP iş ortağı kiracısı altındaki Yönetici Aracıları grubuna abonelik altında otomatik olarak Sahip rolü atanır. Bu rol ataması temel alınarak, grubun üyeleri abonelik altındaki kaynaklara erişebilirsiniz ve kaynakları yönetebilir.

- Müşteri Office 365 Portal'ı kullanarak bir iş ortağından temsilcili yönetim ayrıcalıklarını kaldırdığı zaman, iş ortağı abonelik altındaki bir veya daha fazla role atandığı sürece müşterinin Azure aboneliğini yönetmeye devam eder. İş ortağının Azure aboneliğini yönetmesi için müşterinin rol atamayı kaldırması gerekir.

## <a name="windows-autopilot"></a>Windows Autopilot

CSP İş Ortağı Merkezi, şu koşullarda yönetici ayrıcalıkları temsilcisi olmadan müşterileri için Autopilot profillerini yönetebilir: 

- Müşteri temsilcili yönetim ayrıcalıklarını kaldırırsa ancak kurumsal bayi ilişkisini korursa, bu müşteriler için Autopilot profillerini yönetmeye devam edersiniz.

- Sizin veya başka bir iş ortağının ekleymüş olduğu müşteri cihazlarını yönetebilirsiniz. 

- Müşterinizin İş İçin Microsoft Store, Eğitim İçin Microsoft Store veya Microsoft Intune Portal aracılığıyla ekley Microsoft Intune yönetesiniz.

Autopilot hakkında daha fazla bilgi için bkz. Windows [Autopilot ile cihaz kurulumunu basitleştirme.](autopilot.md)

>[!IMPORTANT]  
>İş Ortağı Merkezi autopilot yönetim deneyimi değişmeye devam ediyor olabilir. Bu makale yayımlanırken aşağıdaki değişiklikler dikkate alınmaktadır:

- İş ortağının, müşteri kiracısı içinde yer alan tüm cihazlardan profil ekleme/güncelleştirme/kaldırma ve profil uygulama/kaldırma işlemi öncesinde iş ortağına müşteri tarafından temsilci ile yönetim ayrıcalığı verilmesi gerekir.

- İş ortağının diğer iş ortakları veya müşteri kiracısı tarafından eklenen cihazları kaldıramadan önce iş ortağına müşteri tarafından temsilci ile yönetim ayrıcalığı verilmesi gerekir. Aksi takdirde, iş ortağı yalnızca aynı iş ortağı tarafından daha önce eklenen cihazları kaldırabilir.
