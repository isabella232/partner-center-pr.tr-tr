---
title: Müşteri ilişkilendirmesi oluşturma
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Talepte Bulunan Kayıtlı İş Ortağı (CPOR) modeliyle müşteri ilişkilendirmeleri oluşturun. Dynamics 365 müşterileri için satış, Microsoft 365 & ve teşviklerin yönetimine yardımcı olur.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1fdabb88d58e149117c88d39f2d7ad522a177f50
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129088510"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a>Microsoft 365 ve Dynamics 365 için Kayıt İş Ortağı (CPOR) modeli aracılığıyla müşteri ilişkilendirmeleri


**Uygun roller:** Teşvikler yöneticisi

1 Ekim 2019'da Microsoft, Çevrimiçi Hizmetler Danışmanlığı (OSA) Satış, Çevrimiçi Hizmet Kullanımı (OSU)-Microsoft 365 ve OSU-Business Uygulama teşvikleri konusunda Microsoft 365 ve Dynamics 365 müşterilerinizle sahip olduğunuz ilişkilendirmeleri yönetmek için Talepte Bulunan Kayıtlı İş Ortağı (CPOR) modelini kullanmaya başladı.

>[!Important]
> Müşteri İlişkisi (CPOR) talepleri yalnızca Çevrimiçi Hizmetler Danışmanlığı (OSA) Satış, Çevrimiçi Hizmet Kullanımı (OSU)-Microsoft 365 ve OSU-Business Uygulama teşvik programları için geçerlidir. Bulut Çözümü Sağlayıcısı (CSP), Managed Reseller, Hosting veya Surface gibi başka bir program için ortak çalışma talebi göndererek burada özetlenen Ortak çalışma talep süreci'ne bakın. <br><br>Talebinizi gönderdiğinizde Microsoft bunu doğrular. Bu noktada sizden daha fazla bilgi istememiz gerekir. Ayrıca ilişkilendirme isteğinizi müşteriye bildirerek. Müşterilerin geri almak için beş iş günü vardır. Kabul etmezlerse, bu kiracıyla ve iş yüküyle olan ilişkilendirmeniz resmi olur. Bu noktada müşterinin kullanım verilerine erişebilirsiniz. 

Talebi tamamlamak için aşağıdaki bilgilere ihtiyacınız olacak:

- Talebi **yapan varlığınız** için MPN kimliği (Microsoft İş Ortağı Ağı kimliği)

- Müşterinin etki alanı **adı (daha** fazla bilgi için bkz. [Kiracı kimliğini, etki alanı adını, kullanıcı nesne kimliğini bulma)](find-ids-and-domain-names.md)

- Müşterinin Dizin **Kimliği veya Kiracı** Kimliği **(daha** fazla bilgi için bkz. [Kiracı kimliğini, etki alanı adını, kullanıcı nesne kimliğini bulma)](find-ids-and-domain-names.md)

- Çözüm **alanı**, örneğin Business Applications veya Microsoft 365

- **Gerçekleştirilen** Etkinlik ve satış öncesi, Kullanım veya Gelir ilişkilendirmesi gibi yapmak istediğiniz talep türü

- Müşterinizin Kişi **adı,** başlığı ve e-posta adresi

- Dynamics 365 için müşterinizin Teknik iletişim  adını, başlığını ve e-posta adresini de sağlayabilirsiniz

- Kendi şirketinizin Kişi **adı ve e-posta** adresi

- Bu talep için **bir Ad** oluştur

- **Talepte bulundurarak** ürün veya iş yükleri

- Müşteri tarafından imzalanan iş bildirimi gibi yürütme kanıtı **(PoE).** Ayrıca kullanmak üzere bir PoE şablonu indirebilirsiniz.

- Yalnızca gelir ilişkilendirmesi talep eden iş ortakları için: **Dynamics çözüm satıcısı adı,** Müşteri **adı** ve **ISV ürününün/çözümünün adı.** 

Ayrıca aşağıdaki noktaları da anlamalısınız:

- Mevcut Microsoft 365 müşteriniz varsa, bu süreci kullanarak OSU teşvikleri kazanmaya devam etmek istediğiniz müşterilerle yeniden ilişkilendirilmeniz gerekir.

- Dynamics 365 veya Power BI mevcut ilişkilendirmeniz varsa, bu ilişkilendirmeler aboneliklerinin süresi sona erinceye kadar geçerli kalır.

- Müşterinin birden çok iş ortağı olabilir, ancak her iş yükü (OSU-Microsoft 365 için) veya abonelik (OSA-Sell ve OSU-Business Uygulamaları için) yalnızca bir iş ortağıyla ilişkilendirilebilir.

## <a name="create-a-customer-association"></a>Müşteri ilişkilendirmesi oluşturma

