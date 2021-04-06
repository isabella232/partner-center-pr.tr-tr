---
title: Bir müşteri hesabı için birden çok kullanıcının içeri aktarılacağı. csv dosyası alanları
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bir müşteri hesabına birden çok kullanıcı eklemek için uygun alanlara sahip bir virgülle ayrılmış değer (. csv) dosyası oluşturun.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441430"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="4d501-103">Bir. csv dosyası oluşturarak müşteri hesabına birden çok kullanıcı ekleme</span><span class="sxs-lookup"><span data-stu-id="4d501-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="4d501-104">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="4d501-104">**Appropriate roles**</span></span>

- <span data-ttu-id="4d501-105">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="4d501-105">Global admin</span></span>

<span data-ttu-id="4d501-106">Bir veri dosyasını, virgülle ayrılmış değer dosya biçimi 'ne (. csv) Iş Ortağı Merkezi 'ne yükleyerek bir müşterinin hesabına tek seferde birden fazla kullanıcı ekleyin.</span><span class="sxs-lookup"><span data-stu-id="4d501-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="4d501-107">Ortak merkezinden bir örnek veri dosyası indirebilir ve ardından kullanım için düzenleyebilir veya aşağıda tanımlanan veri modelini kullanarak yeni bir veri dosyası oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4d501-107">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="4d501-108">Veri dosyası gereksinimleri</span><span class="sxs-lookup"><span data-stu-id="4d501-108">Data file requirements</span></span>

<span data-ttu-id="4d501-109">Toplu karşıya yükleme işlemini kullanarak bir müşterinin hesabına birden çok kullanıcı eklemek için aşağıdaki gereksinimleri karşılamanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="4d501-109">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="4d501-110">Müşteri hesabı için genel yönetici izinlerine sahip olmanız gerekir;</span><span class="sxs-lookup"><span data-stu-id="4d501-110">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="4d501-111">Her kullanıcının e-posta etki alanına (ler) eklenen benzersiz bir e-posta adresi olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="4d501-111">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="4d501-112">Tek seferde en fazla 100 kayıt yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4d501-112">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="4d501-113">100 'den fazla Kullanıcı eklemeniz gerekiyorsa, ek veri dosyaları oluşturun ve karşıya yükleyin.</span><span class="sxs-lookup"><span data-stu-id="4d501-113">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="4d501-114">Tüm kullanıcılar aynı coğrafi **konumda** olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="4d501-114">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="4d501-115">Yalnızca aşağıda açıklanan verileri girin.</span><span class="sxs-lookup"><span data-stu-id="4d501-115">Enter only the data described below.</span></span> <span data-ttu-id="4d501-116">Gereksiz veriler karşıya yüklemenin başarısız olmasına neden olur.</span><span class="sxs-lookup"><span data-stu-id="4d501-116">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="4d501-117">Veri dosyasına aşağıdaki verileri girin:</span><span class="sxs-lookup"><span data-stu-id="4d501-117">Enter the following data in the data file:</span></span>

| <span data-ttu-id="4d501-118">**Sütun adı**</span><span class="sxs-lookup"><span data-stu-id="4d501-118">**Column name**</span></span> | <span data-ttu-id="4d501-119">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="4d501-119">**Description**</span></span>  | <span data-ttu-id="4d501-120">**Sınırlama**</span><span class="sxs-lookup"><span data-stu-id="4d501-120">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="4d501-121">Ad</span><span class="sxs-lookup"><span data-stu-id="4d501-121">First name</span></span>  | <span data-ttu-id="4d501-122">Kullanıcının adı (isteğe bağlı alan)</span><span class="sxs-lookup"><span data-stu-id="4d501-122">User's first name (optional field)</span></span>  | <span data-ttu-id="4d501-123">50-karakter sınırı</span><span class="sxs-lookup"><span data-stu-id="4d501-123">50-character limit</span></span>  |
| <span data-ttu-id="4d501-124">Soyadı</span><span class="sxs-lookup"><span data-stu-id="4d501-124">Last name</span></span>  | <span data-ttu-id="4d501-125">Kullanıcının Soyadı (isteğe bağlı alan)</span><span class="sxs-lookup"><span data-stu-id="4d501-125">User's last name (optional field)</span></span>  | <span data-ttu-id="4d501-126">50-karakter sınırı</span><span class="sxs-lookup"><span data-stu-id="4d501-126">50-character limit</span></span>  |
| <span data-ttu-id="4d501-127">Görünen ad</span><span class="sxs-lookup"><span data-stu-id="4d501-127">Display name</span></span>    | <span data-ttu-id="4d501-128">Iş ortağı merkezinde (gerekli alan) görünen ad</span><span class="sxs-lookup"><span data-stu-id="4d501-128">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="4d501-129">50-karakter sınırı</span><span class="sxs-lookup"><span data-stu-id="4d501-129">50-character limit</span></span>                         |
| <span data-ttu-id="4d501-130">E-posta</span><span class="sxs-lookup"><span data-stu-id="4d501-130">Email</span></span>   | <span data-ttu-id="4d501-131">Müşteri şirketindeki kullanıcının iş e-posta adresi (gerekli alan)</span><span class="sxs-lookup"><span data-stu-id="4d501-131">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="4d501-132">Her kullanıcının benzersiz bir e-posta adresi olmalıdır</span><span class="sxs-lookup"><span data-stu-id="4d501-132">Each user must have a unique email address</span></span> |
| <span data-ttu-id="4d501-133">Durum güncelleştirmesi</span><span class="sxs-lookup"><span data-stu-id="4d501-133">Status update</span></span>   | <span data-ttu-id="4d501-134">Yeni Kullanıcı kaydının başarıyla oluşturulup oluşturulmayacağını göstermek için kullanılır</span><span class="sxs-lookup"><span data-stu-id="4d501-134">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="4d501-135">\*\*Boş bırakın\*\*</span><span class="sxs-lookup"><span data-stu-id="4d501-135">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="4d501-136">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="4d501-136">Next steps</span></span>

- [<span data-ttu-id="4d501-137">Bir müşteri için birden çok kullanıcı ekleme</span><span class="sxs-lookup"><span data-stu-id="4d501-137">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)