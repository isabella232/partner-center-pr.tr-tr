---
title: Müşteri hesabı için birden çok kullanıcı ekleme
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Müşterinin hesabına birden çok kullanıcı eklemek için, virgülle ayrılmış değer (.csv) dosya biçimini kullanarak İş Ortağı Merkezi dosyasına bir veri dosyası yükleyin.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150480"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="4f85b-103">Kullanıcıların bir .csv dosyasını müşterinin hesabına yükleme</span><span class="sxs-lookup"><span data-stu-id="4f85b-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="4f85b-104">**Uygun roller:** Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="4f85b-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="4f85b-105">Virgülle ayrılmış değer dosyası biçimindeki (.csv) bir veri dosyasını aynı anda müşterinin hesabına birden çok kullanıcı İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="4f85b-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="4f85b-106">Müşteri kullanıcılarının dosyasını oluşturma ve müşteri hesabına yükleme</span><span class="sxs-lookup"><span data-stu-id="4f85b-106">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="4f85b-107">Yukarıda açıklanan verilerle virgülle ayrılmış bir değer (.csv) veri dosyası oluşturun.</span><span class="sxs-lookup"><span data-stu-id="4f85b-107">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="4f85b-108">Dosyayı daha sonraki bir adımda göz atabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4f85b-108">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="4f85b-109">Bir [müşteri hesabı için birden çok kullanıcı içeri aktaracak .csv dosyası alanları'ne bakın.](file-customer-users.md)</span><span class="sxs-lookup"><span data-stu-id="4f85b-109">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="4f85b-110">İş Ortağı Merkezi [oturum açın.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="4f85b-110">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="4f85b-111">Yeni İş Ortağı Merkezi **Müşteriler'i ve** ardından listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="4f85b-111">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="4f85b-112">Müşterinin Kullanıcılar ve Lisanslar **sekmesini ve ardından Kullanıcıları** karşıya **yükle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="4f85b-112">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="4f85b-113">Kullanıcı **bilgilerini karşıya yükle altında Gözat'ı** **seçin.**</span><span class="sxs-lookup"><span data-stu-id="4f85b-113">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="4f85b-114">Dosya seçicide veri dosyanızı ve ardından Aç'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="4f85b-114">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="4f85b-115">**Doğrula**'yı seçin.</span><span class="sxs-lookup"><span data-stu-id="4f85b-115">Select **Validate**.</span></span>

    <span data-ttu-id="4f85b-116">**Not**  Hesap oluşturma hatalarının çoğu eksik bilgiler, yanlış biçimlendirilmiş veya yinelenen e-posta adresleri veya dosyada çok fazla kayıt gibi veri dosyası sorunlarından kaynaklandı.</span><span class="sxs-lookup"><span data-stu-id="4f85b-116">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="4f85b-117">Dosya İş Ortağı Merkezi sonra yeni kullanıcılar için coğrafi **Konum'ı** seçin.</span><span class="sxs-lookup"><span data-stu-id="4f85b-117">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="4f85b-118">**Kaydet**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="4f85b-118">Select **Save**.</span></span>
10. <span data-ttu-id="4f85b-119">Kullanıcılar için geçici parola bilgilerini indirin.</span><span class="sxs-lookup"><span data-stu-id="4f85b-119">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="4f85b-120">Bu işlemi daha sonra yapayasınız, şimdi geçici parolalarla dosyayı indirmeyi deneyin.</span><span class="sxs-lookup"><span data-stu-id="4f85b-120">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="4f85b-121">Yeni kullanıcıların yeni hesapları için geçici parolayı kullanarak yeni hesaplarında oturum açmaları gerekir.</span><span class="sxs-lookup"><span data-stu-id="4f85b-121">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="4f85b-122">Yeni kullanıcılara lisansları ve hizmetleri kullanabilir **izni otomatik olarak atanır.**</span><span class="sxs-lookup"><span data-stu-id="4f85b-122">New users are automatically assigned permissions of **Can use licenses and services**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="4f85b-123">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="4f85b-123">Next steps</span></span>

- [<span data-ttu-id="4f85b-124">Iş Ortağı Merkezi 'nde müşterilere kendi ürünlerini veya hizmetlerini satın alma izni verin</span><span class="sxs-lookup"><span data-stu-id="4f85b-124">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
