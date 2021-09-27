---
title: Microsoft tarafından verilen IRS vergi formlarını anlama
description: Microsoft tarafından verilen vergi formlarını, bunları alacak olan kişi ve bunların ne zaman kullanılabilir olduğu da dahil olmak üzere öğrenin.
ms.topic: article
author: mingshen-ms
ms.author: mingshen
ms.service: partner-dashboard
ms.subservice: partnercenter-payouts
ms.localizationpriority: medium
ms.date: 09/30/2020
ms.openlocfilehash: 2e057219696de5eac300f9b6778489e047aceaad
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129073318"
---
# <a name="understand-irs-tax-forms-issued-by-microsoft"></a>Microsoft tarafından verilen IRS vergi formlarını anlama

**Uygun roller:** Genel yönetici

Her yıl Microsoft'tan bir veya daha fazla vergi formu alırsınız. Bu, konumunuz ve size gelen satış veya ödeme miktarına bağlıdır. Microsoft'un bu formları verilerle (IRS) Internal Revenue Service gerekir.

Bu makalede, bu formlar hakkında, bunları alacak olan ve ne zaman kullanılabilir hale gelecekleri de dahil olmak üzere daha fazla açıklanmıştır.

## <a name="types-of-tax-forms"></a>Vergi formu türleri

| IRS vergi formu | Açıklama | Kullanılabilirlik |
|--------------|-------------|--------------|
|1099-MISC, 1099-K | Microsoft'un marketlere katılımı için size yapılan satış etkinliği ve/veya ödemelerle ilgili | Yazdırılan formlar **31** Ocak'ta veya daha önce işaretli olur ve .pdf kopyaları ödeme ve İş Ortağı Merkezi [profillerde kullanılabilir.](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) |
|1042-S | Stopaj vergisine tabi olan, size Birleşik Devletler ilgili | Yazdırılan formlar **15** Mart'ta veya 15 Mart'tan önce sonlanır ve .pdf kopyaları aynı anda İş Ortağı Merkezi'de **(İş Ortağı Merkezi Developer Ayarlar'de** Ödeme ve vergi **>** ödeme ve vergi profilleri altında) kullanılabilir.  |

> [!NOTE]
> IRS vergi formlarında kullanmakta olduğu adres, ödeme hesabınız ve vergi formlarınızı ayar her zaman vergi [profilinizde yer alan adresten gelir.](set-up-your-payout-account.md) Adresiniz değişti ise, Vergi profilinizde adresi **güncelleştirin.**

Vergi formları aşağıdaki adreslerden size gönderilir:

**ABD Vatandaşları:**

| İş Grubu         | Tüzel          | Adres                                          |
|------------------------|-----------------------|--------------------------------------------------|
| Windows, Office, Azure | Microsoft Corporation | One Microsoft Way<br>Redmond, WA 98052 ABD       |
| Reklam            | Microsoft Online Inc. | 6880 Sierra Center Parkway<br>Reno, NV 98511 ABD |

**ABD Dışı Vatandaşlar:**

| İş Grubu         | Tüzel          | Adres                                          |
|------------------------|-----------------------|--------------------------------------------------|
| Windows, Office, Azure | Microsoft Ireland Operations Limited (Ödeme, Microsoft Corporation için nitelikli aracı olarak hareket eden Microsoft İrlanda aracılığıyla Microsoft Corporation) | One Microsoft Place<br>South County Business Park<br>Leopards london, Dublin 18, D18 P521, İrlanda|
| Reklam          | Microsoft Ireland Operations Limited (Ödeme Microsoft Online Inc. tarafından Microsoft Online Inc. için ödeme aracısı olarak hareket eden Microsoft İrlanda aracılığıyla yapılır.) | One Microsoft Place<br>South County& Business Park<br>Leopards london, Dublin 18, D18 P521, İrlanda |
| Reklam            | Microsoft Online Inc. | 6880 Sierra Center Parkway<br>Reno, NV 98511 ABD |

>[!NOTE]
> \* Reklam geliri elde eden şu ülkelerin vatandaşları Microsoft Ireland Operations Limited aracılığıyla ödeme yapacak: Malezya, Hollanda, Afrika, Fransa, Almanya, Çekya, Norveç, Finlandiya, Finlandiya, Fransa, Almanya, Norveç, İrlanda, isle of Man, İtalya, Leton, Liechtenstein, Liechtenstein, Yerkağ, İşkoş, Norveç, İşle, Güney Afrika, İspanya, İsveç, İsviçre, Birleşik Krallık

## <a name="for-developers-located-in-the-united-states"></a>Birleşik Devletler'de bulunan geliştiriciler için

