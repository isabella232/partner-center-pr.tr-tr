---
title: Microsoft tarafından verilen IRS vergi formlarını anlama
description: Microsoft tarafından verilen ve ne zaman kullanılabilir hale getirildikleri dahil olmak üzere vergi formları hakkında bilgi edinin.
ms.topic: article
author: mingshen-ms
ms.author: mingshen
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.localizationpriority: medium
ms.date: 09/30/2020
ms.openlocfilehash: 42c5d6f0d31e6509253fe44d5b97606fc688f177
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712826"
---
# <a name="understand-irs-tax-forms-issued-by-microsoft"></a>Microsoft tarafından verilen IRS vergi formlarını anlama

Her yıl Microsoft 'tan bir veya daha fazla vergi formu alabilirsiniz. Bu, konumunuza ve aldığınız satış veya ödeme miktarına bağlıdır. Microsoft 'un bu formları vermesi ve bunları dahili gelir hizmeti (ıRS) ile dosyaları için yapması gerekir.

Bu makalede, bu formlar hakkında daha fazla bilgi sağlanır.

## <a name="types-of-tax-forms"></a>Vergi formları türleri

| IRS vergi formu | Description | Kullanılabilirlik |
|--------------|-------------|--------------|
|1099-ÇEŞITLI, 1099-K | Microsoft 'un Market konumlarına katılım için size yapılan satış etkinliklerine ve/veya ödemeleriyle ilgili | Yazdırılan formlar, **31 Ocak** tarihinde veya daha önce işaretlenir ve. PDF kopyaları, [iş ortağı merkezi](https://partner.microsoft.com/dashboard) 'nde ( **ödeyen ve vergi > ödeme** kapsamındaki **iş ortağı merkezi hesap ayarları** 'nda) aynı anda kullanılabilir olacaktır |
|1042-S | Birleşik Devletler stopaj vergisine tabi olan ve size yapılan ödemeler ile ilgili | Yazdırılan formlar, **15 Mart** tarihinde veya daha önce işaretlenir ve. PDF kopyaları Iş Ortağı Merkezi 'Nde ( **ödeyen ve vergi > ödeme** kapsamındaki **iş ortağı Merkezi geliştirici ayarları** ) aynı anda kullanılabilir olacaktır  |

> [!NOTE]
> IRS vergi formlarında kullandığımız adres, [ödeme hesabınızı ve vergi formlarınızı ayarlarken](set-up-your-payout-account.md)vergi profilinizdeki adresten gelir. Adresiniz değiştiyse, **vergi profilinizde** adresi güncelleştirdiğinizden emin olun.

Vergi formları şu adreslerden size gönderilecektir:

**ABD vatandaşları:**

| İş grubu         | Yasal varlık          | Adres                                          |
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
> \* Aşağıdaki ülkelerin vatandaşları, reklam gelirini elde eden, Microsoft Irlanda Işlemleri sınırlı olarak ücretlendirilir: Avusturya, Belçika, Bulgaristan, Hırvatistan, Kıbrıs, Czechia, Danimarka, Estonya, Finlandiya, Fransa, Almanya, Yunanistan, Macaristan, Irlanda, Güney ABD, Italya,, Liechtenstein, Litvanya, Liechtenstein, Litvanya, Lüksemburg, Malta, Monako, Hollanda, Norveç, Polonya, Portekiz, Romanya, Yunanistan, Slovenya, Güney Afrika, Ispanya, Isveç, Isviçre, Birleşik Krallık

## <a name="for-developers-located-in-the-united-states"></a>Birleşik Devletler bulunan geliştiriciler için

| Ücretli uygulamalar satan Birleşik Devletler geliştirici ve...   | Şu formu almam gerekir: |
|------------------------|-----------------------|
| Geçerli vergi yılında **200** **ABD Doları $20.000 'den** büyük bir toplam satın alma miktarı (Windows 10 ' da Microsoft Store ile Brezilya ve Çin 'de yapılan satışları **saymıyor** .)| **1099-K:**<br/>Filer: Microsoft Corporation<br/>EIN: \* \* \* \* \* 4442<br/><br/>**Önemli:** Form 1099-K, size yapılan ödemeleri değil, **Brüt satın alma** tutarlarını içerir.| 
| Minecrampamarket 'teki Windows 10 veya (II) satışları Microsoft Store, Brezilya ve Çin 'de gerçekleştirilen, (i) uygulama satışları için **en az $10 ödedim** .<br/><br/>**OR**<br/><br/>İlgili vergi yılında Microsoft 'un uygulama satışlarına yönelik olarak en az $600 ödedim (örneğin, bir yarışmaya veya promosyondan ödemeleri veya ödemeleri teşvik edin)| **1099-ÇEŞITLI:**<br/>Ödeyen: Microsoft Corporation<br/>EIN: \* \* \* \* \* 4442<br/><br/>**Önemli:** Belirli iş varlıkları, Microsoft 'tan alınan ödeme tutarlarından bağımsız olarak 1099-MISC formlar almaz.  Daha fazla bilgi için vergi uzmanınıza başvurun.| 
| Yukarıdakilerin hiçbiri uygulanmaz.| Yok |
| <br/><br/>**Uygulamalarım, uygulamalar ve... için reklamları satan Birleşik Devletler geliştirici.** |<br/><br/>**Şu formu almam gerekir:** |
|Geçerli vergi yılında uygulamalarda reklamları **en az $600 oranında** aldım. | **1099-ÇEŞITLI:**<br/>Ödeyen: Microsoft Online Inc<br/>EIN: \* \* \* \* \* 0505<br/><br/>**Önemli:** Belirli iş varlıkları, Microsoft 'tan alınan ödeme tutarlarından bağımsız olarak 1099-MISC formlar almaz.  Daha fazla bilgi için vergi uzmanınıza başvurun. |
| Geçerli vergi yılında uygulamalardaki reklamları **$600 ' den az ödedim** . | Yok |


## <a name="for-developers-located-outside-of-the-united-states"></a>Birleşik Devletler dışında bulunan geliştiriciler için


| **Soru** | **Yanıt** |
|---|---|
| **Microsoft 'tan 1042-S biçimi aldım. Ne için?** | Microsoft, Birleşik Devletler vergi dairelerine raporlanabilir olarak kabul edilen ve stopaj vergisine tabi olan gelirinizi ödediğimiz için size bir 1042-S formu veya formu sağladı.  Bu raporlama gereksinimi için 1042-S biçimi kullanılır. | 
| **Formlarla ne yapmam gerekir?** | Genellikle, sizin bölüminizdeki belirli bir eylem gerekli değildir. Her türlü vergi kredisi için yerel vergi dairelerine uygulamak istiyorsanız, 1042-S formu sizin için yararlı olabilir.  Bu konuyla ilgili daha fazla bilgi edinmek için kendi vergi danışmanlarınızı inceleyin. | 
| **W8 formunu tamamladığımda, ödemem neden ücretlendirildim?** | Vergiler, aşağıdakilerden biri olursa, şu durumlarda stopaj uygulanır:<br/><br/>1. w8 'in vergi treatıon bölümünü doğru bir şekilde tamamlamadınız veya <br/>2. Birleşik Devletler bir vergi treaine sahip olmayan bir ülkede yerleşik olursunuz.<br/><br/>Güncelleştirilmiş bir w8 formu göndermek için herhangi bir zamanda Iş Ortağı Merkezi ' ni ziyaret edebilirsiniz.<br/><br/> **Note:** Tüm gelir vergi stopaja tabi değildir. | 
| **Geçerli anlaşma bilgileriyle güncelleştirilmiş bir w8 formu gönderdim. Microsoft, kesilen vergiyi iade edebilir mi?** | Vergi stopajdıktan sonra iade edilemez. Bu vergiler için yerel kredi talep edebilir veya ıRS 'den bir para iadesi arayabilir olup olmayacağını tartışmak için vergi danışmanlarınız ile iletişim kurun. | 
| **1042-S formunda hangi satışlar raporlanır?** | Yalnızca **Vergi stopajı 'na tabi olarak sınıflandırılan Birleşik Devletler bulunan alıcıların** satışları raporlanabilir hale getirilir.  Diğer tüm satışlar raporlanabilir olarak kabul edilmez. | 
| **Neden tek bir zarfa ait 1042-S formunun üç kopyasını aldım?** | IRS düzenlemeleri için formun üç kopyasının sağlanması gerekir:<br/><br/>-Alıcı kayıtları için bir tane<br/>-Bir Birleşik Devletler federal vergi iadesi (varsa)<br/>-Bir Birleşik Devletler durum vergisi dönüşü (varsa) |

> [!NOTE]
> **IRS vergi formlarıyla** ilgili ek sorularınız veya endişeleriniz varsa, Iş Ortağı Merkezi panosunda [Yardım ve destek](https://partner.microsoft.com/dashboard/support/) bölümüne gidin. Microsoft, belirli vergi şartlarınızla ilgili soruları yanıtlayamıyor; Bu sorular için lütfen vergi uzmanınızdan gelen önerileri arayın.

## <a name="next-steps"></a>Sonraki adımlar

- [Ticari markette ödeme alma](marketplace-get-paid.md)
