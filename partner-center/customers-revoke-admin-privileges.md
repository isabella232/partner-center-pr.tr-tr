---
title: Müşterinin yönetici ayrıcalıklarını edinin
ms.topic: how-to
ms.date: 12/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Müşterinin hizmetini veya aboneliğini kendi adınıza yönetmek için ihtiyacınız olan izinleri alın. İzinlerin nasıl verildiğini, iptal edildiğini ve yönetildiğini öğrenin.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: 6f99c9ed9fb43136bccf0d3024377ba2208ed1a1
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534888"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Müşterinin hizmetini veya aboneliğini yönetme izinleri alma

**Şunlara uygulanır**

- İş Ortağı Merkezi

**Uygun roller**

- Yönetim Aracısı
- Satış Aracısı

Müşterinin hizmet veya aboneliğini kendi adına yönetmek için müşterinin size bu hizmet için yönetici izinleri vermesi gerekir. Bir müşteriden yönetici izinleri almak için, satıcıya bir satıcı ilişki isteği gönderin. Müşteri isteğinizi onayladıktan sonra hizmetin yönetim portalında oturum açabilir ve müşterinin adına hizmeti yönetebilirsiniz. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Bir müşteriyi sizinle bir satıcı ilişkisi kurmaya davet etme

1.  **Müşteriler** ' i seçin ve ardından **bir satıcı ilişkisi iste**' yi seçin.

2.  Sonraki sayfada taslak e-posta iletisini gözden geçirin. Taslak iletiyi varsayılan e-posta uygulamanızda açabilir veya iletiyi panonuza kopyalayıp bir e-postaya yapıştırabilirsiniz. 

    >[!IMPORTANT]
    >E-postanın metnini düzenleyebilirsiniz ama bağlantıyı eklemeyi unutmayın çünkü bu müşteriyi doğrudan hesabınıza bağlayacak kişiselleştirilmiş bir bağlantıdır. 
    
3.  Bu adımı tamamladığınızda **bitti** ' yi seçin.

4.  E-postayı müşterinize gönderin.

5.  Müşteri davetinizi kabul ettikten sonra **müşteriler** sayfanızda görünürler ve servisi buradan müşteri için temin edebilir...

6.  Müşterinin hesabını, hizmetlerini, kullanıcılarını ve lisanslarını yönetmek için, adının yanındaki aşağı oku seçerek müşterinin kaydını genişletin ve ardından yönetmek istediğiniz hizmetin yönetim portalını seçin.

>[!IMPORTANT]  
>Müşteriler, bir hizmetin yönetim portalında yönetici izinlerini yeniden atayabilir veya kaldırabilir. Bununla birlikte, yönetici izinlerinizi kaldıran müşteriye, sizin adına Microsoft 'a bir hizmet isteği açabilmeyeceğiniz anlamına gelir. Müşteriyle anlaşmanızı yeniden başlatana kadar bu hizmet isteği türlerini müşterinin adına açamazsınız.

Müşterileriniz, iş ortaklarının Office 365 Yönetici portalı içinden kiracılarında yönetici ayrıcalıklarına sahip olduğunu bulabilir. Bunu yapmak için:

1. Müşterinin, genel yönetici olarak Office 365 Yönetici portalında oturum açması gerekir.

2. **Ayarlar**  >  **iş ortağı ilişkileri**' ni seçin.

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

Atanan dizin rollerine bağlı olarak her iki grubun üyeleri, müşteri adına iş ortağı kimlik bilgilerini ve yöneticisini kullanarak müşterinin Azure AD kiracısında ve O365 hizmetlerinde oturum açabilir.

Müşteriniz, yönetici ayrıcalıkları atamasını kaldırırsa, Azure AD rol atamaları kaldırılır ve artık müşterinin Azure AD kiracısı yönetimeyeceksiniz.

### <a name="azure-subscriptions-and-resource-management"></a>Azure abonelikleri ve kaynak yönetimi

Her Azure aboneliğinin kendi kaynak yönetimi rolleri kümesi vardır. Bir CSP iş ortağının bir müşterinin Azure aboneliğini yönetebilmesi için, iş ortağının Azure aboneliğinin altındaki bir veya daha fazla role atanması gerekir. Özellikle:

- Bir müşteri bir satıcı davetini kabul ettiğinde ve bir iş ortağı için Temsilcili yönetim ayrıcalığı verdiğinde, iş ortağı müşteri kiracısı kapsamında mevcut Azure aboneliklerine otomatik olarak erişemez.

- CSP iş ortağı müşteri için yeni bir Azure aboneliği sağlarken, CSP iş ortağı kiracısı altındaki yönetici aracıları grubuna aboneliğin altında otomatik olarak sahip rolü atanır. Bu rol ataması temelinde, Grup üyeleri abonelik kapsamındaki kaynaklara erişebilir ve bunları yönetebilir.

- Bir müşteri, Office 365 portalını kullanarak bir iş ortağının Temsilcili yönetim ayrıcalıklarını kaldırdığında, iş ortağı hala abonelik kapsamındaki bir veya daha fazla role atandığı sürece iş ortağı müşterinin Azure aboneliğini yönetebilir. Ortağın Azure aboneliğini yönetmesini durdurmak için, müşterinin rol atamasını kaldırması gerekir.

## <a name="windows-autopilot"></a>Windows Autopilot

Iş Ortağı Merkezi 'nden, CSP iş ortakları, bu koşullarda yönetici ayrıcalıklarına sahip olmaksızın müşterileri için Autopilot profillerini yönetebilir: 

- Bir müşteri Temsilcili yönetim ayrıcalıklarını kaldırırsa ancak sizinle bir satıcı ilişkisi koruursa, Autopilot profillerini yönetmeye devam edebilirsiniz.

- Siz veya başka bir iş ortağının eklemiş olduğu müşteri cihazlarını yönetebilirsiniz. 

- Müşterinizin Iş Microsoft Store, eğitim için Microsoft Store veya Microsoft Intune Portal aracılığıyla eklediği cihazları yönetemezsiniz.

Autopilot hakkında daha fazla bilgi için bkz. [Windows Autopilot ile cihaz kurulumunu basitleştirme](autopilot.md).

>[!IMPORTANT]  
>Iş Ortağı Merkezi 'nde geçerli Autopilot yönetim deneyimi değişmeye devam edebilir. Bu makalenin yayımlandığı sırada aşağıdaki değişiklikler göz önünde bulundurulmaktadır:

- Ortak, iş ortağının profilleri eklemesini/kaldırmasını/kaldırabilmesi ve profili müşteri kiracısındaki herhangi bir cihazdan uygulama/kaldırma işleminden önce müşteri tarafından atanan yönetim ayrıcalığı verilmelidir.

- Ortak, iş ortağının diğer iş ortakları tarafından eklenen cihazları veya müşteri kiracısındaki müşteriyi kaldırabilmesi için müşterinin Temsilcili Yönetim ayrıcalığına sahip olması gerekir. Aksi takdirde, iş ortağı yalnızca daha önce aynı iş ortağı tarafından eklenen cihazları kaldırabilir.
