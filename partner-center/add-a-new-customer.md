---
title: Yeni müşteri kaydı ekleme
ms.topic: how-to
ms.date: 09/07/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: İş Ortağı Merkezi'da yeni müşteri kaydı İş Ortağı Merkezi. Ardından müşteri aboneliklerini satıp faturalamayı yönetebilir veya müşteri desteği sebilirsiniz.
author: parthp
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 7995ee8f4da20d80fd260bcb77665e244e448227
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960195"
---
# <a name="how-to-add-a-new-customer-record-in-partner-center"></a>İş Ortağı Merkezi'de yeni müşteri kaydı ekleme

**Uygun roller:** Genel yönetici | Kullanıcı yönetimi yönetici | Yönetici aracısı | Satış aracısı

Bu makalede, yeni bir müşterinin İş Ortağı Merkezi. Abonelikleri satmadan, faturalamayı yönetemeden veya müşteriye destek sağlaymadan önce bu adımlar gereklidir.

## <a name="considerations"></a>Dikkat edilmesi gerekenler

**Yeni bir müşteri kaydı eklerken İş Ortağı Merkezi:**

- **Doğru kayıt kimliğini kullanın:** Şirket kayıt kimliğinizi girerken, müşterinin kişisel kimliğini değil, iş verginizi kullanın.

