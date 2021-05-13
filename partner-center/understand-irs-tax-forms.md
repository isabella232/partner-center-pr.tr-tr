---
title: Microsoft tarafından verilen IRS vergi formlarını anlama
description: Microsoft tarafından verilen vergi formlarını, bunları alacak olan kişi ve bunların ne zaman kullanılabilir olduğu da dahil olmak üzere öğrenin.
ms.topic: article
author: mingshen-ms
ms.author: mingshen
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.localizationpriority: medium
ms.date: 09/30/2020
ms.openlocfilehash: d34984c3bbe8588cf2a5a40f7c50b14ba6928405
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818686"
---
# <a name="understand-irs-tax-forms-issued-by-microsoft"></a>Microsoft tarafından verilen IRS vergi formlarını anlama

**Uygun roller:** Genel yönetici

Her yıl Microsoft'tan bir veya daha fazla vergi formu alırsınız. Bu, konumunuz ve size gelen satış veya ödeme miktarına bağlıdır. Microsoft'un bu formları verilerle (IRS) Internal Revenue Service gerekir.

Bu makalede, bu formlar hakkında, bunları alacak olan ve ne zaman kullanılabilir hale gelecekleri de dahil olmak üzere daha fazla açıklanmıştır.

## <a name="types-of-tax-forms"></a>Vergi formu türleri

| IRS vergi formu | Description | Kullanılabilirlik |
|--------------|-------------|--------------|
|1099-MISC, 1099-K | Microsoft'un marketlere katılımı için size yapılan satış etkinliği ve/veya ödemeler ile ilgili | Yazdırılan formlar **31** Ocak'ta veya 31 Ocak'tan önce sonlanır ve .pdf  kopyaları aynı anda [İş Ortağı Merkezi'de](https://partner.microsoft.com/dashboard) (Ödeme ve vergi İş Ortağı Merkezi Ödeme ve vergi profilleri altında **>** Hesabı ayarlarında) kullanılabilir. |
|1042-S | Stopaj vergisine tabi olan, size Birleşik Devletler ilgili | Yazdırılan formlar 15 Mart'ta veya **15** Mart'tan önce ve .pdf kopyaları aynı anda İş Ortağı Merkezi'de (Ödeme ve vergi > Ödeme ve vergi profilleri altındaki **İş Ortağı Merkezi** Geliştirici Ayarları'nda) kullanılabilir.  |

> [!NOTE]
> IRS vergi formlarında kullanmakta olduğu adres, ödeme hesabınız ve vergi formlarınızı ayar her zaman vergi [profilinizde yer alan adresten gelir.](set-up-your-payout-account.md) Adresiniz değişti ise, Vergi profilinizde adresi **güncelleştirin.**

Vergi formları aşağıdaki adreslerden size gönderilir:

**ABD Vatandaşları:**

| İş Grubu         | Tüzel          | Adres                                          |
|------------------------|-----------------------|--------------------------------------------------|
| Windows, Office, Azure | Microsoft Corporation | One Microsoft Way<br>Redmond, WA 98052 USA       |
| Reklam            | Microsoft Online Inc. | 6880 Sierra Center Parkway<br>Reno, NV 98511 USA |

**ABD dışı vatandaşları:**

| İş grubu         | Yasal varlık          | Adres                                          |
|------------------------|-----------------------|--------------------------------------------------|
| Windows, Office, Azure | Microsoft Irlanda Işlemleri sınırlı (Microsoft, Microsoft Corporation 'ın uygun aracı olarak hareket eden Microsoft Irlanda aracılığıyla ödeme yapılır) | Tek bir Microsoft yeri<br>Güney Ilçe Iş Park<br>Leopardstown, Dublin 18, D18 P521, Irlanda|
| Reklam          | Microsoft Irlanda Işlemleri sınırlı (Microsoft Online Inc. için ödeme, Microsoft Online Inc. aracılığıyla Microsoft Irlanda aracılığıyla yapılır.) | Tek bir Microsoft yeri<br>Güney Ilçesi& Iş Park<br>Leopardstown, Dublin 18, D18 P521, Irlanda |
| Reklam            | Microsoft Online Inc. | 6880 Sierra Center Parkway<br>Reno, NV 98511 USA |

>[!NOTE]
> \* Reklam geliri elde eden şu ülkelerin vatandaşları Microsoft Ireland Operations Limited aracılığıyla ödenmektedir: Almanya, Hollanda, Afrika, Fransa, Almanya, Çekya, Norveç, Finlandiya, Finlandiya, Fransa, Almanya, Norveç, İrlanda, isle of Man, İtalya, Leton, Liechtenstein, Liechtenstein, Litya, İşle, İşla, İşleç, Monaco, Hollanda, Portekiz, Norveç, Güney Afrika, İspanya, İsveç, İsviçre, Birleşik Krallık

## <a name="for-developers-located-in-the-united-states"></a>Birleşik Devletler'de bulunan geliştiriciler için

| Ücretli uygulamalar satan bir Birleşik Devletler geliştiriciyim ve...   | Şu formu alalım: |
|------------------------|-----------------------|
| İlgili vergi **yılında 20.000** ABD dolarının üzerinde olan bu satışların toplam satın alma tutarıyla **200'den** fazla uygulama satışım vardı **(Brezilya** ve Çin'de yapılan satışları Windows 10 üzerinde Microsoft Store.)| **1099-K:**<br/>Filer: Microsoft Corporation<br/>EIN: \* \* \* \* \* 4442<br/><br/>**Önemli:** Form 1099-K, **size yapılan ödemeleri** değil, brüt satın alma tutarlarını içerir.| 
| Brezilya ve Çin'de yapılan (i) uygulama satışları için Market'te yapılan Windows 10 üzerinde Microsoft Store (ii) için en az **10** ABD doları ödeme aldı.<br/><br/>**OR**<br/><br/>İlgili vergi yılında Microsoft'tan uygulama satışları ile ilgili değil en az 600 ABD doları ödeme aldım (örneğin, teşvik ödemeleri veya bir yarışmadan veya promosyondan ödemeler)| **1099-MISC:**<br/>Payer: Microsoft Corporation<br/>EIN: \* \* \* \* \* 4442<br/><br/>**Önemli:** Belirli iş varlıkları, Microsoft'tan alınan ödeme tutarlarından bağımsız olarak 1099 MISC formu almaz.  Daha fazla bilgi için vergi uzmanınıza danışın.| 
| Yukarıdakilerin hiçbiri geçerli değildir.| Yok |
| <br/><br/>**Uygulamalarda reklam satan Birleşik Devletler geliştiriciyim ve...** |<br/><br/>**Şu formu alalım:** |
|İlgili vergi yılında uygulamalarda yer alan reklamlardan en az **600** ABD doları ödeme aldı. | **1099-ÇEŞITLI:**<br/>Ödeyen: Microsoft Online Inc<br/>EIN: \* \* \* \* \* 0505<br/><br/>**Önemli:** Belirli iş varlıkları, Microsoft 'tan alınan ödeme tutarlarından bağımsız olarak 1099-MISC formlar almaz.  Daha fazla bilgi için vergi uzmanınıza başvurun. |
| Geçerli vergi yılında uygulamalardaki reklamları **$600 ' den az ödedim** . | Yok |


