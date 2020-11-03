---
title: Azure AD hizmet sorumlusu
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure AD kiracınıza hizmet sorumlusu ekleme hakkında bilgi edinin. Bunun yapılması, Iş Ortağı Merkezi 'ne bir Azure AD uygulaması (hizmet sorumlusu) ekleme anlamına gelir.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 21ef2aaa46359570bbf13c12c5fb6c1f5eab080a
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2020
ms.locfileid: "92531218"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="8fd44-104">Iş Ortağı Merkezi 'ne bir Azure AD uygulaması (hizmet sorumlusu) ekleme</span><span class="sxs-lookup"><span data-stu-id="8fd44-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="8fd44-105">**Uygulama hedefi**</span><span class="sxs-lookup"><span data-stu-id="8fd44-105">**Applies to**</span></span>

- <span data-ttu-id="8fd44-106">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="8fd44-106">Partner Center</span></span>

<span data-ttu-id="8fd44-107">**Uygun roller**</span><span class="sxs-lookup"><span data-stu-id="8fd44-107">**Appropriate roles**</span></span>

- <span data-ttu-id="8fd44-108">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="8fd44-108">Global admin</span></span>

<span data-ttu-id="8fd44-109">Iş Ortağı Merkezi 'ndeki ticari Market programında artık Iş Ortağı Merkezi hesabınıza bir kullanıcı olarak bir Azure AD uygulaması (hizmet sorumlusu) ekleyebileceksiniz.</span><span class="sxs-lookup"><span data-stu-id="8fd44-109">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="8fd44-110">(Bunu daha önce Bulut İş Ortağı Portalı veya CPP, hesabınızda de yapabileceksiniz.</span><span class="sxs-lookup"><span data-stu-id="8fd44-110">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="8fd44-111">Artık Iş Ortağı Merkezi 'ne geçirdiniz, CPP hesabı salt okunurdur.)</span><span class="sxs-lookup"><span data-stu-id="8fd44-111">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="8fd44-112">Hizmet sorumlusu, Azure AD uygulaması ile eşanlamlıdır.</span><span class="sxs-lookup"><span data-stu-id="8fd44-112">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="8fd44-113">Azure AD uygulaması ekleme (hizmet sorumlusu)</span><span class="sxs-lookup"><span data-stu-id="8fd44-113">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="8fd44-114">Iş Ortağı Merkezi panosundan **Ayarlar** ' ı seçin ve ardından **Geliştirici ayarları** ' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="8fd44-114">From the Partner Center dashboard, select **Settings** and then select **Developer settings** .</span></span>

2. <span data-ttu-id="8fd44-115">**Kullanıcıları** seçin ve ardından **Azure AD uygulamaları Ekle** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="8fd44-115">Select **Users** and then select **Add Azure AD Applications** .</span></span>

3. <span data-ttu-id="8fd44-116">Mevcut bir Azure AD uygulaması seçin veya yeni bir tane oluşturun.</span><span class="sxs-lookup"><span data-stu-id="8fd44-116">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="8fd44-117">Yeni bir Azure AD uygulaması oluşturursanız, aşağıdaki bilgileri ekleyin:</span><span class="sxs-lookup"><span data-stu-id="8fd44-117">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="8fd44-118">**Yanıt URL 'si** : KULLANıCıLARıN Azure AD uygulamanızı kullanmak için oturum açabilecekleri URL.</span><span class="sxs-lookup"><span data-stu-id="8fd44-118">**Reply URL** : The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="8fd44-119">**Uygulama kimliği URI 'si** : Azure AD 'ye yönelik çoklu oturum açma isteği gönderdiğinde sunulan Azure AD uygulaması için mantıksal tanımlayıcı.</span><span class="sxs-lookup"><span data-stu-id="8fd44-119">**App ID URI** : A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="8fd44-120">**Güvenlik rolleri** : roller **Yöneticisi** (cpp ' deki ' Owner ' rolüyle aynı) ve **Geliştirici** (cpp ' de ' katkıda bulunan ' rolüyle aynı), iş ortağı merkezi 'nde ticari Market programına uygulanır ve bu Azure AD uygulamasıyla ilişkilendirilebilir.</span><span class="sxs-lookup"><span data-stu-id="8fd44-120">**Security roles** : The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="8fd44-121">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="8fd44-121">Next steps</span></span>

- [<span data-ttu-id="8fd44-122">Iş Ortağı Merkezi 'nde ticari Market 'e genel bakış</span><span class="sxs-lookup"><span data-stu-id="8fd44-122">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)