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
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/03/2020
ms.locfileid: "92531159"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="a1d58-103">Bir. csv dosyası oluşturarak müşteri hesabına birden çok kullanıcı ekleme</span><span class="sxs-lookup"><span data-stu-id="a1d58-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="a1d58-104">**Uygulama hedefi**</span><span class="sxs-lookup"><span data-stu-id="a1d58-104">**Applies to**</span></span>

- <span data-ttu-id="a1d58-105">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="a1d58-105">Partner Center</span></span>

<span data-ttu-id="a1d58-106">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="a1d58-106">**Appropriate roles**</span></span>

- <span data-ttu-id="a1d58-107">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="a1d58-107">Global admin</span></span>

<span data-ttu-id="a1d58-108">Bir veri dosyasını, virgülle ayrılmış değer dosya biçimi 'ne (. csv) Iş Ortağı Merkezi 'ne yükleyerek bir müşterinin hesabına tek seferde birden fazla kullanıcı ekleyin.</span><span class="sxs-lookup"><span data-stu-id="a1d58-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="a1d58-109">Ortak merkezinden bir örnek veri dosyası indirebilir ve ardından kullanım için düzenleyebilir veya aşağıda tanımlanan veri modelini kullanarak yeni bir veri dosyası oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a1d58-109">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="a1d58-110">Veri dosyası gereksinimleri</span><span class="sxs-lookup"><span data-stu-id="a1d58-110">Data file requirements</span></span>

<span data-ttu-id="a1d58-111">Toplu karşıya yükleme işlemini kullanarak bir müşterinin hesabına birden çok kullanıcı eklemek için aşağıdaki gereksinimleri karşılamanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="a1d58-111">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="a1d58-112">Müşteri hesabı için genel yönetici izinlerine sahip olmanız gerekir;</span><span class="sxs-lookup"><span data-stu-id="a1d58-112">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="a1d58-113">Her kullanıcının e-posta etki alanına (ler) eklenen benzersiz bir e-posta adresi olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="a1d58-113">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="a1d58-114">Tek seferde en fazla 100 kayıt yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a1d58-114">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="a1d58-115">100 'den fazla Kullanıcı eklemeniz gerekiyorsa, ek veri dosyaları oluşturun ve karşıya yükleyin.</span><span class="sxs-lookup"><span data-stu-id="a1d58-115">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="a1d58-116">Tüm kullanıcılar aynı coğrafi **konumda** olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="a1d58-116">All users must be in the same geographic **Location** .</span></span>
- <span data-ttu-id="a1d58-117">Yalnızca aşağıda açıklanan verileri girin.</span><span class="sxs-lookup"><span data-stu-id="a1d58-117">Enter only the data described below.</span></span> <span data-ttu-id="a1d58-118">Gereksiz veriler karşıya yüklemenin başarısız olmasına neden olur.</span><span class="sxs-lookup"><span data-stu-id="a1d58-118">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="a1d58-119">Veri dosyasına aşağıdaki verileri girin:</span><span class="sxs-lookup"><span data-stu-id="a1d58-119">Enter the following data in the data file:</span></span>

| <span data-ttu-id="a1d58-120">**Sütun adı**</span><span class="sxs-lookup"><span data-stu-id="a1d58-120">**Column name**</span></span> | <span data-ttu-id="a1d58-121">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="a1d58-121">**Description**</span></span>  | <span data-ttu-id="a1d58-122">**Sınırlama**</span><span class="sxs-lookup"><span data-stu-id="a1d58-122">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="a1d58-123">Ad</span><span class="sxs-lookup"><span data-stu-id="a1d58-123">First name</span></span>  | <span data-ttu-id="a1d58-124">Kullanıcının adı (isteğe bağlı alan)</span><span class="sxs-lookup"><span data-stu-id="a1d58-124">User's first name (optional field)</span></span>  | <span data-ttu-id="a1d58-125">50-karakter sınırı</span><span class="sxs-lookup"><span data-stu-id="a1d58-125">50-character limit</span></span>  |
| <span data-ttu-id="a1d58-126">Soyadı</span><span class="sxs-lookup"><span data-stu-id="a1d58-126">Last name</span></span>  | <span data-ttu-id="a1d58-127">Kullanıcının Soyadı (isteğe bağlı alan)</span><span class="sxs-lookup"><span data-stu-id="a1d58-127">User's last name (optional field)</span></span>  | <span data-ttu-id="a1d58-128">50-karakter sınırı</span><span class="sxs-lookup"><span data-stu-id="a1d58-128">50-character limit</span></span>  |
| <span data-ttu-id="a1d58-129">Görünen ad</span><span class="sxs-lookup"><span data-stu-id="a1d58-129">Display name</span></span>    | <span data-ttu-id="a1d58-130">Iş ortağı merkezinde (gerekli alan) görünen ad</span><span class="sxs-lookup"><span data-stu-id="a1d58-130">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="a1d58-131">50-karakter sınırı</span><span class="sxs-lookup"><span data-stu-id="a1d58-131">50-character limit</span></span>                         |
| <span data-ttu-id="a1d58-132">E-posta</span><span class="sxs-lookup"><span data-stu-id="a1d58-132">Email</span></span>   | <span data-ttu-id="a1d58-133">Müşteri şirketindeki kullanıcının iş e-posta adresi (gerekli alan)</span><span class="sxs-lookup"><span data-stu-id="a1d58-133">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="a1d58-134">Her kullanıcının benzersiz bir e-posta adresi olmalıdır</span><span class="sxs-lookup"><span data-stu-id="a1d58-134">Each user must have a unique email address</span></span> |
| <span data-ttu-id="a1d58-135">Durum güncelleştirmesi</span><span class="sxs-lookup"><span data-stu-id="a1d58-135">Status update</span></span>   | <span data-ttu-id="a1d58-136">Yeni Kullanıcı kaydının başarıyla oluşturulup oluşturulmayacağını göstermek için kullanılır</span><span class="sxs-lookup"><span data-stu-id="a1d58-136">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="a1d58-137">\*\*Boş bırakın\*\*</span><span class="sxs-lookup"><span data-stu-id="a1d58-137">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="a1d58-138">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="a1d58-138">Next steps</span></span>

- [<span data-ttu-id="a1d58-139">Bir müşteri için birden çok kullanıcı ekleme</span><span class="sxs-lookup"><span data-stu-id="a1d58-139">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)