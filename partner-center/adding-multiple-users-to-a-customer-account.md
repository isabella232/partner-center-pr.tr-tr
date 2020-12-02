---
title: Müşteri hesabı için birden çok kullanıcı ekleme
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bir müşterinin hesabına birden çok kullanıcı eklemek için, virgülle ayrılmış değer (. csv) dosya biçimini kullanarak Iş Ortağı Merkezi 'ne bir veri dosyası yükleyin.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9f1d6e2a59bd892b7b79a1e3aa532242cdd0e302
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474198"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="7a857-103">Kullanıcıların bir. csv dosyasını bir müşterinin hesabına yükleyin</span><span class="sxs-lookup"><span data-stu-id="7a857-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="7a857-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="7a857-104">**Appropriate roles**</span></span>

- <span data-ttu-id="7a857-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="7a857-105">Global admin</span></span>

<span data-ttu-id="7a857-106">Bir veri dosyasını, virgülle ayrılmış değer dosya biçimi 'ne (. csv) Iş Ortağı Merkezi 'ne yükleyerek bir müşterinin hesabına tek seferde birden fazla kullanıcı ekleyin.</span><span class="sxs-lookup"><span data-stu-id="7a857-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="7a857-107">Müşteri kullanıcıları dosyasını oluşturun ve müşteri hesabına yükleyin</span><span class="sxs-lookup"><span data-stu-id="7a857-107">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="7a857-108">Yukarıda açıklanan verilerle bir virgülle ayrılmış değer (. csv) veri dosyası oluşturun.</span><span class="sxs-lookup"><span data-stu-id="7a857-108">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="7a857-109">Daha sonraki bir adımda bu dosyaya gözatabilmeniz için dosyayı kaydedin.</span><span class="sxs-lookup"><span data-stu-id="7a857-109">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="7a857-110">[Bir müşteri hesabı için birden çok kullanıcıyı içeri aktarmak üzere. csv dosyasına yönelik alanlara](file-customer-users.md)bakın.</span><span class="sxs-lookup"><span data-stu-id="7a857-110">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="7a857-111">Iş Ortağı Merkezi [panosunda](https://partner.microsoft.com/dashboard)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="7a857-111">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="7a857-112">Iş Ortağı Merkezi menüsünde **müşteriler**' i seçin ve listeden bir müşteri seçin.</span><span class="sxs-lookup"><span data-stu-id="7a857-112">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="7a857-113">Müşterinin **Kullanıcılar ve lisanslar** sekmesini seçin ve ardından **kullanıcıları karşıya yükle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="7a857-113">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="7a857-114">**Kullanıcı bilgilerini karşıya yükle** altında, **Araştır**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="7a857-114">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="7a857-115">Dosya seçicisinde veri dosyanızı seçin ve sonra **Aç**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="7a857-115">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="7a857-116">**Doğrula**'yı seçin.</span><span class="sxs-lookup"><span data-stu-id="7a857-116">Select **Validate**.</span></span>

    <span data-ttu-id="7a857-117">**Göz önünde**  Hesap oluşturma hatalarının çoğu, eksik bilgiler, hatalı biçimlendirilmiş veya yinelenen e-posta adresleri veya dosyadaki çok fazla kayıt da dahil olmak üzere veri dosyası sorunlarından kaynaklanır.</span><span class="sxs-lookup"><span data-stu-id="7a857-117">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="7a857-118">Iş Ortağı Merkezi dosyayı doğruladıktan sonra, yeni kullanıcıların coğrafi **konumunu** seçin.</span><span class="sxs-lookup"><span data-stu-id="7a857-118">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="7a857-119">**Kaydet**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="7a857-119">Select **Save**.</span></span>
10. <span data-ttu-id="7a857-120">Kullanıcılar için geçici parola bilgilerini indirin.</span><span class="sxs-lookup"><span data-stu-id="7a857-120">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="7a857-121">Daha sonra yapamayabilmeniz için dosyayı geçici parolalarla birlikte indirdiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="7a857-121">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="7a857-122">Yeni kullanıcıların yeni hesaplarının geçici parolasını kullanarak yeni hesaplarında oturum açması gerekir.</span><span class="sxs-lookup"><span data-stu-id="7a857-122">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="7a857-123">Yeni kullanıcılara, **Lisans ve hizmetleri kullanabilir** , otomatik olarak izinler atanır.</span><span class="sxs-lookup"><span data-stu-id="7a857-123">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

## <a name="next-steps"></a><span data-ttu-id="7a857-124">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="7a857-124">Next steps</span></span>

- [<span data-ttu-id="7a857-125">Iş Ortağı Merkezi 'nde müşterilere kendi ürünlerini veya hizmetlerini satın alma izni verin</span><span class="sxs-lookup"><span data-stu-id="7a857-125">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
