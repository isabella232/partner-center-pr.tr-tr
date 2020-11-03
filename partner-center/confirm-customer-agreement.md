---
title: Müşterinin Microsoft Müşteri Sözleşmesi’ni kabul ettiğini doğrulama
description: Microsoft Müşteri sözleşmesinin müşteri kabulünü onaylama hakkında bilgi edinin. Bulut çözümü sağlayıcısı (CSP) program katılımcılarının, müşteriler için Microsoft ürünlerini ve hizmetlerini sıralamak üzere bu kullanıcılara ihtiyacı vardır.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 05/05/2020
ms.openlocfilehash: 45a34473ff63875af8bd07962ea836661bc948ee
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532111"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-in-the-csp-partner-program"></a>CSP iş ortağı programında Microsoft Müşteri Sözleşmesi 'nin müşteri kabulünü onaylayın

**Uygulama hedefi**

- İş Ortağı Merkezi
- Microsoft 365 Yönetim Merkezi

**Uygun roller**

- Yönetim Aracısı
- Satış Aracısı

Microsoft, 1 Ekim 2019 ' de, Microsoft Bulut sözleşmesinin yerini alacak şekilde CSP programına **Microsoft Müşteri Sözleşmesi** 'ni sunmuştur. Dolaylı satıcılar için ek [rehberlik](indirect-reseller-tasks-in-partner-center.md) okuyun. İş ortaklarının yeni sözleşmeye geçişini kolaylaştırmak için, her iki anlaşma de 31 Ocak 2020 ' e kadar CSP programında birlikte varvardı. 1 Şubat 2020 ' den itibaren, Microsoft Müşteri Sözleşmesi Microsoft Bulut sözleşmesinin üzerinden değiştirilmiştir.

Müşterilerin Microsoft Müşteri anlaşmasını kabul etmek için iki seçeneği vardır. 

**Seçenek 1** : müşteri kabulünü kabul eden iş ortağı kanıtı Iş Ortağı Merkezi API/SDK kullanarak veya Iş Ortağı Merkezi panosu aracılığıyla müşteri kabulünü doğrulayabilirler.

**Seçenek 2** : müşteri doğrudan kabul-iş ortağı, Microsoft 365 Yönetim merkezinde sözleşmeyi gözden geçirmek ve kabul etmek IÇIN bir URL aracılığıyla müşteriyi davet edebilir.

## <a name="access-microsoft-customer-agreement-template"></a>Microsoft müşteri anlaşması şablonuna erişin

