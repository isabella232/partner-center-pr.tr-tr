---
title: Abonelikleri yeni ticarete geçir
ms.topic: article
ms.date: 10/04/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Abonelikler geçirmeye yönelik yeni ticari deneyimler hakkında bilgi edinin.
author: iragulati1
ms.author: iragulati
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bad50c36cd0e0523fe70115e0b39d88e0e68ab68
ms.sourcegitcommit: 462d6026287b85c9feea602af5bcdf924f3e6976
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/05/2021
ms.locfileid: "129454671"
---
# <a name="introduction-migrate-subscriptions-to-new-commerce"></a>Giriş: abonelikleri yeni ticarete geçirme

**Uygun roller**: yönetici Aracısı | Satış Aracısı | Genel yönetici

> [!NOTE]
> yeni ticari deneyim değişiklikleri şu anda yalnızca Microsoft 365/dynamics 365 yeni ticaret deneyimi technical preview 'ın parçası olan iş ortakları tarafından kullanılabilir.
Abonelikler, uygunluk ölçütüne uyuyorsa ve LIKE teklifi gibi bir kullanılabilir ise, iş ortakları abonelikleri yeni ticarete geçirebilir.

## <a name="ineligible-subscriptions"></a>Kaçınak abonelikler ##

Tüm abonelikler Şu anda geçiş için uygun olmayacaktır. Aşağıdaki abonelik kategorileri Şu anda uygun değil: 

- Etkin olmayan abonelikler (bir abonelik devre dışı olduğunda hizmette değişiklik gerçekleşmez) 

- Deneme abonelikleri (parasal avantaj veya etkileri yoktur; beklentileri, deneme süresi eskileri çalıştıralım 

- Promosyonlara sahip abonelikler (NCE 'deki yükseltmeler, eski sürümündeki bu promosyonların bağımsızdır) 

- Eklentiler içeren abonelikler (Eklentileri Eklentiler ile geçirme, daha sonra etkinleştirilecek; Şu anda, birlikte geçiş işlemini destekliyoruz) 

- Gov, edu veya kar amacı olmayan kitleler için abonelikler (bilinen tekliflerin eskiden NCE 'ye eşlenmesi desteklenmez) 

- Kullanımdan kaldırılan veya kullanım dışı bırakılmış abonelikler (bu abonelikler için, yeni ticaret ortamında teklif sunmak gibi bir işlem olmaz) 

Yukarıdaki aboneliklerin geçişleri Şu anda bu özellik için kapsam dışında. Ayrıca, tek bir abonelik, abonelik toplu işleri yerine geçiş birimi olur. 

## <a name="suspending-a-legacy-subscription-during-migration"></a>Geçiş sırasında eski bir aboneliği askıya alma ##

Eski bir abonelik, abonelik için başarılı bir yeni ticaret yolu sağlandıktan sonra askıya alınır. Bu yetenek, bir aboneliğin geçişini Başlatan bir Iş ortağının takip eden engelleyiciler varsa hizmet kaybını önler. Ayrıca, hem eski hem de yeni ticaret abonelikleri için bir Double faturalandırma gerçekleşmeyecektir. Geçiş başlatıldıktan sonra, NCE aboneliğine ilişkin faturalandırmayla ilgili herhangi bir çakışma oluşmasını engellemek için eski abonelik için faturalandırma durdurulur.

## <a name="billing-term-and-frequency"></a>Faturalama dönemi ve sıklığı ##

Geçirilen abonelik için faturalandırma dönemi ve faturalandırma sıklığı, eski aboneliğin fatura dönemi ve faturalandırma sıklığıyla aynı kalacaktır; dönem bitiş tarihi aynı kalacaktır.

## <a name="new-commerce-promotions"></a>Yeni ticaret promosyonları ##

Promosyonların eski sürümündeki abonelikler geçiş için uygun değildir. Geçirilen abonelikler, yeni ticari tanıtım promosyonları için uygun olabilir. Promosyonlar, geçiş noktasındaki abonelik döneminin geri kalanına eşit olarak dağıtılır. 

## <a name="cancelling-subscriptions-or-decreasing-licenses"></a>Abonelikleri iptal etme veya lisans azaltma ##

Geçiş sonrasında, 72 saatlik bir iptal penceresi vardır. Bu 72 saat içinde, Iş ortakları aboneliği iptal edebilir veya Bu penceredeki lisans miktarını azaltabilir. Geçişin tamamlandığı zamandan itibaren 24 saat zaman içinde, aboneliğin veya lisansların iptallerinin bir gününde kullanılması eşit olarak dağıtılır; geçişin tamamlandığı zamandan itibaren 48 saat zaman içinde, aboneliğin veya lisansların iptallerinin süresi iki günlük kullanım için eşit olarak dağıtılır. 

## <a name="migration-history"></a>Geçiş geçmişi ##

API 'Ler aracılığıyla geçiş geçmişiyle ilgili ayrıntıların başlangıç ve tamamlanma koşulları gibi ayrıntılara yeni GetMigration API ve MigrationID alanı kullanılarak erişilebilir. UX üzerinde, yeni NCE aboneliğinin geçirildiği abonelik KIMLIĞI, müşterinin "abonelikler" sayfasındaki Abonelik satırı öğesine tıklandıktan sonra erişilen Ayrıntılar sayfasının en üstünde görünür. 

## <a name="apis"></a>API'ler ##

Benzer aboneliklerin geçişi için 3 yeni REST API 'si piyasaya sürüldü. İlk "CheckMigration" API 'SI bir abonelik için geçişe uygunluk denetimi sağlayacaktır. Abonelik uygun olduğunda ikinci "CreateMigration" API 'SI geçişi oluşturacaktır. Son olarak, üçüncü "GetMigration" API 'SI Iş ortağının geçiş durumunu denetlemesine izin verir. 
