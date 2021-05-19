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
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150990"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="5c65c-103">Bir. csv dosyası oluşturarak müşteri hesabına birden çok kullanıcı ekleme</span><span class="sxs-lookup"><span data-stu-id="5c65c-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="5c65c-104">**Uygun roller**: genel yönetici</span><span class="sxs-lookup"><span data-stu-id="5c65c-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="5c65c-105">Bir veri dosyasını, virgülle ayrılmış değer dosya biçimi 'ne (. csv) Iş Ortağı Merkezi 'ne yükleyerek bir müşterinin hesabına tek seferde birden fazla kullanıcı ekleyin.</span><span class="sxs-lookup"><span data-stu-id="5c65c-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="5c65c-106">Ortak merkezinden bir örnek veri dosyası indirebilir ve ardından kullanım için düzenleyebilir veya aşağıda tanımlanan veri modelini kullanarak yeni bir veri dosyası oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5c65c-106">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="5c65c-107">Veri dosyası gereksinimleri</span><span class="sxs-lookup"><span data-stu-id="5c65c-107">Data file requirements</span></span>

<span data-ttu-id="5c65c-108">Toplu karşıya yükleme işlemini kullanarak bir müşterinin hesabına birden çok kullanıcı eklemek için aşağıdaki gereksinimleri karşılamanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="5c65c-108">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="5c65c-109">Müşteri hesabı için genel yönetici izinlerine sahip olmanız gerekir;</span><span class="sxs-lookup"><span data-stu-id="5c65c-109">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="5c65c-110">Her kullanıcının e-posta etki alanına (ler) eklenen benzersiz bir e-posta adresi olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="5c65c-110">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="5c65c-111">Tek seferde en fazla 100 kayıt yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5c65c-111">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="5c65c-112">100 'den fazla Kullanıcı eklemeniz gerekiyorsa, ek veri dosyaları oluşturun ve karşıya yükleyin.</span><span class="sxs-lookup"><span data-stu-id="5c65c-112">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="5c65c-113">Tüm kullanıcılar aynı coğrafi **konumda** olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="5c65c-113">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="5c65c-114">Yalnızca aşağıda açıklanan verileri girin.</span><span class="sxs-lookup"><span data-stu-id="5c65c-114">Enter only the data described below.</span></span> <span data-ttu-id="5c65c-115">Gereksiz veriler karşıya yüklemenin başarısız olmasına neden olur.</span><span class="sxs-lookup"><span data-stu-id="5c65c-115">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="5c65c-116">Veri dosyasına aşağıdaki verileri girin:</span><span class="sxs-lookup"><span data-stu-id="5c65c-116">Enter the following data in the data file:</span></span>

| <span data-ttu-id="5c65c-117">**Sütun adı**</span><span class="sxs-lookup"><span data-stu-id="5c65c-117">**Column name**</span></span> | <span data-ttu-id="5c65c-118">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="5c65c-118">**Description**</span></span>  | <span data-ttu-id="5c65c-119">**Sınırlama**</span><span class="sxs-lookup"><span data-stu-id="5c65c-119">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="5c65c-120">Ad</span><span class="sxs-lookup"><span data-stu-id="5c65c-120">First name</span></span>  | <span data-ttu-id="5c65c-121">Kullanıcının adı (isteğe bağlı alan)</span><span class="sxs-lookup"><span data-stu-id="5c65c-121">User's first name (optional field)</span></span>  | <span data-ttu-id="5c65c-122">50-karakter sınırı</span><span class="sxs-lookup"><span data-stu-id="5c65c-122">50-character limit</span></span>  |
| <span data-ttu-id="5c65c-123">Soyadı</span><span class="sxs-lookup"><span data-stu-id="5c65c-123">Last name</span></span>  | <span data-ttu-id="5c65c-124">Kullanıcının Soyadı (isteğe bağlı alan)</span><span class="sxs-lookup"><span data-stu-id="5c65c-124">User's last name (optional field)</span></span>  | <span data-ttu-id="5c65c-125">50-karakter sınırı</span><span class="sxs-lookup"><span data-stu-id="5c65c-125">50-character limit</span></span>  |
| <span data-ttu-id="5c65c-126">Görünen ad</span><span class="sxs-lookup"><span data-stu-id="5c65c-126">Display name</span></span>    | <span data-ttu-id="5c65c-127">Ad, İş Ortağı Merkezi (gerekli alan)</span><span class="sxs-lookup"><span data-stu-id="5c65c-127">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="5c65c-128">50 karakterlik sınır</span><span class="sxs-lookup"><span data-stu-id="5c65c-128">50-character limit</span></span>                         |
| <span data-ttu-id="5c65c-129">E-posta</span><span class="sxs-lookup"><span data-stu-id="5c65c-129">Email</span></span>   | <span data-ttu-id="5c65c-130">Müşterinin müşteri şirketinde iş e-posta adresi (gerekli alan)</span><span class="sxs-lookup"><span data-stu-id="5c65c-130">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="5c65c-131">Her kullanıcının benzersiz bir e-posta adresi olmalıdır</span><span class="sxs-lookup"><span data-stu-id="5c65c-131">Each user must have a unique email address</span></span> |
| <span data-ttu-id="5c65c-132">Durum güncelleştirmesi</span><span class="sxs-lookup"><span data-stu-id="5c65c-132">Status update</span></span>   | <span data-ttu-id="5c65c-133">Yeni kullanıcı kaydının başarıyla oluşturulıp oluşturula olmadığını belirtmek için kullanılır</span><span class="sxs-lookup"><span data-stu-id="5c65c-133">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="5c65c-134">\*\*Boş bırakın\*\*</span><span class="sxs-lookup"><span data-stu-id="5c65c-134">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="5c65c-135">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="5c65c-135">Next steps</span></span>

- [<span data-ttu-id="5c65c-136">Bir müşteri için birden çok kullanıcı ekleme</span><span class="sxs-lookup"><span data-stu-id="5c65c-136">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)