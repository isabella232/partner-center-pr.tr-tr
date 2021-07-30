---
title: Microsoft'tan SLA iade isteğinde bulunma
ms.topic: article
ms.date: 03/31/2021
description: Müşterileriniz bir hizmet kesintisi yaşanırsa, Microsoft 'tan bir hizmet düzeyi sözleşmesi (SLA) kredisi istemek için avantajları, kısıtlamaları ve yordamları öğrenin.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: d98130f22fee81a50b40b8ae08a3fcf909201389
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2021
ms.locfileid: "114839694"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Microsoft 'tan bir hizmet düzeyi sözleşmesi (SLA) kredisi isteme

**Uygun roller**: yönetici Aracısı | Genel yönetici

Müşterileriniz için sağladığınızı bir hizmet kesintiye neden olursa, Microsoft 'tan **hizmet düzeyi sözleşmesi (SLA) kredileri** isteyebilirsiniz.

## <a name="sla-credit-calculation"></a>SLA kredi hesaplaması

Microsoft 'tan alınan SLA kredileri, hangi hizmet (ler) in etkilendiğini temel alır. örneğin, müşterinizin bir Office 365 paketi varsa ancak yalnızca bir SharePoint kesintisi yaşanıyorsa, SLA kredisi yalnızca SharePoint için onaylanır ve müşterinin tüm planı değildir.

*Krediler, etkilenen hizmet ve kesinti süresi temel alınarak Pro derecelendirilir.* SLA kredilerine uygun olan senaryoların türlerini görmek için bkz. [çevrimiçi hizmetler BIRLEŞTIRILMIŞ SLA belgesi](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37). bu bilgiler, Bulut Çözümü Sağlayıcısı (CSP) programı aracılığıyla satılan hizmetler için geçerlidir.


## <a name="request-an-sla-credit"></a>SLA Kredisi isteme

*CSP iş ortağı, olayın gerçekleştiği ay sonra takvim ayının sonuna kadar talebi ve tüm gerekli bilgileri göndermesi gerekir.* Örneğin, olay 15 Şubat 'da oluştuysa, Microsoft talep ve tüm gerekli bilgileri 31 Mart 'a almalıdır. Son müşteriler ve dolaylı satıcılar SLA kredi taleplerini gönderemez; dolaylı sağlayıcı veya doğrudan fatura ortağı kendi adına talepler göndermesi gerekir.

> [!NOTE]
> Danışmanlık olayları genellikle SLA kredileri için uygun değildir. Hizmet durumu panosuna gönderilen bir olay, *bir kiracının etkilenip etkilenmeyeceğini* ve Microsoft 'un yayımlama sırasında sahip olduğu en iyi bilgileri temsil ettiğini gösterir. Sağlık sayfası verileri bir hizmetin genel kullanılabilirliğini temsil eder. Tek tek hizmet etkisi, risk azaltma ve çözüm farklılık gösterebilir. Daha fazla ayrıntı için son olay sonrası ve olay sonrası Incelemesini gözden geçirebilirsiniz. daha fazla bilgi için bkz. [Microsoft 365 hizmeti sistem durumunu denetleme](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) .

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
- Hizmet etkisini çözme ile ilgili olarak müşteri kişisinin destek bileti numarası ve ayrıntıları


#### <a name="outage-incident-identifier"></a>Kesinti olayı tanımlayıcısı

kesinti olayı tanımlayıcısını Microsoft 365 yönetim merkezi **hizmet durumu** sayfasında bulabilirsiniz. **kesinti olayı kimliği** , etkilenen hizmeti gösteren iki harfli kısaltmadan önce gelen bir sayıdır (örneğin, bir Exchange Online kesintisi için *EX25194* ). Takip tablosu yaygın hizmet kısaltmalarını açıklar:

| İki harfli kısaltma | Microsoft hizmeti |
| ----------------------- | ----------------- |
| DEĞERINE | Exchange Online |
| INFO | Exchange Online Protection |
| Ise | Skype Kurumsal Çevrimiçi (eski adıyla Lync Online) |
| İşletim Sistemi | Office Aboneliğiniz |
| PB | Office 365 için Power BI |
| SP2 | SharePoint Online |
| ASKıYA | Yammer Enterprise |
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