Microsoft müşteri anlaşması şablonunun en son sürümünü [buradan](https://aka.ms/customeragreement)el ile indirebilirsiniz. Microsoft Müşteri Sözleşmesi ülkeye özeldir. Microsoft müşteri anlaşması şablonunu istenirken, müşterinin konumuna göre doğru ülkeyi seçtiğinizden emin olun.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Seçenek 1: Iş Ortağı Merkezi 'nde müşteri kabulünü onaylayın

İş ortakları, yeni ve mevcut müşteriler için Iş Ortağı Merkezi 'nde Microsoft Müşteri sözleşmesinin müşteri tarafından kabul edildiğini doğrulayabilirsiniz. Satıcılar, müşterilerinin adına test edemez ve kanıtlama tamamlandı olarak kendi dolaylı sağlayıcısıyla birlikte çalışmalıdır.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Yeni müşteriler için müşteri kabulünü Onayla

Iş Ortağı Merkezi 'nde yeni bir müşteri kiracısı oluşturduğunuzda, müşterinin Microsoft Müşteri sözleşmesinin kabul edildiğini onaylamak için aşağıdaki adımları kullanın. Bu adımları gerçekleştirmek için bir yönetici Aracısı veya satış aracısı olmanız gerekir.

1. **Müşteriler** ' i ve ardından **yeni müşteri** ' yi seçin.

2. **Hesap bilgileri** altında şirketin ve birincil kişisinin bilgilerini girin.

3. **Microsoft sözleşmesi** ' nin altında, müşterinin Microsoft Müşteri anlaşmasını kabul etmiş olduğunu doğrulamak için kutuyu seçin.

4. **Sözleşme kabul tarihi** altında, uygun tarihi girin. Bunu gelecekteki bir tarihle ayarlayamazsınız.

5. Görüntülenen birincil kullanıcı iletişim bilgilerinin doğru olduğundan emin olun. Yanlış ise **Güncelleştir** ' i seçin ve sözleşmeyi kabul eden kişi için doğru bilgileri girin.

6. Müşteri kiracısını oluşturmaya devam etmek için **İleri ' yi** seçin.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Yeni müşteri":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Mevcut müşteriler için müşteri kabulünü Onayla

Bunu yapmak için bir Yönetim Aracısı veya satış aracısı olmanız gerekir:

1. **Müşteriler** ’i seçin. Müşteriyi bulun ve seçin.

2. **Hesap bilgilerini** seçin.

3. **Microsoft Müşteri Sözleşmesi** altında **Güncelleştir** ' i seçin.

4. Sözleşmeyi kabul eden kişinin **adı** , **Soyadı** , **e-posta adresi** ve **telefon numarasını** (isteğe bağlı) girin. **Sözleşme kabul tarihi** altında, uygun tarihi girin. Bunu gelecekteki bir tarihle ayarlayamazsınız.

5. **Kaydet** ve devam et ' i seçin.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Yeni müşteri":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Müşteri kabulü onayını al

Aşağıdaki adımları kullanarak mevcut bir müşterinin Microsoft Müşteri anlaşmasını kabul etmiş olduğunu onaylayın. Bunu yapmak için bir Yönetim Aracısı veya satış aracısı olmanız gerekir.

1. **Müşteriler** ' i seçin ve ardından görmek istediğiniz müşteriyi bulun ve seçin.

2. **Hesap bilgilerini** seçin.

3. **Microsoft Müşteri Sözleşmesi** ' nin altında, bu müşteri tarafından onay olup olmadığını veya bu müşteri tarafından sağlanmadığını görüntüleyin.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Iş Ortağı Merkezi API/SDK kullanarak müşteri kabulünü onaylama

Iş Ortağı Merkezi API/SDK 'sını, Microsoft Müşteri sözleşmesinin müşteri tarafından kabul edildiğini onaylamak için kullanabilirsiniz. API/SDK hakkında daha fazla bilgi için bkz:

- [Microsoft Müşteri Sözleşmesi için anlaşma meta verilerini alın](/partner-center/develop/get-customer-agreement-metadata)

- [Microsoft Müşteri sözleşmesinin müşteri kabulünü Onayla](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Microsoft Müşteri sözleşmesinin müşteri kabulünün onayını alın](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Microsoft müşteri anlaşması şablonu için bir indirme bağlantısı alın](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Seçenek 2: Microsoft 365 Yönetim merkezinde müşteri kabulü

İş ortakları yeni ve mevcut müşterileri bir URL aracılığıyla davet ederek Microsoft 365 Yönetim Merkezi 'ndeki sözleşmeyi gözden geçirebilir ve kabul edebilir. Sonraki birkaç bölümde nasıl yapılacağı gösterilmektedir:

- Yeni bir müşteri oluşturun ve sözleşmeyi gözden geçirmek ve kabul etmek için müşteriyi davet edin.

- Satıcı ilişkilerini ve anlaşmasını gözden geçirmek ve kabul etmek için yeni bir müşteri davet edin.

- Mevcut bir müşteriyi gözden geçirip sözleşmeyi kabul edecek şekilde davet edin.

>[!NOTE]
> [Iş ortağı MERKEZI API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) 'sını, müşterinin Microsoft Müşteri sözleşmesinin doğrudan kabulüne ilişkin durumunu almak için kullanabilirsiniz.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Yeni bir müşteri oluşturun ve sözleşmeyi gözden geçirmek ve kabul etmek için müşteriyi davet edin

Iş Ortağı Merkezi 'nde yeni bir müşteri oluşturmak için aşağıdaki adımları kullanın ve ardından Microsoft 365 Yönetim Merkezi 'nde Microsoft Müşteri anlaşmasını gözden geçirip kabul edin.

1. Iş Ortağı Merkezi 'nin içindeki **müşteriler** sekmesinden **Müşteri Ekle** ' yi seçin.

2. **Hesap bilgileri** altında, müşterinin Şirket adı ve birincil ilgili kişisi dahil olmak üzere tüm gerekli alanlara yeni müşteri hakkındaki bilgileri girin.

3. **Müşteri Sözleşmesi** ' nin altında, ilk seçeneği belirleyin, **müşterinin Microsoft 365 Yönetim merkezinde Microsoft Müşteri sözleşmesini kabul etmesi istenir** . Sayfadaki diğer tüm gerekli alanları doldurun.

4. Ileri ' yi seçin **: gözden geçirin** ve ardından müşteri kiracısını oluşturma adımlarına devam edin. 

>[!NOTE] 
>Yeni müşteriler, Microsoft Müşteri anlaşmasını kabul edene kadar yeni bir satın alma yapamaz.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Yeni müşteri":::

5. Yeni müşteri iş akışındaki **onay** ekranına ulaştığınızda müşteri kimlik bilgilerini kaydedin. Bu kimlik bilgilerini müşterinize daha sonra sağlamanız gerekir.

6. Iş ortağı merkezi dışında, Microsoft 365 Yönetim merkezinde Microsoft Müşteri anlaşmasını kabul etmek üzere müşteriyi davet eden bir e-posta oluşturun ve gönderin. Bu öğeleri e-postaya eklediğinizden emin olun:

   - Bu [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) 'ye bir bağlantı (oturum açma gerekir)

   - 5. adımda kaydettiğiniz müşterinin kimlik bilgileri.

7. Müşteri, daha sonra iş ortağından gelen daveti alacak ve [URL 'yi](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)seçmeyecektir.

8. Müşteri, iş ortağından daha önce alınan müşteri kimlik bilgilerini kullanarak Microsoft 365 Yönetim Merkezi 'Nde oturum açar.

9. Müşteri daha sonra Microsoft Müşteri anlaşmasını kabul etmek için kutuyu kontrol eder.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Satıcı ilişkilerini gözden geçirmek ve kabul etmek için yeni bir müşteri davet edin ve Microsoft Müşteri Sözleşmesi 

Yeni bir müşteriyi gözden geçirmek ve satıcı ilişkilerini ve Microsoft Müşteri anlaşmasını kabul etmek üzere davet etmek için aşağıdaki adımları kullanın. 

1. Iş Ortağı Merkezi 'nin içindeki **müşteriler** sekmesinden **bir satıcı ilişki iste** bağlantısı ' nı seçin. 

2. Metin ve müşteriyi Microsoft 365 yönetim merkezine yönlendiren parametreli bir URL dahil olmak üzere otomatik e-posta şablonu oluşturulacaktır.

3. Otomatik olarak oluşturulan e-posta şablonunu özelleştirebilir ve sonra **Panoya Kopyala** ' yı seçerek **e-posta ile açabilirsiniz** .

4. Müşteriyi **satıcı ilişki** Isteği ve **Microsoft Müşteri Sözleşmesi 'ni** kabul etmek üzere davet etmek için bu e-posta şablonunu kullanın. (Örneğin, e-posta davetinin Içinde, iş ortağının otomatik olarak sağlanmış URL 'YI ve son zamanlarda oluşturulan müşteri kimlik bilgilerini de içerdiğinden emin olun.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Yeni müşteri":::

5. Müşteri e-posta ile davet alır ve parametreli URL 'yi tıklatır. 

6. Müşteri, Microsoft 365 Yönetim Merkezi 'Nde oturum açmak için iş ortağı tarafından belirtilen kimlik bilgilerini kullanır.

7. Müşteri, **satıcı ilişkilerini** ve **Microsoft Müşteri anlaşmasını** kabul etmek için kutuyu kontrol eder. 

8. Aynı URL içinde, müşteri üzerinde çalıştıkları farklı iş ortaklarının birleştirilmiş bir listesini görebilir. Ayrıntıları görmek için bir iş ortağı seçebilir.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Yeni müşteri":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Anlaşmayı gözden geçirmek ve kabul etmek için mevcut bir müşteriyi davet etme

Mevcut bir müşteriyi gözden geçirmek ve Microsoft Müşteri anlaşmasını kabul etmek üzere davet etmek için aşağıdaki adımları kullanın. 

1. Müşteri e-postasını, Microsoft Müşteri anlaşmasını kabul etmek için müşterinize davet eden gömülü URL ile oluşturun.

2. Müşteriniz daveti e-posta yoluyla alır ve [URL 'yi](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)tıklatır. 

3. Müşteri kimlik bilgilerini Microsoft 365 yönetim merkezine girer.

4. Müşteriniz, Microsoft Müşteri anlaşmasını kabul etmek için kutuyu kontrol eder. 

5. Aynı URL içinde, müşteri üzerinde çalıştıkları farklı iş ortaklarının birleştirilmiş listesini görebilir. Ayrıntıları görmek için bir iş ortağı seçebilir.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Yeni müşteri":::

>[!NOTE]
>Bazı senaryolarda, müşteriler Microsoft Müşteri anlaşmasını doğrudan kabul edemeyebilir. Bu durumlar hakkında daha fazla bilgi edinmek için, [Müşterinizin adına sınama yapmanız gereken iki senaryoya](attest-acceptance-customer-agreement.md)bakın.

### <a name="historical-timeline-details"></a>Geçmiş zaman çizelgesi ayrıntıları

| Tarih | Ina | Ayrıntılar |
|------------|------------|--------------------------------|
|01 Ağustos 2019| Sanal alanda UX önizlemesi kullanılabilir| İş ortakları, CSP korumalı alan ortamındaki Iş Ortağı Merkezi panosunu kullanarak Microsoft Müşteri sözleşmesinin müşteri kabul edildiğini doğrulayabilirsiniz. CSP korumalı alan ortamına erişimi olan iş ortakları, Kullanıcı deneyimi değişikliklerini önizleyin. Sandbox erişimi olmayan iş ortakları, bu konudaki değişiklikler hakkında bilgi alabilir.|
|03 Eylül 2019|API önizlemesi, korumalı alanında kullanılabilir.|İş ortağı, CSP korumalı alan ortamında Iş Ortağı Merkezi API 'sini kullanarak Microsoft Müşteri sözleşmesinin müşteri tarafından kabul edildiğini doğrulayabilirsiniz. API iş ortakları, API değişikliklerini önizlemek ve yeni sözleşmeyi desteklemek üzere API Tümleştirmesi üzerinde çalışmaya başlamak için bu fırsatı kullanabilir.|
|20 Eylül 2019|.NET SDK önizlemesi, korumalı alanında kullanılabilir.|İş ortağı, CSP Sandbox ortamında Iş ortağı merkezi .NET SDK 'sını kullanarak Microsoft Müşteri sözleşmesinin müşteri tarafından kabul edildiğini doğrulayabilirsiniz. API iş ortakları, bu fırsatı kullanarak .NET SDK değişikliklerinin önizlemesini yapabilir ve yeni sözleşmeyi desteklemek üzere API Tümleştirmesi üzerinde çalışmaya başlayabilir.|
|01 Ekim 2019|Üretimde sunulan Microsoft Müşteri Sözleşmesi|Microsoft, Microsoft Bulut sözleşmesinin yerini alacak şekilde CSP programına Microsoft Müşteri Sözleşmesi 'ni tanıtır. İş ortakları, Iş Ortağı Merkezi panosunu ve üretimde API 'YI kullanarak Microsoft Müşteri sözleşmesinin müşteri tarafından kabul edildiğini doğrulayabilirsiniz. Microsoft Bulut sözleşmesi, CSP iş ortağı programı içinde desteklenir. Bununla birlikte, iş ortaklarının Microsoft Müşteri sözleşmesine geçirmeye başlaması önerilir. Mevcut Aboneliklerde yapılan yeni satın almalar ve lisans sayısı değişiklikleri, Microsoft Müşteri sözleşmesinin veya Microsoft Bulut sözleşmesinin iş ortağı onayını gerektirir. Belirli yeni teklifler (örneğin, yeni Azure planı) Microsoft Müşteri sözleşmesinin onayını gerektirecektir.|
|31 Ocak 2020|Microsoft Bulut sözleşmesi Üretimden kaldırıldı|Microsoft Bulut sözleşmesi artık CSP iş ortağı programı içinde kabul edilmez. Mevcut Aboneliklerde yapılan yeni satın almalar ve lisans sayısı değişiklikleri, ortağın Microsoft Müşteri Sözleşmesi onayını sağlamasını gerektirir. Bu gereksinim, yeni müşteriler ve Microsoft Bulut sözleşmesini önceden kabul etmiş olabilecek mevcut müşteriler için geçerlidir.|
|3 Şubat 2020|İş ortağı artık, kimliği doğrulanmış Microsoft 365 Yönetim Merkezi 'nde sözleşmeyi gözden geçirmek ve kabul etmek için bir URL aracılığıyla müşteriyi davet etme seçeneğine sahiptir. | Müşteri, Microsoft 365 Yönetim Merkezi 'nde Microsoft Müşteri anlaşmasını kabul edebilir. Müşterinin Microsoft 365 Yönetim Merkezi 'nde sözleşmenin doğrudan kabulü, koşulların onayını onaylar. 