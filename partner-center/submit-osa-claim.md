---
title: Müşteri ilişkilendirmesi oluşturma
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Kayıt (CPOR) modelinin talep ortağı ile müşteri ilişkilendirmeleri oluşturun. Microsoft 365 & Dynamics 365 müşterileri için sales, usage, teşvikleri yönetimine yardımcı olur.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 87c2fc9b9d835b7dfcfbe8736e82d3862409c124
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129073577"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a>Microsoft 365 ve Dynamics 365 için istenen kayıt ortağı (cpor) modeli aracılığıyla müşteri ilişkilendirmeleri


**Uygun roller**: teşvikleri admin

Microsoft, 1 ekim 2019 ' de, sahip olduğunuz ilişkileri yönetmek için kayıt ortağı iş ortağı (cpor) modelini kullanarak, çevrimiçi hizmetler danışmanlığı (OSA) satışı, çevrimiçi hizmetler kullanımı (OSU)-Microsoft 365 ve OSU-Business Application teşvikleri ile ilgili 365 Microsoft 365.

>[!Important]
> müşteri birliği (cpor) talepleri yalnızca çevrimiçi hizmetler danışma belgesi (OSA) satışı, çevrimiçi hizmetler kullanımı (OSU)-Microsoft 365 ve OSU-Business uygulama teşvik programları için geçerlidir. Bulut Çözümü Sağlayıcısı (CSP), yönetilen satıcı, barındırma veya yüzey gibi başka bir program için bir ortak op talebi gönderiyorsanız, lütfen burada özetlenen ortak op talep işlemine bakın. <br><br>Talep gönderdiğinizde, Microsoft onu doğrular. Bu noktada daha fazla bilgi isteyeceğiz. İlişki isteğinizin müşterisini de bilgilendireceğiz. Müşterilerin kabul etmek için beş iş günü vardır. Devre dışı kalmazsanız, bu belirli kiracı ve iş yüküyle olan ilişkilendirmeniz resmi olur. Bu noktada müşterinin kullanım verilerine erişebilirsiniz. 

Bir talebi tamamlayabilmeniz için aşağıdaki bilgilere ihtiyacınız vardır:

- Talebi yapan varlığınızın **MPN kimliği** (Microsoft iş ortağı ağı kimliği)

- Müşterinin **etki alanı adı** (daha fazla bilgi için bkz. [Kiracı kimliğini bulma, etki alanı adı, Kullanıcı nesne kimliği](find-ids-and-domain-names.md))

- Müşterinin **DIZIN kimliği** veya **Kiracı kimliği** (daha fazla bilgi IÇIN bkz. [Kiracı kimliğini bulma, etki alanı adı, Kullanıcı nesne kimliği](find-ids-and-domain-names.md))

- Business Applications veya Microsoft 365 gibi **çözüm alanı**

- Gerçekleştirdiğiniz **etkinlik** ve satış öncesi, kullanım veya gelir ilişkisi gibi yapmak istediğiniz talep türü

- Müşterinizin **kişi adı**, başlığı ve e-posta adresi

- Dynamics 365 için Ayrıca müşterinizin **teknik iletişim** adı, başlığı ve e-posta adresini sağlamanız gerekir

- Kendi şirketinizin **kişi adı** ve e-posta adresi

- Bu talep için bir **ad** oluşturacaksınız

- Seçtiğiniz **ürün (ler)** veya iş yükleri

- Müşteri tarafından imzalanan iş beyanı gibi **yürütme kanıtı (PoE)**. Ayrıca, kullanmak üzere bir PoE şablonu indirebilirsiniz.

- İş ortakları yalnızca gelir ilişkilendirmesini talep etmek için: **Dynamics çözüm satıcı adı**, **MÜŞTERI adı** ve **ISV ürün/çözüm adı**. 

Ayrıca aşağıdaki noktaları da anlamanız gerekir:

- Microsoft 365 müşterileriniz varsa, bu işlemi kullanarak OSU teşvikleri kazanmanıza devam etmek istediğinizden sonra yeniden ilişkilendirmeniz gerekir.

- Dynamics 365 veya Power BI müşterilerle mevcut ilişkilendirmeleriniz varsa, bu ilişkilendirmeler aboneliklerinin süresi dolmadan geçerli olmaya devam eder.

- Müşterinin birden çok iş ortağı olabilir, ancak her iş yükü (OSU-Microsoft 365 için) veya abonelik (OSA-Sell ve OSU-Business uygulamalar için) yalnızca bir ortağıyla ilişkilendirilebilir.

## <a name="create-a-customer-association"></a>Müşteri ilişkilendirmesi oluşturma

