---
title: Müşterinin yönetici ayrıcalıklarını alma
ms.topic: how-to
ms.date: 12/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bir müşterinin hizmetini veya aboneliğini kendi adına yönetmek için ihtiyacınız olan izinleri alın. İzinlerin nasıl verilmiş, iptal edilmiş ve yönetiliyor olduğunu öğrenin.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: 779e76d6bb3e8df679a5ca6fa8ce441e42529161
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147301"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Müşterinin hizmetini veya aboneliğini yönetmek için izinler alma

**Uygun roller:** Yönetici aracısı | Satış aracısı

Müşterinin hizmetini veya aboneliğini kendi adına yönetmek için, müşterinin size bu hizmet için yönetici izinleri ataması gerekir. Müşteriden yönetici izinleri almak için bir kurumsal bayi ilişkisi isteği e-postası gönderin. Müşteri isteğinizi onay verdikten sonra hizmetin yönetim portalında oturum açma ve hizmeti müşteri adına yönetme yetkisine sahip olur. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Müşteriyi, kurumsal bayi ilişkisi kurması için davet etme

1.  **Müşteriler'i** ve ardından Kurumsal **bayi ilişkisi isteğide bulun'ı seçin.**

2.  Sonraki sayfada taslak e-posta iletisini gözden geçirin. Taslak iletiyi varsayılan e-posta uygulamanızda açabilir veya iletiyi panonuza kopyalayıp bir e-postaya yapıştırabilirsiniz. 

    >[!IMPORTANT]
    >E-postanın metnini düzenleyebilirsiniz ama bağlantıyı eklemeyi unutmayın çünkü bu müşteriyi doğrudan hesabınıza bağlayacak kişiselleştirilmiş bir bağlantıdır. 
    
3.  Bu **adımı** tamamlandıktan sonra Bitti'yi seçin.

4.  E-postayı müşterinize gönderin.

5.  Müşteri daveti kabul ettikten sonra Müşteriler  sayfanıza görünür ve siz de müşteri için hizmeti orada s sağlama ve yönetmeye devam edebilirsiniz.

6.  Müşterinin hesabını, hizmetlerini, kullanıcılarını ve lisanslarını yönetmek için, adının yanındaki aşağı oku seçerek müşterinin kaydını genişletin ve ardından yönetmek istediğiniz hizmetin yönetici portalını seçin.

>[!IMPORTANT]  
>Müşteriler, bir hizmetin yönetim portalında yönetici izinlerini yeniden ayalar veya kaldırabilir. Bununla birlikte, yönetici izinlerinizi kaldırmanın, artık Microsoft'a kendi adına bir hizmet isteği açamazsınız anlamına geldiğini müşteriye bildirmeniz gerekir. Müşteriyle sözleşmenizi yeniden anlaşmadan müşterinin adına bu tür hizmet isteklerini açamazsiniz.

Müşterileriniz, Office 365 yönetici portalında kiracılarında hangi iş ortaklarının yönetici ayrıcalıklarına sahip olduğunu bulabilir. Bunu yapmak için:

1. Müşterinin Office 365 yönetim portalında Genel yönetici olarak oturum açması gerekir.

2. Ayarlar **İş Ortağı**  >  **ilişkileri'ne tıklayın.**

3. **Ortak ilişkiler** sayfasında, müşteri, çalıştıkları iş ortaklarının bir listesini ve kiracının kendilerine atanmış yönetim ayrıcalıkları verildiğini görür.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Müşteriler, iş ortağının yönetici ayrıcalıklarını yönetebilir 

Müşteriniz, kiracının Temsilcili yönetici ayrıcalıklarınızı kaldırmaya karar verebilir, ancak abonelik ve lisans yenileme amaçları için sizinle ilişkiyi koruyabilir. Müşteriler, Office 365 Yönetim Merkezi 'ndeki **Iş ortağı ilişkileri** sayfasında Office 365 hesaplarıyla ilgili hakları ve izinleri yönetir. Bu sayfada, müşteriler şunları yapabilir:

- Hangi iş ortaklarının bir ilişkisi olduğunu ve hangi iş ortaklarının yönetici ayrıcalıklarına sahip olduğunu görün

- Bir ortağın Temsilcili yönetim ayrıcalıklarını kiracıya kaldırma

Temsilcili yönetim ayrıcalıklarını bir iş ortağından kaldırmak için:

1. **Iş ortağı ilişkileri** sayfasında, ilgilendiğiniz iş ortağını seçin.
2. Ayrıntılar bölmesinde, **yönetici temsilcisi kaldır**' ı seçin.
3. Onay bölmesinde **Kaldır**' ı seçin.

