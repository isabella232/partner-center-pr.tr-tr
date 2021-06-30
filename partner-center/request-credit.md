---
title: Microsoft'tan SLA iade isteğinde bulunma
ms.topic: article
ms.date: 03/31/2021
description: Müşterileriniz hizmet kesintisi yaşamaları için Microsoft'tan hizmet düzeyi sözleşmesi (SLA) kredisi talep etmek için avantajları, kısıtlamaları ve yordamları öğrenin.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: f521e55869d60987fb46cd5d570bf206939e0782
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080648"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Microsoft'tan hizmet düzeyi sözleşmesi (SLA) kredisi nasıl ve ne zaman talep edilebilir?

**Uygun roller:** Yönetici aracısı | Genel yönetici

Müşterileriniz için sağlamakta olduğu bir hizmette kesinti olursa Microsoft'tan hizmet düzeyi sözleşmesi **(SLA)** kredileri isteği alabilirsiniz.

## <a name="sla-credit-calculation"></a>SLA kredi hesaplaması

Microsoft'un SLA kredileri, hangi hizmetlerden etkilenlerine bağlı olarak belirlenir. Örneğin, müşterinizin bir Office 365 paketi varsa ancak yalnızca SharePoint kesintisi yaşanıyorsa, SLA kredisi yalnızca SharePoint için onaylanır ve müşterinin planının tamamı için onaylanmaz.

*Krediler, etkilenen hizmete ve kesinti süresine göre provok olarak derecelendirilmiştir.* SLA kredileri için uygun senaryo türlerini görmek için Çevrimiçi Hizmetler Birleştirilmiş [SLA belgesine bakın.](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37) Bu bilgiler, Bulut Çözümü Sağlayıcısı (CSP) programı aracılığıyla satılan hizmetler için de geçerlidir.


## <a name="request-an-sla-credit"></a>SLA kredisi isteği

*CSP iş ortağının talebi ve tüm gerekli bilgileri olayın meydana geldiği ayı takip eden takvim ayı sonuna kadar göndermesi gerekir.* Örneğin, olay 15 Şubat'ta oluştu ise Microsoft'un talebi ve tüm gerekli bilgileri 31 Mart'a kadar almaları gerekir. Son müşteriler ve dolaylı kurumsal bayiler, SLA kredi talepleri gönderemektedir; Dolaylı sağlayıcı veya doğrudan fatura iş ortağının talepleri kendileri adına göndermesi gerekir.

> [!NOTE]
> Danışmanlık olayları SLA kredileri için uygun değildir. Hizmet Durumu Panosu'na gönderilen bir  olay, kiracının etki altında olduğunu gösterir ve yayımlama zamanında Microsoft'un sahip olduğu en iyi bilgileri temsil eder. Sistem durumu sayfası verileri bir hizmetin genel kullanılabilirliğini temsil eder. Tek tek hizmet etkisi, azaltma ve çözüm farklılık gösterebilir. Diğer ayrıntılar için son Olay Gönderisini ve Olay Sonrası Gözden Geçirmeyi gözden geçirebilirsiniz. Daha [fazla bilgi için Microsoft 365 hizmet durumunu](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) denetleme.

### <a name="required-information"></a>Gerekli bilgiler

Müşteri adı, kiracı tanımlayıcısı, iş ortağı bileti# ve oluşturulan bilet tarih/saat damgası bir talebin işlenmesi için yeterli değildir.

[Microsoft'a bir SLA kredi isteği](#submit-sla-credit-request) göndermeden önce, destek **biletinize** eklemek için aşağıdaki tüm bilgileri toplamanız gerekir:

- Müşteri kiracısı GUID'si
- Kesinti [olayı tanımlayıcısı?](#outage-incident-identifier)
- Müşterinin kesintiden etki olduğuna ve SLA kredisi isteğine sahip olduğuna dair kanıt.
- Etkilene abonelikler CSP aracılığıyla mı satın alındı? (*evet* veya *hayır*)

#### <a name="evidence-that-proves-customer-impact"></a>Müşterinin etkisini kanıtlayacak kanıt

- Kapalı kalma süresi ve süresiyle ilgili bilgiler
- Etkilenen kullanıcıların sayısı ve konumları (varsa)
- Olay oluşma zamanında olayı çözümleme girişimlerinizin açıklamaları
- Etkilene müşteriden destek ve daha sonra kredi isteği e-postası
- Hizmet etkisini çözümleme konusunda destek bileti numarası ve müşteriyle iletişimin ayrıntıları


#### <a name="outage-incident-identifier"></a>Kesinti olayı tanımlayıcısı

Kesinti olayı tanımlayıcısını hizmet durumu sayfasındaki **Hizmet** Durumu sayfasında Microsoft 365 yönetim merkezi. Kesinti **Olay Kimliği,** etkilenen hizmeti (örneğin, Exchange Online kesintisi için *EX25194)* belirten iki harfli bir kısaltmadan önce gelen bir sayıdır. Aşağıdaki tabloda Common Service kısaltmaları açıkmektedir:

| İki harfli kısaltma | Microsoft hizmeti |
| ----------------------- | ----------------- |
| Ex | Exchange Online |
| Fo | Exchange Online Protection |
| Sb | Skype Kurumsal Çevrimiçi Sürüm (eski adı Lync Online) |
| İşletim Sistemi | Office Aboneliği |
| PB | Office 365 için Power BI |
| Sp | SharePoint Online |
| YA | Yammer Enterprise |
| MO | Portal hatası |

### <a name="submit-sla-credit-request"></a>SLA kredi isteği gönderme

SLA kredi isteğinizi Microsoft'a İş Ortağı Merkezi için:

1. İş Ortağı Merkezi panosunda oturum açın.
2. Sol menüde Hizmet istekleri'ne ve ardından **İş ortağı** destek **istekleri'ne tıklayın.**
3. İş ortağı **isteği sayfasında Yeni** **istek'i seçin.**
4. İsteği **başlat sayfasında** **CSP - müşteriler, siparişler ve abonelikler bölümünü bulun.** Bu bölümde Sorun türü **seçin'i ve ardından** Müşteri hizmetleri **kredi istekleri'ne tıklayın.**
5. Önerilen **çözümler sayfasında, Daha** fazla yardıma **ihtiyacınız var mı?** altında Evet'i **seçin.**
6. Ayrıntılar **sayfasında** Sorun ayrıntıları **bölümünü** doldurun. Ayrıntılar **metin** kutusuna daha önce toplanmış olan [gerekli bilgileri](#required-information) girmeyin.
7. SLA **kredi** isteğinizi göndermek için Gönder'i seçin.

## <a name="next-steps"></a>Sonraki adımlar

- [Sorunları müşteriniz adına bildirme](report-problems-on-behalf-of-a-customer.md)