- **Bazı ülkeler için ek bilgi girin:** [Doğrudan fatura](#company-registration-id-and-phone-number-required-for-some-countries) iş ortağı veya dolaylı sağlayıcıysanız bazı ülkelerde şirket kayıt kimliği ve telefon numarası gereklidir
- **Onay Microsoft Müşteri Sözleşmesi** onaylayın: Müşteri adına sipariş alamadan önce, müşteri adına sipariş [Microsoft Müşteri Sözleşmesi.](confirm-customer-agreement.md)
- **Mevcut müşteriler  için farklı** adımlar kullanın: Çok kanallı veya Çok Kanallı [](multichannel.md) bir senaryo [](multipartner.md) aracılığıyla İş Ortağı Merkezi müşteri kayıtlarına sahip olan müşteriler de dahil olmak üzere [mevcut](request-a-relationship-with-a-customer.md)müşteriler için, buradaki adımları takip etmek yerine onlarla bir ilişki isteğinde bulundurabilirsiniz.
- **Ayrıntılı, doğru müşteri bilgilerini girin:** Müşteri müşteri doğrulaması için şunların sağ olduğundan emin olun:
  - Resmi belgelerde görünen yasal/resmi adı tam olarak girin.
  - Kısaltmalar veya kısa formlar kullanmaktan kaçının.
  - Test adlarını kullanma.
  - Tam adres bilgilerini (örneğin, konum ayrıntıları, şehir, eyalet, ülke ve posta/posta kodu) girin.

## <a name="new-rules-for-company-name-and-email-address"></a>Şirket adı ve e-posta adresi için yeni kurallar

22 Eylül 2021'den itibaren aşağıdaki yeni doğrulama kuralları geçerli olacaktır.

Bir şirket adı girerken aşağıdakilere izin verilmez:
- Yalnızca bir karakter kullanma.
- Yalnızca $^# gibi özel &kullanın (aşağıdaki [tabloya](#table-of-special-characters) bakın).
- Yalnızca boşlukları ve/veya sekmeleri kullanma.
- LLC, Inc gibi kısıtlı listeden tek başına kısaltmaları kullanma [(aşağıdaki](#table-of-abbreviations) tabloya bakın).
- ".com", ".org", ".edu", ".club" gibi internet Top-Level Etki Alanı (TDL) uzantılarına sahip adlar kullanma [(aşağıdaki](#table-of-top-level-domain-extensions) tabloya bakın).

- Aynı karakterin, 999 gibi başka bir karakterle üç veya daha fazla kez tekrarlanan bir karakter kullanma.

- 1 2 3 gibi tek tek karakterlerle karışık boşluklar ve/veya sekmeler kullanma.

Müşteri e-posta adresi girerken aşağıdakilere izin verilmez:

- E-posta adresi @microsoft.com içermez.
- Müşteri e-posta adresi, iş ortağıyla aynı etki alanı adını içere değildir. Örneğin ABC adlı bir iş ortağı ile müşteri e-postası oluşturamayabilirsiniz. @abc.com

## <a name="to-add-a-new-customer-in-partner-center"></a>İş Ortağı Merkezi'nde yeni müşteri eklemek için

1. Yeni İş Ortağı Merkezi Müşteriler'i **ve** ardından Müşteri **ekle'yi seçin.**
2. Müşteriniz bir eğitim kurumu ise eğitim [müşterisi oluşturma hakkında bilgi için bkz.](sell-to-education-customers.md).

3. Hesap **bilgileri sayfasında** müşterinin ayrıntılarını ve birincil iletişim bilgilerini girin.
   >[!IMPORTANT]
   >İş ortaklarının aşağıdakilere onayları gerekir:
   >
   >Kurumsal bayi seçmeden kuruluşum dolaylı iş ortağı ve Doğrudan İş Ortağı olarak hareket ediyor olduğunu onayluyorum
   >
   >Bu sipariş kapsamında satın alınan ürünleri üst kuruluşuma bağlı olan diğer iş ortaklarına yeniden satışa almamamı onayluyorum

   >[!NOTE]
   >EU/EFTA yasaları, bu ülkelerde işlem yapan iş ortaklarının bir işlem içinde ilişkili ek kurumsal bayileri beyan etmek zorunda olduğunu bildirmektedir. Aşağıdaki kurallar geçerli olur:
   >- Herhangi bir ek kurumsal bayiden önce bir ilk kurumsal bayi seçilmelidir
   >- Ek kurumsal bayiler herhangi bir ek teşvik, teklif vb. haklara sahip olmayacaktır.
   >- Girilen ek satıcı, uygun olduğunda doğru MPN kimliğinin girilmiş olduğundan ve kurumsal bayinin MPA'yı imzalamış olduğundan emin olmak için doğrulanır.
   >- İşlem kapsamında en fazla 5 ek kurumsal bayi girilebilir 

4. Dolaylı sağlayıcıysanız, listeden bu müşterinin abonelikleriyle ilişkilendirmek istediğiniz dolaylı kurumsal bayiyi seçin.

5. Gerekli bilgileri girmeyi bitirdikten sonra **Sonraki: Abonelikler'i seçin.**

6. Abonelikler  sayfasında, müşterinizin satın almak istediği tekliflerini seçin, lisans sayısını girin ve ardından Sonraki: Gözden **Geçir'i seçin.**

7. Gözden Geçir **sayfasında,** girdilerinizi doğruluk için denetleyin ve gönder'i **seçin.**

8. Müşteri bilgilerini eklemeyi bitirdikten ve gerekli abonelikleri satın aldığınız zaman Bitti'yi **seçin.**

## <a name="company-registration-id-and-phone-number-required-for-some-countries"></a>Bazı ülkeler için gereken şirket kayıt kimliği ve telefon numarası

Aşağıdaki ülkelerdeki müşteriler için kayıt ekleyen doğrudan fatura iş ortakları ve dolaylı sağlayıcılar da şirket telefon numarasını ve kayıt kimliğini (kuruluş INN'si olarak da bilinir) girmeli:

Afrika, Afrika, Brezilya, Brezilya, Hindistan, Güney Afrika, Kırgızlar, Afrika, Vietnam, Myanmar, Arak, Rusya, Suudi Arabistan, Güney Afrika, Güney Sudan, Tajikistan, Arjantin, Rusya, Afrika, Birleşik Birleşik Arab Vezni, Özbekistan, Vietnam ve Vietnam

## <a name="company-name-and-email-characters-abbreviations-and-extensions"></a>Şirket adı ve e-posta karakterleri, kısaltmalar ve uzantılar

Aşağıdaki tablolarda, yukarıdaki yeni kurallar bölümünde [belirtilen öğeler](#new-rules-for-company-name-and-email-address) listelemektedir.

### <a name="table-of-special-characters"></a>Özel karakter tablosu

| Karakter. | Karakter. | Karakter. | Karakter. |
| ----- | ----- | -----| ----- |
| '~' | '-' |  '=' |  '_' |
|  '#' | '.' |  '%' |  '-' |
|  '+' |  ':' |  '^' |  '[' |
|  '$' |  '–' |  '&' |  ']' |
|  '@' |  '—' |  '*' |  '(' |
|  ',' |  ')' |  '”' |  '⟩' |
|  '`' |  '<' |  '!' |  '\\' |
|  '(' |  '>' |  '“' |  '/' |
|  ')' |  '{' |  '‘' |  '\|' |
|  '\' |  '}' |  '،' |  ':' |
|  ';' |  '⟨' |  '’' | '?' |
|  '”' |  '⟩' |  '\\' |  |


### <a name="table-of-abbreviations"></a>Kısaltma tablosu

| Abbr. | Abbr. | Abbr. | Abbr. |
| ----- | ----- | ----- | ----- |
|" c p a" | "pty" | "l. l. c." | "gmbh" |
| "c.p.a." | "pty ltd" | "l.l.c." | "olarak" |
| "l.l.p." | "pte ltd" | " l l p" | "wll" |
| "c. p. a." | "private limited" | "corp" | "lda" |
| "l. l. p." | "pvt" | "corporation" | "sarl" |
| " l l c" | "pvt ltd" | "inc" | "kft" |
| "corp." | "zrt" | "incorporated" | "ltd" |
| "llc." | "ooo" | "sınırlı" | "ltd." |
| "llp." | "llp" | "llc" | "sdn zamand"

### <a name="table-of-top-level-domain-extensions"></a>En üst düzey etki alanı uzantıları tablosu

| Dahili.  | Dahili.  | Dahili.  | Dahili. |
| ----- | ----- | ----- | ----- |
| .ac | .ba | .ca | .de |
| .ad | .bb | .cc | .dj |
| .ae | .bd | Cd | .dk |
| .af | .be | .cf | .dm |
| .ag | .bf | .cg | .do |
| Ai | .bg | .ch | .dz |
| .al | .fare | .ci | .fm |
| .am | .bi | .ck | .fo |
| .an | .kanallar | .cl | Fr |
| .ao | .bl | .cm | .ga |
| .aq | .bm | .cn | .gb |
| .ar | .bn | .co | .gd |
| .as | .bo | .cr | Ge |
| .at | .bq | .cu | .gf |
| Au | .br | .cv | .gg |
| .aw | .bs | .cw | .gh |
| .ax | .bt | .cx | .gi |
| .az | .bv | .cy | .gl |
| .ec | .bw | .cz | .gm |
| .ee | .by | .eu | .gn |
| .örn. | .bz | .fi | .gp |
| .eh | Es | .fj | .gq |
| .er | .et | .fk | .gr |
| .gs | .gw | .hm | .ht |
| .gt | .skop | .hn | .hu |
| .gu | .hk | Hr | .id |
| .ie | .kz | .mo | .nz |
| .il | .la | .mp | .om |
| .im | .lb | .mq | .pa |
| .in | .lc | .mr | .pe |
| .io | .li | .ms | .pf |
| .iq | .lk | .mt | .pg |
| .ir | .lr | .mu | .ph |
| .is | .ls | .mv | .pk |
| .it | .lt | .mw | .pl |
| .je | .lu | .mx | .pm |
| .jm | .lv | .my | .pn |
| .jo | .ly | .mz | .pr |
| .jp | .ma | .na | Ps |
| .ke | .mc | .nc | .pt |
| .kg | .md | .ne | .pw |
| .km | .me | .nf | .py |
| .ki | .mf | .ng | .qa |
| .km | .mg | .ni | .re |
| .kn | .mh | Nl | .ro |
| .kp | .mk | .no | .rs |
| .kr | .ml | .np | Ru |
| .wan | .mm | .nr | .rw |
| .ky | .mn | .nu | .sa |
| .sb | .tf | .vc | .中国 |
| .sc | .tg | .ve | .中國 |
| .sd | Th | .vg | .భారత్ |
| .se | .tj | .vi | .ලංකා |
| .sg | .tk | .vn | .ભારત |
| .sh | .tl | .vu | .भारतम् |
| .si | .tm | .wf | .भारत |
| .sj | .tn | .ws | .भारोत |
| .sk | .to | .ಭಾರತ | .укр |
| .sl | .tp | .한국 | .香港 |
| .sm | .tr | .ଭାରତ | .台湾 |
| .sn | Tt | .ভাৰত | .台灣 |
| .so | .tv | .ভারত | .мон |
| .sr | .tw | .சிங்கப்பூர் | .tc |
| .ss | .tz | .sz | .td |
| .st | .ua | .বাংলা | .uz |
| .su | .ug | .қаз | .va |
| .sv | .uk | .срб | .мкд |
| .sx | .um | .бг | .ею |
| .sy | .us | .бел | Uslu |
| .tc | .uz | .мкд |  |

## <a name="next-steps"></a>Sonraki adımlar

- Bulut Çözümü Sağlayıcısı programı aracılığıyla müşterilere ne satabilirsiniz hakkında daha fazla bilgi için bkz. [Bulut Çözümü Sağlayıcısı programı](csp-offers.md)