>[!IMPORTANT]  
>İş ortağına yönelik Azure AD rol atamaları örtük olarak bulunur. Azure AD Portal/PowerShell/Graph kullanarak Azure AD rollerinin üyelerini listedenemeye çalışırsanız, iş ortağı döndürülmez. İş ortaklarının Azure AD rollerine atanıp atanmadığını öğrenmek için, iş ortağının Temsilcili yönetim ayrıcalığının verildiğini öğrenmek üzere Office 365 yönetim portalındaki Iş ortağı ilişkiler sayfasına başvurmanız gerekir.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Azure AD 'de yönetici ayrıcalıkları temsilcisi 

İş ortağının Azure AD kiracısında, temsilcili yönetim için kullanılan iki güvenlik grubu, Yönetim Aracısı ve Yardım Masası Aracısı vardır. Bir müşteri, bir iş ortağı için Temsilcili yönetim ayrıcalığı verdiğinde:

- Yönetici Aracısı grubu, müşterinin Azure AD kiracısında genel yönetici rolüne atanır.

- Yardım Masası aracı grubu, müşterinin Azure AD kiracısındaki yardım masası yönetici rolüne atanır.

Atanan dizin rollerine bağlı olarak, her iki grubun üyeleri de müşteri adına iş ortağı kimlik bilgilerini ve yöneticiyi kullanarak müşterinin Azure AD kiracısı ve O365 hizmetlerinde oturum açın.

Müşteriniz yönetici temsilcisi ayrıcalıklarını kaldırırsa Azure AD rol atamaları kaldırılır ve artık müşterinin Azure AD kiracısını yönetemeyeceksiniz.

### <a name="azure-subscriptions-and-resource-management"></a>Azure abonelikleri ve kaynak yönetimi

Her Azure aboneliğinin kendi kaynak yönetimi rolleri kümesi vardır. CSP iş ortağının müşterinin Azure aboneliğini yönetemeden önce iş ortağının Azure aboneliği altındaki bir veya daha fazla role atanmaları gerekir. Özellikle:

- Müşteri bir kurumsal bayi davetini kabul edin ve bir iş ortağına temsilcili yönetim ayrıcalığı verdi mi, iş ortağı müşteri kiracısı altındaki mevcut Azure aboneliklerine otomatik olarak erişim elde etmez.

- CSP iş ortağı müşteri için yeni bir Azure aboneliği sağlarken, CSP iş ortağı kiracısı altındaki Yönetici Aracıları grubuna abonelik altında otomatik olarak Sahip rolü atanır. Bu rol ataması temel alınarak, grubun üyeleri abonelik altındaki kaynaklara erişebilirsiniz ve kaynakları yönetebilir.

- Müşteri Office 365 Portal'ı kullanarak bir iş ortağından temsilcili yönetim ayrıcalıklarını kaldırdığı zaman, iş ortağı abonelik altındaki bir veya daha fazla role atandığı sürece müşterinin Azure aboneliğini yönetmeye devam eder. İş ortağının Azure aboneliğini yönetmesi için müşterinin rol atamayı kaldırması gerekir.

## <a name="windows-autopilot"></a>Windows Autopilot

CSP İş Ortağı Merkezi, şu koşullarda yönetici ayrıcalıkları temsilcisi olmadan müşterileri için Autopilot profillerini yönetebilir: 

- Müşteri temsilcili yönetim ayrıcalıklarını kaldırırsa ancak kurumsal bayi ilişkisini korursa, bu müşteriler için Autopilot profillerini yönetmeye devam edersiniz.

- Sizin veya başka bir iş ortağının ekleymüş olduğu müşteri cihazlarını yönetebilirsiniz. 

- Müşterinizin Iş Microsoft Store, eğitim için Microsoft Store veya Microsoft Intune Portal aracılığıyla eklediği cihazları yönetemezsiniz.

Autopilot hakkında daha fazla bilgi için bkz. [Windows Autopilot ile cihaz kurulumunu basitleştirme](autopilot.md).

>[!IMPORTANT]  
>Iş Ortağı Merkezi 'nde geçerli Autopilot yönetim deneyimi değişmeye devam edebilir. Bu makalenin yayımlandığı sırada aşağıdaki değişiklikler göz önünde bulundurulmaktadır:

- Ortak, iş ortağının profilleri eklemesini/kaldırmasını/kaldırabilmesi ve profili müşteri kiracısındaki herhangi bir cihazdan uygulama/kaldırma işleminden önce müşteri tarafından atanan yönetim ayrıcalığı verilmelidir.

- Ortak, iş ortağının diğer iş ortakları tarafından eklenen cihazları veya müşteri kiracısındaki müşteriyi kaldırabilmesi için müşterinin Temsilcili Yönetim ayrıcalığına sahip olması gerekir. Aksi takdirde, iş ortağı yalnızca daha önce aynı iş ortağı tarafından eklenen cihazları kaldırabilir.
