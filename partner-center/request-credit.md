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
ms.openlocfilehash: 100a3d2988c19d57f7426c7212b7464d8e96dc94
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152962"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Microsoft'tan hizmet düzeyi sözleşmesi (SLA) kredisi nasıl ve ne zaman talep edilebilir?

**Uygun roller:** Yönetici aracısı | Genel yönetici

Müşterileriniz için sağlamakta olduğu bir hizmette kesinti olursa Microsoft'tan hizmet düzeyi sözleşmesi **(SLA)** kredileri talep edilebilir.

## <a name="sla-credit-calculation"></a>SLA kredi hesaplaması

Microsoft'un SLA kredileri, hangi hizmetlerden etkilenenin bağlı olarak belirlenir. Örneğin, müşterinizin bir Office 365 paketi varsa ancak yalnızca SharePoint kesintisi yaşanıyorsa, SLA kredisi yalnızca SharePoint için onaylanır ve müşterinin planının tamamı için onaylanmaz.

*Krediler, etkilenen hizmete ve kesinti süresine göre provok olarak derecelendirilmiştir.* SLA kredileri için uygun senaryo türlerini görmek için Çevrimiçi Hizmetler Birleştirilmiş [SLA belgesine bakın.](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37) Bu bilgiler, Bulut Çözümü Sağlayıcısı programı aracılığıyla satılan hizmetler için de geçerlidir.


## <a name="request-an-sla-credit"></a>SLA kredisi isteği

*Bulut Çözümü Sağlayıcısı (CSP) iş ortağının talebi ve tüm gerekli bilgileri olayın meydana geldiği ayı takip eden takvim ayı sonuna kadar göndermesi gerekir.* Örneğin, olay 15 Şubat'ta oluştu ise Microsoft'un talebi ve tüm gerekli bilgileri 31 Mart'a kadar almaları gerekir. Son müşteriler ve dolaylı kurumsal bayiler SLA kredi talepleri gönderemektedir; Dolaylı sağlayıcı veya doğrudan fatura iş ortağının talepleri kendileri adına göndermesi gerekir.

>[!NOTE]
>Danışmanlık olayları ([Hizmet durumunu Microsoft 365)](/microsoft-365/enterprise/view-service-health#incidents-and-advisories)SLA kredileri için uygun değildir.

### <a name="required-information"></a>Gerekli bilgiler

Müşteri adı, kiracı tanımlayıcısı, iş ortağı bileti# ve oluşturulan bilet tarih/saat damgası bir talebin işlenmesi için yeterli değildir.

[Microsoft'a bir SLA kredi isteği](#submit-sla-credit-request) göndermeden önce destek **biletinize** eklemek için aşağıdaki tüm bilgileri toplamanız gerekir:

- Müşteri kiracısı GUID'si
- Kesinti [olayı tanımlayıcısı?](#outage-incident-identifier)
- Müşterinin kesinti tarafından etkilendiğine ve bir SLA Kredisi istemiş olduğunu kanıtlandı.
- CSP aracılığıyla satın alınan etkilenen abonelikler mi? (*Evet* veya *Hayır*)

#### <a name="evidence-that-proves-customer-impact"></a>Müşteri etkisini kanıtlayan kanıt

- Kapalı kalma süresinin süresi ve süresiyle ilgili bilgiler
- Etkilenen kullanıcıların sayısı ve konumları (varsa)
- Olay oluşma sırasında çözülmesi girişimlerinizin açıklamaları
- Etkilenen müşteriden gelen ve daha sonra kredi isteyen bir e-posta
- Hizmet etkisini çözme ile ilgili olarak müşteri kişisinin destek bileti numarası ve ayrıntıları


#### <a name="outage-incident-identifier"></a>Kesinti olayı tanımlayıcısı

Kesinti olayı tanıtıcısını, Microsoft 365 Yönetim Merkezi 'ndeki **hizmet durumu** sayfasında bulabilirsiniz. **Kesinti OLAYı kimliği** , etkilenen hizmeti (örneğin, Exchange Online kesintisi için *EX25194* ) gösteren iki harfli kısaltmadan önce gelen bir sayıdır. Takip tablosu yaygın hizmet kısaltmalarını açıklar:

| İki harfli kısaltma | Microsoft hizmeti |
| ----------------------- | ----------------- |
| DEĞERINE | Exchange Online |
| INFO | Exchange Online koruması |
| Ise | Skype Kurumsal Çevrimiçi (eski adıyla Lync Online) |
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