> [!NOTE]
> Çalışma alanları arabirimi hakkında daha fazla bilgi edinmek için [bkz. İş Ortağı Merkezi.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Çalışma alanları görünümü](#tab/workspaces-view)

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. Teşvikler **kutucuğunu** ve ardından Müşteri **ilişkilendirmeleri'ne tıklayın.**

3. Müşteri ilişkilendirmeleri sayfasının üst kısmında + Müşteri **ilişkilendirme'yi seçin.**

4. Müşteriyle ilişkilendirilecek iş ortağı konumunun **MPN kimliğini** seçip müşterinin etki alanı adını ve dizin kimliğini ekleyin. [Bunu bulun](find-ids-and-domain-names.md)

5. **Devam**’ı seçin.

6. Çözüm alanı **ve Etkinlik'i** **seçin.** 

   > [!NOTE]
   > Uygulama'Business Applications, Kullanım **ve/veya** Satış Öncesi veya Gelir ilişkilendirmesi'ne ve **ardından** Devam'ı **seçin.**
   >
   > Gelir ilişkilendirmesini seçerseniz aşağıda listelenenlerden biraz farklı bilgiler istenir.

7. Müşteriyi ilişkilendirme sayfasında uygun **bilgileri girin** ve Talep oluştur'a **tıklayın.**

8. Bu müşteri ilişkilendirmesi ile ilişkili ürünleri ve ardından Devam'ı **seçin.**

9. Müşterinin ve şirketinizin iletişim bilgilerini girin. Tüm alanlar zorunludur. 

   > [!NOTE]
   > Ürününüz Dynamics 365 ise ve seçtiğiniz ürünün bu müşteri için birden çok aboneliği varsa abonelik kimliğini de girmeniz gerekir.

10. PoE'nizi teminin. Bunu kutuya sürükleyebilir, kendi destekleyici belgelerinize göz atabilir veya **Şablonu indir**'i seçerek bir şablon kullanabilirsiniz. 

11. İsteğe bağlı olarak açıklama ekleyip kaydedin ve ardından **Talebi gönder**'i seçin. Müşteriye, müşteri ilişkilendirmenizi onaylamanızı isteyen bir e-posta göndereceğiz.

   > [!NOTE]
   > Müşteri ilişkilendirmenizi gönderdiniz mi düzenleyemezsiniz.

Müşteri ilişkilendirmenizin durumu, **Durum** alanında görüntülenir.

Bir müşteri ilişkilendirmesinin geçmişini görüntülemek için **Geçmiş**'i seçin.

#### <a name="current-view"></a>[Geçerli görünüm](#tab/current-view)

1. [İş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.

2. Teşvikler **sekmesini, Genel** Bakış'ı **ve** ardından Müşteri **ilişkilendirmeleri'ne tıklayın.**

3. Müşteri ilişkilendirmeleri sayfasının üst kısmında + Müşteri **ilişkilendirme'yi seçin.**

4. Müşteriyle ilişkilendirilecek iş ortağı konumunun **MPN kimliğini** seçip müşterinin etki alanı adını ve dizin kimliğini ekleyin. [Bunu bulun](find-ids-and-domain-names.md)

5. **Devam**’ı seçin.

6. Çözüm alanı **ve Etkinlik'i** **seçin.**

   > [!NOTE]
   > Uygulama'Business Applications, Kullanım **ve/veya** Satış Öncesi veya Gelir ilişkilendirmesi'ne ve **ardından** Devam'ı **seçin.**
   >
   > Gelir ilişkilendirmesini seçerseniz aşağıda listelenenlerden biraz farklı bilgiler istenir.

7. Müşteriyi ilişkilendirme sayfasında uygun **bilgileri girin** ve Talep oluştur'a **tıklayın.**

8. Bu müşteri ilişkilendirmesi ile ilişkili ürünleri ve ardından Devam'ı **seçin.**

9. Müşterinin ve şirketinizin iletişim bilgilerini girin. Tüm alanlar zorunludur. 

   > [!NOTE]
   > Ürününüz Dynamics 365 ise ve seçtiğiniz ürünün bu müşteri için birden çok aboneliği varsa abonelik kimliğini de girmeniz gerekir.

10. PoE'nizi teminin. Bunu kutuya sürükleyebilir, kendi destekleyici belgelerinize göz atabilir veya **Şablonu indir**'i seçerek bir şablon kullanabilirsiniz. 

11. İsteğe bağlı olarak açıklama ekleyip kaydedin ve ardından **Talebi gönder**'i seçin. Müşteriye, müşteri ilişkilendirmenizi onaylamanızı isteyen bir e-posta göndereceğiz.

   > [!NOTE]
   > Müşteri ilişkilendirmenizi gönderdiniz mi düzenleyemezsiniz.

Müşteri ilişkilendirmenizin durumu, **Durum** alanında görüntülenir.

Bir müşteri ilişkilendirmesinin geçmişini görüntülemek için **Geçmiş**'i seçin.

* * *

## <a name="next-steps"></a>Sonraki adımlar

- [Müşteri ilişkilendirmelerini yönetme](incentives-manage-customer-associations.md)