| Ücretli uygulama satışı yapan Birleşik Devletler geliştiriciyim ve...   | Şu formu alalım: |
|------------------------|-----------------------|
| İlgili vergi **yılında 20.000** ABD dolarının üzerinde olan bu satışların toplam satın alma tutarıyla **200'den** fazla uygulama satışım vardı **(Brezilya** ve Çin'de yapılan satışları Windows 10 üzerinde Microsoft Store.)| **1099-K:**<br/>Filer: Microsoft Corporation<br/>EIN: \* \* \* \* \* 4442<br/><br/>**Önemli:** Form 1099-K, **size yapılan ödemeleri** değil, brüt satın alma tutarlarını içerir.| 
| (i) Brezilya ve Çin'de yapılan uygulama satışları için Windows 10 üzerinde Microsoft Store veya (ii) Minecraft Market'te yapılan ödemelerde en az **10** ABD doları aldı.<br/><br/>**OR**<br/><br/>İlgili vergi yılında Microsoft'tan uygulama satışları ile ilgili değil en az 600 ABD doları ödeme aldım (örneğin, teşvik ödemeleri veya bir yarışmadan veya promosyondan ödemeler)| **1099-MISC:**<br/>Ödeme: Microsoft Corporation<br/>EIN: \* \* \* \* \* 4442<br/><br/>**Önemli:** Bazı iş varlıkları, Microsoft'tan alınan ödeme tutarlarından bağımsız olarak 1099 MISC formu almaz.  Daha fazla bilgi için vergi uzmanınıza danışın.| 
| Yukarıdakilerin hiçbiri geçerli değildir.| Hiçbiri |
| <br/><br/>**Uygulamalarda reklam satan Birleşik Devletler geliştiriciyim ve...** |<br/><br/>**Şu formu alalım:** |
|İlgili vergi yılında uygulamalarda yer alan reklamlardan en az **600** ABD doları ödeme aldı. | **1099-MISC:**<br/>Payer: Microsoft Online Inc<br/>EIN: \* \* \* \* \* 0505<br/><br/>**Önemli:** Bazı iş varlıkları, Microsoft'tan alınan ödeme tutarlarından bağımsız olarak 1099 MISC formu almaz.  Daha fazla bilgi için vergi uzmanınıza danışın. |
| İlgili vergi **yılında uygulamalarda yer alan reklamlardan 600** ABD dolarından az ödeme aldı. | Hiçbiri |


## <a name="for-developers-located-outside-of-the-united-states"></a>Uygulamanın dışında bulunan geliştiriciler Birleşik Devletler


| **Soru** | **Yanıt** |
|---|---|
| **Microsoft'tan 1042-S formu aldı. Bu ne için?** | Microsoft size 1042-S formu veya formları sağladı çünkü size vergi dairesine raporlanabilir olarak kabul edilen ve stopaj vergisine tabi Birleşik Devletler gelir ödememiz gerekir.  Bu raporlama gereksinimi için Form 1042-S kullanılır. | 
| **Formlarla ne yapabilirim?** | Genel olarak, sizin tarafınıza özel bir eylem gerekmez. Herhangi bir vergi kredisi formu için yerel vergi yetkililerinize uygulamak istediğiniz 1042-S formu sizin için yararlı olabilir.  Bu konu hakkında daha fazla bilgi almak için kendi vergi danışmanlarınıza danışın. | 
| **W8 formunu tamamlaya kadar ödemelerimin vergileri neden yardımla karşılandı?** | Vergiler şu şekilde olursa yardımdan muaf olur:<br/><br/>1. W8'in vergi vergi bölümünü doğru tamamlamadınız veya <br/>2. Vergi vergisini ödemeyen bir ülkede Birleşik Devletler.<br/><br/>Güncelleştirilmiş bir W8 İş Ortağı Merkezi göndermek için herhangi bir zamanda bu sayfayı ziyaret edin.<br/><br/> **Not:** Gelirlerin hepsi vergi stopajı durumuna tabi değildir. | 
| **Geçerli bilgilerle güncelleştirilmiş bir W8 formu gönderildi. Microsoft, yardımdan muaf olan vergiyi iade ediyor mu?** | Vergiler geri alındıktan sonra para iadesi alınamaz. Vergi danışmanlarınıza başvurarak bu vergiler için yerel bir kredi talep edip edilip ediley olmadığı veya IRS'den para iadesi alınıp alınıp alınamayyıp alınamayışlarını tartışarak. | 
| **1042-S formunda hangi satışlar raporlandı?** | Yalnızca **Vergi stopajı 'na tabi olarak sınıflandırılan Birleşik Devletler bulunan alıcıların** satışları raporlanabilir hale getirilir.  Diğer tüm satışlar raporlanabilir olarak kabul edilmez. | 
| **Neden tek bir zarfa ait 1042-S formunun üç kopyasını aldım?** | IRS düzenlemeleri için formun üç kopyasının sağlanması gerekir:<br/><br/>-Alıcı kayıtları için bir tane<br/>-Bir Birleşik Devletler federal vergi iadesi (varsa)<br/>-Bir Birleşik Devletler durum vergisi dönüşü (varsa) |

> [!NOTE]
> **IRS vergi formlarıyla** ilgili ek sorularınız veya endişeleriniz varsa, Iş Ortağı Merkezi panosunda [Yardım + Destek](https://partner.microsoft.com/dashboard/support/) bölümüne gidin. Microsoft, belirli vergi şartlarınızla ilgili soruları yanıtlayamıyor; Bu sorular için lütfen vergi uzmanınızdan gelen önerileri arayın.

## <a name="next-steps"></a>Sonraki adımlar

- [Ticari markette ödeme alma](marketplace-get-paid.md)