> [!NOTE]
> Iş Ortağı Merkezi önizleme arabirimi, mantıksal olarak gruplanmış çalışma alanları aracılığıyla daha verimli ve üretken bir kullanıcı deneyimi sağlar. Çalışma alanları arabirimi ve nasıl kullanılacağı hakkında daha fazla bilgi edinmek için bkz. [Iş ortağı merkezini alma](get-around-partner-center.md#turn-workspaces-on-and-off).

#### <a name="workspaces-view"></a>[Çalışma alanları görünümü](#tab/workspaces-view)

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. **Teşvikleri** kutucuğunu seçin ve ardından **Müşteri ilişkilendirmeleri**' ni seçin.

3. Müşteri ilişkilendirmeleri sayfasının en üstünde **+ müşteri ilişkisi**' nı seçin.

4. Müşteriyle ilişkilendirilecek iş ortağı konumunun **MPN kimliğini** seçip müşterinin etki alanı adını ve dizin kimliğini ekleyin. [Bunu bulun](find-ids-and-domain-names.md)

5. **Devam**’ı seçin.

6. **Çözüm alanını** ve **etkinliği** seçin. 

   > [!NOTE]
   > Business Applications ' yi seçerseniz, **kullanım ve/veya satış öncesi** ya da **gelir ilişkilendirmesini** seçin ve ardından **devam**' ı seçin.
   >
   > Gelir ilişkilendirmesini seçerseniz aşağıda listelenenlerden biraz farklı bilgiler istenir.

7. **Müşteri ilişkilendir** sayfasında uygun bilgileri girin ve **Talep Oluştur**' u seçin.

8. Bu müşteri ilişkisiyle ilişkili ürünleri seçin ve ardından **devam**' ı seçin.

9. Müşterinin ve şirketinizin iletişim bilgilerini girin. Tüm alanlar zorunludur. 

   > [!NOTE]
   > Ürününüz Dynamics 365 ise ve seçtiğiniz üründe bu müşteri için birden çok abonelik varsa, abonelik KIMLIĞINI de girmeniz gerekir.

10. PoE bilgilerinizi sağlayın. Bunu kutuya sürükleyebilir, kendi destekleyici belgelerinize göz atabilir veya **Şablonu indir**'i seçerek bir şablon kullanabilirsiniz. 

11. İsteğe bağlı olarak açıklama ekleyip kaydedin ve ardından **Talebi gönder**'i seçin. Müşteriye, müşteri ilişkilendirmenizi onaylamanızı isteyen bir e-posta göndereceğiz.

   > [!NOTE]
   > Müşteri ilişkilendirmesini gönderdikten sonra düzenleyemezsiniz.

Müşteri ilişkilendirmenizin durumu, **Durum** alanında görüntülenir.

Bir müşteri ilişkilendirmesinin geçmişini görüntülemek için **Geçmiş**'i seçin.

#### <a name="current-view"></a>[Geçerli görünüm](#tab/current-view)

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. **Teşvikleri** sekmesini seçin, **genel bakış**' ı seçin ve ardından **Müşteri ilişkilendirmeleri**' ni seçin.

3. Müşteri ilişkilendirmeleri sayfasının en üstünde **+ müşteri ilişkisi**' nı seçin.

4. Müşteriyle ilişkilendirilecek iş ortağı konumunun **MPN kimliğini** seçip müşterinin etki alanı adını ve dizin kimliğini ekleyin. [Bunu bulun](find-ids-and-domain-names.md)

5. **Devam**’ı seçin.

6. **Çözüm alanını** ve **etkinliği** seçin.

   > [!NOTE]
   > Business Applications ' yi seçerseniz, **kullanım ve/veya satış öncesi** ya da **gelir ilişkilendirmesini** seçin ve ardından **devam**' ı seçin.
   >
   > Gelir ilişkilendirmesini seçerseniz aşağıda listelenenlerden biraz farklı bilgiler istenir.

7. **Müşteri ilişkilendir** sayfasında uygun bilgileri girin ve **Talep Oluştur**' u seçin.

8. Bu müşteri ilişkisiyle ilişkili ürünleri seçin ve ardından **devam**' ı seçin.

9. Müşterinin ve şirketinizin iletişim bilgilerini girin. Tüm alanlar zorunludur. 

   > [!NOTE]
   > Ürününüz Dynamics 365 ise ve seçtiğiniz üründe bu müşteri için birden çok abonelik varsa, abonelik KIMLIĞINI de girmeniz gerekir.

10. PoE bilgilerinizi sağlayın. Bunu kutuya sürükleyebilir, kendi destekleyici belgelerinize göz atabilir veya **Şablonu indir**'i seçerek bir şablon kullanabilirsiniz. 

11. İsteğe bağlı olarak açıklama ekleyip kaydedin ve ardından **Talebi gönder**'i seçin. Müşteriye, müşteri ilişkilendirmenizi onaylamanızı isteyen bir e-posta göndereceğiz.

   > [!NOTE]
   > Müşteri ilişkilendirmesini gönderdikten sonra düzenleyemezsiniz.

Müşteri ilişkilendirmenizin durumu, **Durum** alanında görüntülenir.

Bir müşteri ilişkilendirmesinin geçmişini görüntülemek için **Geçmiş**'i seçin.

* * *

## <a name="next-steps"></a>Sonraki adımlar

- [Müşteri ilişkilendirmelerini yönetme](incentives-manage-customer-associations.md)