---
title: İş ortağı hesabınızdaki konumları yönetin
ms.topic: article
ms.date: 10/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Yeni bir konum ekleme ve bilgisayar, CSP iş, abonelik ve diğer işlemlerde MPN KIMLIĞI 'nin nasıl kullanıldığını öğrenin.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c6b0fc84636befedbc51aa0672ce19110eb4d9aa
ms.sourcegitcommit: 1719ff11409cd6953602b7798f8cfe821b8ea15e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/15/2020
ms.locfileid: "92531971"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>MPN hesap konumlarını yönetin ve yeni bir konum ekleyin

**Uygulama hedefi**

- İş Ortağı Merkezi

**Uygun roller**

- Genel yönetici
- Hesap yöneticisi

MPN KIMLIĞI konumu, şirketinizin her belirli bir konumunu tanımlar. MPN KIMLIK konumunu kullanarak, uygulamaları, Transact bulut çözümü sağlayıcısı (CSP) işletme ve diğer iş işlemlerine, teşvik etmek için kullanabilirsiniz. Genel MPN KIMLIĞI, destek istekleri gibi işlem olmayan etkinlikler için kullanılır.

## <a name="the-following-is-a-typical-scenario"></a>Tipik bir senaryo aşağıda verilmiştir:

Contoso, UK 'teki ortak genel hesabına (PGA) sahiptir. Bu, kayıtlı yasal işletmektir ve tüm işlemsel olmayan işleri yönetmek için Global MPN KIMLIĞI kullanılır. Contoso Ayrıca, UK, Fransa ve ABD 'de başka bir konumdaki yan kuruluşlar veya bölümler için Iş ortağı konum hesapları (PLA) ile eşdeğerdir. MPN hesap yapısında, bu PLAs 'ler benzersiz konum MPN kimlikleri olarak gösterilir. PLAs 'ler, CSP veya teşvikleri programları gibi işlem işleri için kullanılır. Ödemeler belirli konumlara bağlıdır. 

>[!NOTE]
>CSP kiracısı ve MPN konum KIMLIĞI arasında bir 1-1 ilişkisi vardır.

:::image type="content" source="images/locations/locations1.png" alt-text="MPN konumlarının yapısı":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a>CSP iş için yeni bir konum eklemek üzere Önkoşullar

Yeni bir CSP iş konumu eklemek için birkaç önkoşul vardır:

1. İş yapmak istediğiniz ülkede MPN KIMLIĞI 'ne sahip olmanız gerekir.

1. [İş bölgesinde](regional-authorization-overview.md) zaten CSP 'ye kayıtlı olmayan yeni BIR Azure AD kiracısına sahip olmanız gerekir. CSP 'ye kaydoldığınızda bunu oluşturun.
 
3. Bölgede CSP programına kaydolmak için yeni AAD kiracısını kullanın.
Yasal Şirket adı, adres, birincil iletişim ayrıntıları dahil yasal Şirket ayrıntılarını sağlama. Bu hesap, doğrulamaya devam edecek, bu nedenle geçerli bilgiler eklediğinizden emin olun.

>[!NOTE] 
 >**Yeni** Azure AD kiracısı için **Yeni** kimlik bilgileriyle oturum açmayı unutmayın. Mevcut kimlik bilgilerinizi, Iş Ortağı Merkezi zaten bir hesap varmış gibi tanıyacak şekilde kullanmayacaktır.

4. Microsoft Iş ortağı sözleşmesi 'Ni kabul edin ve hesabı etkinleştirin.

## <a name="add-an-mpn-location"></a>MPN konumu ekleme

1. Iş Ortağı Merkezi 'nde MPN hesabını kullanarak oturum açın. MPN hesabının genel yönetici veya hesap yönetici ayrıcalıklarına sahip olması gerekir. 

1. **Ayar simgesinden** **iş ortağı ayarları** ' nı seçin.

2. **Konum seçin.**

3. **Konum Ekle** ' yi seçin ve şirkete eklemek istediğiniz konumun adres ayrıntılarını ve konum için bir birincil kişiyi ekleyin.

> [!NOTE]
> Iş Ortağı Merkezi 'ne bir konum eklendikten sonra kaldırılamaz. Oturum açmak için doğru MPN KIMLIĞINI kullandıysanız, **MPN** 'Yi Iş Ortağı Merkezi 'nin sol menüsünde görürsünüz.

## <a name="change-global-partner-account-location"></a>Küresel iş ortağı hesabı konumunu değiştir

1. **[Konumlar](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** sayfasında, yasal varlığınız olarak istediğiniz konumun listelendiğinden emin olmak için konumların listesini kontrol edin. Değilse, ekleyin.

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="MPN konumlarının yapısı":::

2. **Iş ortağı profilini** seçin ve ardından **yasal iş profilini Güncelleştir** ' i seçin.

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="MPN konumlarının yapısı":::

3. Bölgeyi ve yasal varlığı seçip **gönderebilirsiniz** .

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="MPN konumlarının yapısı":::

## <a name="next-steps"></a>Sonraki adımlar

- [Doğrulama süreci](verification-responses.md)hakkında bilgi edinin.