## <a name="for-developers-located-outside-of-the-united-states"></a>Birleşik Devletler dışında bulunan geliştiriciler için


| **Soru** | **Yanıt** |
|---|---|
| **Microsoft 'tan 1042-S biçimi aldım. Ne için?** | Microsoft, Birleşik Devletler vergi dairelerine raporlanabilir olarak kabul edilen ve stopaj vergisine tabi olan gelirinizi ödediğimiz için size bir 1042-S formu veya formu sağladı.  Bu raporlama gereksinimi için 1042-S biçimi kullanılır. | 
| **Formlarla ne yapmam gerekir?** | Genellikle, sizin bölüminizdeki belirli bir eylem gerekli değildir. Her türlü vergi kredisi için yerel vergi dairelerine uygulamak istiyorsanız, 1042-S formu sizin için yararlı olabilir.  Bu konuyla ilgili daha fazla bilgi edinmek için kendi vergi danışmanlarınızı inceleyin. | 
| **W8 formunu tamamladığımda, ödemem neden ücretlendirildim?** | Vergiler, aşağıdakilerden biri olursa, şu durumlarda stopaj uygulanır:<br/><br/>1. w8 'in vergi treatıon bölümünü doğru bir şekilde tamamlamadınız veya <br/>2. Birleşik Devletler bir vergi treaine sahip olmayan bir ülkede yerleşik olursunuz.<br/><br/>Güncelleştirilmiş bir w8 formu göndermek için herhangi bir zamanda Iş Ortağı Merkezi ' ni ziyaret edebilirsiniz.<br/><br/> **Note:** Tüm gelir vergi stopaja tabi değildir. | 
| **Geçerli bilgilerle güncelleştirilmiş bir W8 formu gönderildi. Microsoft, yardımdan muaf olan vergiyi iade ediyor mu?** | Vergiler geri alındıktan sonra para iadesi alınamaz. Vergi danışmanlarınıza başvurarak bu vergiler için yerel bir kredi talep edip edilip ediley olmadığı veya IRS'den para iadesi alınıp alınamayyıp alınamayyışlarını tartışarak. | 
| **1042-S formunda hangi satışlar raporlandı?** | Yalnızca vergi **stopajı olarak sınıflandırılan Birleşik Devletler** alıcılara yapılan satışlar raporlanabilir.  Diğer tüm satışlar raporlanabilir olarak kabul edilemez. | 
| **Neden aynı zarfta 1042-S formunun üç kopyasını aldım?** | IRS düzenlemeleri, formun üç kopyasının sağlanmalıdır:<br/><br/>- Alıcının kayıtları için bir tane<br/>- Federal vergi iadesini Birleşik Devletler (varsa) için bir dosyalama<br/>- Bir eyalet Birleşik Devletler (varsa) ile dosyalama için |

> [!NOTE]
> **IRS** vergi formlarına ilişkin ek sorularınız veya endişeleriniz varsa, IRS panosunda [Yardım](https://partner.microsoft.com/dashboard/support/) ve destek İş Ortağı Merkezi gidin. Microsoft, belirli vergi koşullarınız ile ilgili soruları yanıtamaz; Bu sorular için lütfen vergi uzmanından öneriler alın.

## <a name="next-steps"></a>Sonraki adımlar

- [Ticari markette ödeme alma](marketplace-get-paid.md)
