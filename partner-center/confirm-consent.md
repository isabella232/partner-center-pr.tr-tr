---
title: Microsoft Müşteri Sözleşmesinin müşteri kabulünü onaylama
description: Microsoft Müşteri sözleşmesinin müşteri kabulünü onaylama hakkında bilgi edinin. Bu, müşterilerin Microsoft ürünlerini ve hizmetlerini sıralamak için gerekebilir.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/02/2021
ms.openlocfilehash: ab2f5be77f6480b4a8b47bef0e0fd5096f7c1776
ms.sourcegitcommit: a7897284b79abb1ceeee79deb3a87b72d59900dc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "102029925"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Müşterinin Microsoft Müşteri Sözleşmesi’ni kabul ettiğini doğrulama


**Uygun roller**

- Yönetim Aracısı
- Satış Aracısı

> [!NOTE]
> Sözleşme kaynağı şu anda yalnızca Microsoft genel bulutundaki Iş Ortağı Merkezi tarafından desteklenmektedir. Şunları yapmak için geçerli değildir:
> * 21Vianet tarafından çalıştırılan iş ortağı Merkezi
> * Microsoft Bulut Almanya için İş Ortağı Merkezi
> * Microsoft Cloud for US Government için İş Ortağı Merkezi


İş ortağı olarak, müşterinin Microsoft ürünlerini ve hizmetlerini sipariş etmeden önce, müşterinizin Microsoft Müşteri sözleşmesini kabul etmeniz gerekir. İş ortaklarının uyumluluk gereksinimlerini karşıladığından daha iyi yardımcı olması için, Microsoft, anlaşmayı kabul eden kişiyle ilgili aşağıdaki ayrıntıları sağlayarak iş ortaklarının kabul onaylamasını ister:

- Ad

- Soyadı

- E-posta adresi

- Telefon numarası (isteğe bağlı)

- Kabul tarihi

Doğrudan fatura ortakları ve dolaylı sağlayıcılar, Iş ortağı merkezi veya Iş Ortağı Merkezi API 'SI aracılığıyla deneyimidir olduğunda Microsoft Müşteri sözleşmesinin müşteri kabulünü kabul etmelidir. Onay *zorunludur*.

>[!NOTE]
>31 Ocak 2020 itibariyle, mevcut ve yeni olan tüm müşteriler yeni Microsoft Müşteri sözleşmesinin imzalanmalıdır. Daha fazla bilgi edinmek için [Microsoft Müşteri sözleşmesinin müşteri kabulünü Onayla](confirm-customer-agreement.md)makalesini okuyun.

Belirli bir müşteri için onay sağlanmazsa:

- Bu müşteri için yeni siparişler oluşturamayacak.

- Bu müşteri için lisans tabanlı mevcut aboneliklerin lisans sayısını değiştiremeyeceksiniz.

Müşteri kabulünü onaylama işlemi, Iş ortağı merkezi veya Iş Ortağı Merkezi API 'SI aracılığıyla yapılabilir. Bunu Iş Ortağı Merkezi API 'SI aracılığıyla yapmak için aşağıdaki konulara bakın:

- [Müşteri onayı onayını al](/partner-center/develop/get-confirmation-of-customer-consent)

- [Anlaşma meta verilerini al](/partner-center/develop/get-agreement-metadata)

- [Müşteri onayını Onayla](/partner-center/develop/confirm-customer-consent)

Bu, hem üretim hem de korumalı ortamlar için geçerlidir.

## <a name="confirm-customer-acceptance-for-a-new-customer"></a>Yeni müşteri için müşteri kabulünü Onayla

Iş Ortağı Merkezi 'nde yeni bir müşteri kiracısı oluştururken müşteri kabulünü onaylamak için aşağıdaki yordamı kullanın. Bunu yapmak için bir Yönetim Aracısı veya satış aracısı olmanız gerekir.

1. **Müşteriler**' i ve ardından **yeni müşteri** ' yi seçip **hesap bilgileri**' ni seçin.

2. **Şirket** ve **birincil ilgili kişiyle** ilgili bilgileri girin.

   :::image type="content" source="images/mca/mca1.png" alt-text="Şirket bilgileri":::

3. **Microsoft Müşteri Sözleşmesi** altında **müşterinin en son Microsoft Müşteri anlaşmasını kabul etmiş olduğunu** seçin.

4. **Sözleşme kabul tarihi** altında, uygun tarihi girin. Bunu gelecekteki bir tarihle ayarlayamazsınız.

5. Kabulü sağlayan kullanıcının ayrıntılarını girin.

   :::image type="content" source="images/mca/MCA3.png" alt-text="Kabul tarihi Ekle":::

   Varsayılan olarak, birincil kişi Kullanıcı bilgileri görüntülenir. Bu doğru değilse **Güncelleştir** ' i seçin ve ardından sözleşmeyi kabul eden kişinin **adı**, **Soyadı**, **e-posta adresi** ve **telefon numarasını* (isteğe bağlı) girin.

6. Müşteri kiracısını oluşturmaya yönelik kalan adımlara devam etmek için **İleri ' yi** seçin.

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Mevcut bir müşteri için müşteri kabulünü Onayla

Bunu yapmak için bir Yönetim Aracısı veya satış aracısı olmanız gerekir.

1. **Müşteriler**' i seçin ve ardından görmek istediğiniz müşteriyi bulun ve seçin.

2. **Hesap bilgilerini** seçin.

3. **Microsoft Müşteri Sözleşmesi** altında **Güncelleştir**' i seçin.

   :::image type="content" source="images/mca/mca4.png" alt-text="Güncelleştirme":::

4. Sözleşmeyi kabul eden kullanıcının **adını**, **soyadını**, **e-posta adresini** ve **telefon numarasını** (isteğe bağlı) girin.

5. **Sözleşme kabul tarihi** altında, uygun tarihi girin. Bunu gelecekteki bir tarihle ayarlayamazsınız.

6. **Kaydet ve devam et**’i seçin.

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Mevcut bir müşteri için yeni sipariş oluştururken müşteri kabulünü Onayla

Daha önce teyit edilmemiş mevcut bir müşteri için yeni bir sipariş oluşturmayı denerseniz, onayı tamamlamaya yönelik bir istem alırsınız. Bunu yapmak için aşağıdaki yordamı kullanın.

1. Sözleşmeyi kabul eden kullanıcının **adını**, **soyadını**, **e-posta adresini** ve **telefon numarasını** (isteğe bağlı) girin.

2. **Sözleşme kabul tarihi** altında, uygun tarihi girin. Bunu gelecekteki bir tarihle ayarlayamazsınız.

3. **Kaydet ve devam et**’i seçin.

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Mevcut bir müşteri için müşteri kabulünün onayını alma

Aşağıdaki yordamı kullanarak daha önce sağlamış olduğunuz mevcut bir müşteri için müşteri kabulünün onayını alabilirsiniz. Bunu yapmak için bir Yönetim Aracısı veya satış aracısı olmanız gerekir.

1. **Müşteriler**' i seçin ve ardından görmek istediğiniz müşteriyi bulun ve seçin.

2. **Hesap bilgilerini** seçin.

3. **Microsoft Müşteri Sözleşmesi**' nin altında, bu müşteri için onay verilip verilmeyeceğini görürsünüz.

## <a name="next-steps"></a>Sonraki adımlar

- [CSP iş ortağı programında Microsoft Müşteri Sözleşmesi 'nin müşteri kabulünü onaylayın](confirm-customer-agreement.md)

- [Müşterinizin adına Microsoft Müşteri sözleşmesinin onay onayı](attest-acceptance-customer-agreement.md)