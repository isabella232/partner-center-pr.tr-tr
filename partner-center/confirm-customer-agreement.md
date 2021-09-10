---
title: Müşterinizin, Microsoft Müşteri anlaşmasını CSP programına kabul ettiğini onaylama
description: Bulut Çözümü Sağlayıcısı (CSP) iş ortaklarının, müşteriler için Microsoft hizmetleri sipariş etmeden önce Microsoft müşteri sözleşmesinin müşteri kabulünü onaylamasını gerekir.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: aa8f08b52a16aae56b02b09d5fdf607e92180ca5
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960055"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Müşterinizin, Microsoft Müşteri anlaşmasını CSP programına kabul ettiğini onaylama

**Uygun roller**: yönetici Aracısı | Satış Aracısı


Müşterilerin, Microsoft Müşteri anlaşmasını kabul ettikleri iki seçeneği vardır.

**Seçenek 1**: müşteri kabulünü kabul eden iş ortağı kanıtı Iş Ortağı Merkezi API/SDK kullanarak veya Iş Ortağı Merkezi panosu aracılığıyla müşteri kabulünü doğrulayabilirler.

**seçenek 2**: müşteri doğrudan kabul-ortağı, Microsoft 365 Yönetici merkezindeki sözleşmeyi gözden geçirmek ve kabul etmek için bir URL aracılığıyla müşteriyi davet edebilir.

## <a name="access-microsoft-customer-agreement-template"></a>Microsoft müşteri anlaşması şablonuna erişin

