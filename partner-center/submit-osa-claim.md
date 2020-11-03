---
title: Müşteri ilişkilendirmesi oluşturma
ms.topic: article
ms.date: 09/11/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Kayıt (CPOR) modelinin talep ortağı ile müşteri ilişkilendirmeleri oluşturun. Microsoft 365 & Dynamics 365 müşterileri için Sales, Usage, teşvikleri yönetimine yardımcı olur.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e34698b51a159445f4354e366f79f510533e6f30
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92531999"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a>Microsoft 365 ve Dynamics 365 için Istenen kayıt ortağı (CPOR) modeli aracılığıyla müşteri ilişkilendirmeleri

**Uygulama hedefi**

- İş Ortağı Merkezi

**Uygun roller:**

- Teşvikleri Yöneticisi

Microsoft, 1 Ekim 2019 ' de, Microsoft 365 sahip olduğunuz ilişkileri yönetmek için kayıt ortağı (CPOR) modelini kullanmaya başlamıştır 365 ve bu, çevrimiçi hizmetler danışmanlığı (OSA) satışı, çevrimiçi hizmetler kullanımı (OSU)-Microsoft 365 ve OSU-Business Application teşvikleri.

>[!Important]
> Müşteri Birliği (CPOR) talepleri yalnızca çevrimiçi hizmetler Danışma belgesi (OSA) satışı, çevrimiçi hizmetler kullanımı (OSU)-Microsoft 365 ve OSU-Business uygulama teşvik programları için geçerlidir. Bulut çözümü sağlayıcısı, yönetilen satıcı, barındırma veya yüzey gibi başka bir program için bir ortak op talebi gönderiyorsanız, lütfen burada özetlenen ortak op talep işlemine bakın. <br><br>Talep gönderdiğinizde, Microsoft onu doğrular. Bu noktada daha fazla bilgi isteyeceğiz. İlişki isteğinizin müşterisini de bilgilendireceğiz. Müşterilerin kabul etmek için beş iş günü vardır. Devre dışı kalmazsanız, bu belirli kiracı ve iş yüküyle olan ilişkilendirmeniz resmi olur. Bu noktada müşterinin kullanım verilerine erişebilirsiniz. 

Bir talebi tamamlayabilmeniz için aşağıdaki bilgilere ihtiyacınız vardır:

- Varlığınızın, talebi yapan **MPN kimliği**

- Müşterinin **etki alanı adı** [bunu bulun](find-domain-name.md)

- Müşterinin **DIZIN kimliği** veya **Kiracı kimliği** şunu [bulun](find-domain-name.md)

- Business Applications veya Microsoft 365 gibi **çözüm alanı**

- Gerçekleştirdiğiniz **etkinlik** ve satış öncesi, kullanım veya gelir ilişkisi gibi yapmak istediğiniz talep türü

- Müşterinizin **kişi adı** , başlığı ve e-posta adresi

- Dynamics 365 için Ayrıca müşterinizin **teknik iletişim** adı, başlığı ve e-posta adresini sağlamanız gerekir

- Kendi şirketinizin **kişi adı** ve e-posta adresi

- Bu talep için bir **ad** oluşturacaksınız

- Seçtiğiniz **ürün (ler)** veya iş yükleri

- Müşteri tarafından imzalanan iş beyanı gibi **yürütme kanıtı (PoE)** . Ayrıca, kullanmak üzere bir PoE şablonu indirebilirsiniz.

- İş ortakları yalnızca gelir ilişkilendirmesini talep etmek için: **Dynamics çözüm satıcı adı** , **MÜŞTERI adı** ve **ISV ürün/çözüm adı** . 

Ayrıca aşağıdaki noktaları da anlamanız gerekir:

- Mevcut Microsoft 365 müşterileriniz varsa, bu işlemi kullanarak OSU teşvikleri kazanmak için devam etmek istediğinize yeniden ilişkilendirmeniz gerekir.

- Dynamics 365 veya Power BI müşterilerle mevcut ilişkilendirmeleriniz varsa, bu ilişkilendirmeler aboneliklerinin süresi dolmadan geçerli olmaya devam eder.

- Müşterinin birden çok iş ortağı olabilir, ancak her iş yükü (OSU-Microsoft 365 için) veya abonelik (OSA-Sell ve OSU-Business uygulamalar için) yalnızca bir ortağıyla ilişkilendirilebilir.

## <a name="create-a-customer-association"></a>Müşteri ilişkilendirmesi oluşturma

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. **Teşvikleri** sekmesini seçin, **genel bakış** ' ı seçin ve ardından **Müşteri ilişkilendirmeleri** ' ni seçin.

3. Müşteri ilişkilendirmeleri sayfasının en üstünde **+ müşteri ilişkisi** ' nı seçin.

4. Müşteriyle ilişkilendirilecek iş ortağı konumunun **MPN kimliğini** seçip müşterinin etki alanı adını ve dizin kimliğini ekleyin. [Bunu bulun](find-domain-name.md)

5. **Devam** ’ı seçin.

6. **Çözüm alanını** ve **etkinliği** seçin. 

   >[!Note]
   >
   >Business Applications ' yi seçerseniz, **kullanım ve/veya satış öncesi** ya da **gelir ilişkilendirmesini** seçin ve ardından **devam** ' ı seçin. 
   <br><br>Gelir ilişkilendirmesini seçerseniz aşağıda listelenenlerden biraz farklı bilgiler istenir.

7. **Müşteri ilişkilendir** sayfasında uygun bilgileri girin ve **Talep Oluştur** ' u seçin.

8. Bu müşteri ilişkisiyle ilişkili ürünleri seçin ve ardından **devam** ' ı seçin.

9. Müşterinin ve şirketinizin iletişim bilgilerini girin. Tüm alanlar zorunludur. 

   >[!NOTE]
   >Ürününüz Dynamics 365 ise ve seçtiğiniz üründe bu müşteri için birden çok abonelik varsa, abonelik KIMLIĞINI de girmeniz gerekir.

10. Yürütme kanıtı (PoE) sağlayın. Bunu kutuya sürükleyebilir, kendi destekleyici belgelerinize göz atabilir veya **Şablonu indir** 'i seçerek bir şablon kullanabilirsiniz. 

11. İsteğe bağlı olarak açıklama ekleyip kaydedin ve ardından **Talebi gönder** 'i seçin. Müşteriye, müşteri ilişkilendirmenizi onaylamanızı isteyen bir e-posta göndereceğiz.

   >[!NOTE]
   >Müşteri ilişkilendirmesini gönderdikten sonra düzenleyemezsiniz.

Müşteri ilişkilendirmenizin durumu, **Durum** alanında görüntülenir.

Bir müşteri ilişkilendirmesinin geçmişini görüntülemek için **Geçmiş** 'i seçin.

## <a name="next-steps"></a>Sonraki adımlar

- [Müşteri ilişkilendirmelerini yönetme](incentives-manage-customer-associations.md)