---
title: Microsoft'tan SLA iade isteğinde bulunma
ms.topic: article
ms.date: 03/31/2021
description: Müşterileriniz bir hizmet kesintisi yaşanırsa, Microsoft 'tan bir hizmet düzeyi sözleşmesi (SLA) kredisi istemek için avantajları, kısıtlamaları ve yordamları öğrenin.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: d33188510b127873864260199ff92018e1a4d995
ms.sourcegitcommit: 766b2bb46dffd29e532b42106359f83e51b96700
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/31/2021
ms.locfileid: "106103834"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Microsoft 'tan bir hizmet düzeyi sözleşmesi (SLA) kredisi isteme

Müşterileriniz için sağladığınızı bir hizmet kesintiye neden olursa, Microsoft 'tan **hizmet düzeyi sözleşmesi (SLA) kredileri** isteyebileceksiniz.

## <a name="sla-credit-calculation"></a>SLA kredi hesaplaması

Microsoft 'tan alınan SLA kredileri, hangi hizmet (ler) in etkilendiğini temel alır. Örneğin, müşterinizin bir Office 365 paketi varsa ancak yalnızca bir SharePoint kesintisi yaşanıyorsa, SLA Kredisi yalnızca SharePoint için onaylanır ve müşterinin tüm planı değildir.

*Krediler, etkilenen hizmet ve kesinti süresi temel alınarak Pro derecelendirilir.* SLA kredilerine uygun olan senaryoların türlerini görmek için bkz. [çevrimiçi hizmetler BIRLEŞTIRILMIŞ SLA belgesi](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37). Bu bilgiler, bulut çözümü sağlayıcısı programı aracılığıyla satılan hizmetler için geçerlidir.


## <a name="request-an-sla-credit"></a>SLA Kredisi isteme

*Bulut çözümü sağlayıcısı (CSP) iş ortağı, olayın gerçekleştiği ay sonra takvim ayının sonuna kadar talebi ve tüm gerekli bilgileri göndermesi gerekir.* Örneğin, olay 15 Şubat 'ta oluştuysa, Microsoft bu isteği ve tüm gerekli bilgileri 31 Mart tarihine kadar almalıdır. Son müşteriler ve dolaylı satıcılar SLA kredi taleplerini gönderemez; dolaylı sağlayıcı veya doğrudan fatura ortağı kendi adına talepler göndermesi gerekir.

>[!NOTE]
>Danışmanlık olayları ([Microsoft 365 hizmeti sistem durumunu denetleme](https://docs.microsoft.com/microsoft-365/enterprise/view-service-health?&preserve-view=trueo365-worldwide#incidents-and-advisories)) SLA kredileri için uygun değildir.

### <a name="required-information"></a>Gerekli bilgiler

Müşteri adı, kiracı tanımlayıcısı, iş ortağı bileti # ve bilet oluşturma tarih/saat damgası, bir talebin işlenmesine yetecek kadar yeterli değildir.

Microsoft 'a [BIR SLA Kredisi isteği göndermeden](#submit-sla-credit-request) önce, destek biletine dahil etmek için aşağıdaki **Tüm** bilgileri toplamanız gerekir:

- Müşteri kiracının GUID 'SI
- [Kesinti olayı tanımlayıcısı](#outage-incident-identifier)?
- Müşterinin kesinti tarafından etkilendiğine ve bir SLA Kredisi istemiş olduğunu kanıtlandı.
- CSP aracılığıyla satın alınan etkilenen abonelikler mi? (*Evet* veya *Hayır*)

#### <a name="evidence-that-proves-customer-impact"></a>Müşteri etkisini kanıtlayan kanıt

- Kapalı kalma süresinin süresi ve süresiyle ilgili bilgiler
- Etkilenen kullanıcıların sayısı ve konumları (varsa)
- Olay oluşma sırasında çözülmesi girişimlerinizin açıklamaları
- Etkilenen müşteriden gelen ve daha sonra kredi isteyen bir e-posta
- Hizmetin etkisinin çözümlenmesinden bağımsız olarak müşterinin ilgili kişisinin destek bileti numarası ve ayrıntıları


#### <a name="outage-incident-identifier"></a>Kesinti olayı tanımlayıcısı

Kesinti olayı tanıtıcısını, Microsoft 365 Yönetim Merkezi 'ndeki **hizmet durumu** sayfasında bulabilirsiniz. **Kesinti OLAYı kimliği** , etkilenen hizmeti (örneğin, Exchange Online kesintisi için *EX25194* ) gösteren iki harfli kısaltmadan önce gelen bir sayıdır. Takip tablosu yaygın hizmet kısaltmalarını açıklar:

| İki harfli kısaltma | Microsoft hizmeti |
| ----------------------- | ----------------- |
| DEĞERINE | Exchange Online |
| INFO | Exchange Online koruması |
| Ise | Skype Kurumsal Çevrimiçi (eski adıyla Lync Online) |
| İşletim Sistemi | Office aboneliği |
| PB | Office 365 için Power BI |
| SP2 | SharePoint Online |
| ASKıYA | Yammer Kurumsal |
| MO | Portal hatası |

### <a name="submit-sla-credit-request"></a>SLA kredi isteği gönder

SLA kredi isteğinizi Iş Ortağı Merkezi panosu üzerinden Microsoft 'a göndermek için:

1. İş Ortağı Merkezi panosunda oturum açın.
2. Sol taraftaki menüde **hizmet istekleri**' ni seçin ve **iş ortağı destek istekleri**' ni seçin.
3. **Iş ortağı isteği** sayfasında, **yeni istek**' ı seçin.
4. **Isteği Başlat** sayfasında, **CSP-müşteriler, siparişler ve abonelikler** bölümünü bulun. Bu bölümde, **bir sorun türü seçin**' i seçin ve ardından **Müşteri Hizmetleri kredi istekleri**' ni seçin.
5. **Önerilen çözümler** sayfasında, **daha fazla yardıma mı ihtiyacınız var?** altında **Evet**' i seçin.
6. **Ayrıntılar** sayfasında, **Sorun ayrıntıları** bölümünü doldurun. **Ayrıntılar** metin kutusunda, daha önce topladığınız [gerekli bilgileri](#required-information) girdiğinizden emin olun.
7. SLA kredi isteğiniz içinde göndermek için **Gönder** ' i seçin.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşterinizin adına sorunları bildirin](report-problems-on-behalf-of-a-customer.md)