Microsoft müşteri anlaşması şablonunun en son sürümünü [buradan](https://aka.ms/customeragreement)el ile indirebilirsiniz. Microsoft Müşteri Sözleşmesi ülkeye özeldir. Microsoft müşteri anlaşması şablonunu istenirken, müşterinin konumuna göre doğru ülkeyi seçtiğinizden emin olun.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Seçenek 1: Iş Ortağı Merkezi 'nde müşteri kabulünü onaylayın

Doğrudan fatura ortakları, yeni ve mevcut müşteriler için Iş Ortağı Merkezi 'nde Microsoft Müşteri sözleşmesinin müşteri tarafından kabul edildiğini doğrulayabilirsiniz. Dolaylı satıcılar müşterilerinin adına test edemez ve kanıtlama tamamlandı olarak kendi dolaylı sağlayıcısıyla birlikte çalışmalıdır.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Yeni müşteriler için müşteri kabulünü Onayla

Iş Ortağı Merkezi 'nde yeni bir müşteri kiracısı oluşturduğunuzda, müşterinin Microsoft Müşteri sözleşmesinin kabul edildiğini onaylamak için aşağıdaki adımları kullanın. Bu adımları gerçekleştirmek için bir yönetici Aracısı veya satış aracısı olmanız gerekir.

1. **Müşteriler**' i ve ardından **yeni müşteri**' yi seçin.

2. **Hesap bilgileri** altında şirketin ve birincil kişisinin bilgilerini girin.

3. **Microsoft sözleşmesi**' nin altında, müşterinin Microsoft Müşteri anlaşmasını kabul etmiş olduğunu doğrulamak için kutuyu seçin.

4. **Sözleşme kabul tarihi** altında, uygun tarihi girin. Bunu gelecekteki bir tarihle ayarlayamazsınız.

5. Görüntülenen birincil kullanıcı iletişim bilgilerinin doğru olduğundan emin olun. Yanlış ise **Güncelleştir** ' i seçin ve sözleşmeyi kabul eden kişi için doğru bilgileri girin.

6. Müşteri kiracısını oluşturmaya devam etmek için **İleri ' yi** seçin.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Yeni müşteri.":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Mevcut müşteriler için müşteri kabulünü Onayla

Bunu yapmak için bir Yönetim Aracısı veya satış aracısı olmanız gerekir:

1. **Müşteriler**’i seçin. Müşteriyi bulun ve seçin.

2. **Hesap bilgilerini** seçin.

3. **Microsoft Müşteri Sözleşmesi** altında **Güncelleştir**' i seçin.

4. sözleşmeyi kabul eden kişinin **adı**, **soyadı**, **e-posta adresi** ve **Telefon numarasını** (isteğe bağlı) girin. **Sözleşme kabul tarihi** altında, uygun tarihi girin. Bunu gelecekteki bir tarihle ayarlayamazsınız.

5. **Kaydet** ve devam et ' i seçin.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Mevcut müşteri.":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Müşteri kabulü onayını al

Mevcut bir müşterinin Microsoft Müşteri anlaşmasını kabul etmiş olduğunu onaylamak için aşağıdaki adımları kullanın. Bunu yapmak için bir Yönetim Aracısı veya satış aracısı olmanız gerekir.

1. **Müşteriler**' i seçin ve ardından görmek istediğiniz müşteriyi bulun ve seçin.

2. **Hesap bilgilerini** seçin.

3. **Microsoft Müşteri Sözleşmesi**' nin altında, bu müşteri tarafından onay olup olmadığını veya bu müşteri tarafından sağlanmadığını görüntüleyin.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Iş Ortağı Merkezi API/SDK kullanarak müşteri kabulünü onaylama

Iş Ortağı Merkezi API/SDK 'sını, Microsoft Müşteri sözleşmesinin müşteri tarafından kabul edildiğini onaylamak için kullanabilirsiniz. API/SDK hakkında daha fazla bilgi için bkz:

- [Microsoft Müşteri Sözleşmesi için anlaşma meta verilerini alma](/partner-center/develop/get-customer-agreement-metadata)

- [Microsoft Müşteri Sözleşmesinin müşteri kabulünü onaylama](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Microsoft Müşteri Sözleşmesinin müşteri kabulünün onayını alma](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Microsoft müşteri anlaşması şablonu için bir indirme bağlantısı alın](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>seçenek 2: Microsoft 365 Yönetici merkezinde müşteri kabulü

iş ortakları yeni ve mevcut müşterileri bir URL aracılığıyla davet ederek Microsoft 365 Yönetici merkezi içindeki sözleşmeyi gözden geçirebilir ve kabul edebilir. Sonraki birkaç bölümde nasıl yapılacağı gösterilmektedir:

- Yeni bir müşteri oluşturun ve sözleşmeyi gözden geçirmek ve kabul etmek için müşteriyi davet edin.

- Satıcı ilişkilerini ve anlaşmasını gözden geçirmek ve kabul etmek için yeni bir müşteri davet edin.

- Mevcut bir müşteriyi gözden geçirip sözleşmeyi kabul edecek şekilde davet edin.

>[!NOTE]
> [Iş ortağı MERKEZI API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) 'sını, müşterinin Microsoft Müşteri sözleşmesinin doğrudan kabulüne ilişkin durumunu almak için kullanabilirsiniz.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Yeni bir müşteri oluşturun ve sözleşmeyi gözden geçirmek ve kabul etmek için müşteriyi davet edin

iş ortağı merkezi 'nde yeni bir müşteri oluşturmak için aşağıdaki adımları kullanın, ardından Microsoft 365 Yönetici Center içindeki Microsoft müşteri sözleşmesini gözden geçirip kabul edin.

1. Iş Ortağı Merkezi 'nin içindeki **müşteriler** sekmesinden **Müşteri Ekle**' yi seçin.

2. **Hesap bilgileri** altında, müşterinin Şirket adı ve birincil ilgili kişisi dahil olmak üzere tüm gerekli alanlara yeni müşteri hakkındaki bilgileri girin.

3. **müşteri sözleşmesi**' nin altında, **müşteri Microsoft 365 Yönetici merkezi 'nde Microsoft müşteri anlaşmasını kabul etmesi istenecektir**. Sayfadaki diğer tüm gerekli alanları doldurun.

4. Ileri ' yi seçin **: gözden geçirin** ve ardından müşteri kiracısını oluşturma adımlarına devam edin. 

>[!NOTE] 
>Yeni müşteriler, Microsoft Müşteri anlaşmasını kabul edene kadar satın alma yapamaz.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Yeni müşteri oluşturun.":::

5. Yeni müşteri iş akışındaki **onay** ekranına ulaştığınızda müşteri kimlik bilgilerini kaydedin. Bu kimlik bilgilerini müşterinize daha sonra sağlamanız gerekir.

6. iş ortağı merkezi dışında, Microsoft müşteri anlaşmasını Microsoft 365 Yönetici Center 'da kabul etmek üzere müşteriyi davet eden bir e-posta oluşturun ve gönderin. Bu öğeleri e-postaya eklediğinizden emin olun:

   - Bu [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) 'ye bir bağlantı (oturum açma gerekir)

   - 5. adımda kaydettiğiniz müşterinin kimlik bilgileri.

7. Müşteri, daha sonra iş ortağından gelen daveti alacak ve [URL 'yi](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)seçmeyecektir.

8. müşteri, verdiğiniz müşteri kimlik bilgilerini kullanarak Microsoft 365 Yönetici Center 'da oturum açar.

9. Müşteri, Microsoft Müşteri anlaşmasını kabul etmek için kutuyu kontrol eder.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Satıcı ilişkilerini gözden geçirmek ve kabul etmek için yeni bir müşteri davet edin ve Microsoft Müşteri Sözleşmesi 

Yeni bir müşteriyi gözden geçirmek ve satıcı ilişkilerini ve Microsoft Müşteri anlaşmasını kabul etmek üzere davet etmek için aşağıdaki adımları kullanın. 

1. Iş Ortağı Merkezi 'nin içindeki **müşteriler** sekmesinden **bir satıcı ilişki iste** bağlantısı ' nı seçin. 

2. metin ve müşteriyi Microsoft 365 Yönetici merkezine yönlendiren parametreli bir URL dahil olmak üzere otomatik e-posta şablonu oluşturulacaktır.

3. Otomatik olarak oluşturulan e-posta şablonunu özelleştirebilir ve sonra **Panoya Kopyala** ' yı seçerek **e-posta ile açabilirsiniz**.

4. Müşteriyi **satıcı ilişki** Isteği ve **Microsoft Müşteri Sözleşmesi 'ni** kabul etmek üzere davet etmek için bu e-posta şablonunu kullanın. (Örneğin, e-posta davetinin Içinde, iş ortağının otomatik olarak sağlanmış URL 'YI ve son zamanlarda oluşturulan müşteri kimlik bilgilerini de içerdiğinden emin olun.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="ilişki oluşturun.":::

5. Müşteri e-posta ile davet alır ve parametreli URL 'yi tıklatır. 

6. müşteri e-posta içinde Microsoft 365 Yönetici merkezi 'nde oturum açmak için sağladığınız kimlik bilgilerini kullanır.

7. Müşteri, **satıcı ilişkilerini** ve **Microsoft Müşteri anlaşmasını** kabul etmek için kutuyu kontrol eder. 

8. Aynı URL içinde, müşteri üzerinde çalıştıkları farklı iş ortaklarının birleştirilmiş bir listesini görebilir. Ayrıntıları görmek için bir iş ortağı seçebilir.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Sözleşmeyi kabul edin.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Anlaşmayı gözden geçirmek ve kabul etmek için mevcut bir müşteriyi davet etme

Mevcut bir müşteriyi gözden geçirmek ve Microsoft Müşteri anlaşmasını kabul etmek üzere davet etmek için aşağıdaki adımları kullanın. 

1. Müşteri e-postasını, Microsoft Müşteri anlaşmasını kabul etmek için müşterinize davet eden gömülü URL ile oluşturun.

2. Müşteriniz daveti e-posta yoluyla alır ve [URL 'yi](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)tıklatır. 

3. müşteri, kimlik bilgilerini Microsoft 365 Yönetici merkezine girer.

4. Müşteriniz, Microsoft Müşteri anlaşmasını kabul etmek için kutuyu kontrol eder. 

5. Aynı URL içinde, müşteri üzerinde çalıştıkları farklı iş ortaklarının birleştirilmiş listesini görebilir. Ayrıntıları görmek için bir iş ortağı seçebilir.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="müşterisi.":::

>[!NOTE]
>Bazı senaryolarda, müşteriler Microsoft Müşteri anlaşmasını doğrudan kabul edemeyebilir. Bu durumlar hakkında daha fazla bilgi edinmek için, aşağıdaki Müşterinizin adına sınamanız gereken Iki senaryoyu okuyun.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Müşteriniz adına bunu test etmek için ihtiyacınız olan iki senaryo

Müşterilerin Microsoft 365 Yönetici Center'da doğrudan kabul edile Microsoft Müşteri Sözleşmesi iki senaryo vardır.

**Senaryo 1:** Mevcut bir müşteri, mevcut iş ortağı ilişkisi aracılığıyla aşağıdakilerin herhangi birini satın aldı: teklifler, yazılım veya yazılım abonelikleri, Ayrılmış Örnekler veya Azure planı. Müşteri şimdi yeni satın alma işlemleri yapmaya (otomatik yenileme hariç) başvurur. Müşteri URL'ye tıkladığında "Lütfen İş Ortağınıza ulaşarak url'yi kabul Microsoft Müşteri Sözleşmesi."  

**Sorununu çözmek** için: Müşteri adına bunu doğrulayın.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="İş Microsoft 365 Yönetici onayını onaylamak için iş ortağınıza ulaşmanızı isteyen Microsoft Müşteri Sözleşmesi.":::

**Senaryo 2:** Mevcut bir müşteri aşağıdaki tekliflerden, yazılım ve yazılım aboneliklerinin, Ayrılmış Örneklerin ve Azure planının herhangi birini satın aldı. Müşteri şimdi yeni bir iş ortağıyla yeni satın alma girişiminde bulundu.

Müşteri yeni iş ortağı ilişkisini ve sözleşmeyi kabul etmek için Microsoft 365 Yönetici Center URL'sini tıkladığında "Lütfen İş Ortağınıza ulaşarak bu ilişkiyi kabul ettiğinize emin olmak için Microsoft Müşteri Sözleşmesi."  

**Sorununu çözmek** için: Müşteri adına bunu doğrulayın.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Müşterinin sözleşmeyi kabul etmiş olduğunu onaylayın

Daha önce onaylamadınız mevcut bir müşteri için yeni bir sipariş oluşturmanız gerekirse, onayı tamamlamanız için bir istem alırsınız. Bunu yapmak için aşağıdaki yordamı kullanın.

1. Sözleşmeyi **kabul eden** kullanıcının **ad,** **Soyadı,** **Telefon** adresi ve kimlik numarasını (isteğe bağlı) girin.

2. Sözleşme **kabul tarihi'nin** altında uygun tarihi girin. Bunu gelecekteki bir tarihe ayaramazsiniz.

3. **Kaydet ve devam et**’i seçin. 

## <a name="next-steps"></a>Sonraki adımlar

- [Şirket profili bilgilerini doğrulama veya güncelleştirme](update-your-partner-profile.md)
- [Microsoft Müşteri Sözleşmeleri (bölgeye, dile göre)](Agreements.md)
