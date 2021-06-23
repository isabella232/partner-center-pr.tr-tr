---
title: Azure AD hizmet sorumlusu
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure AD kiracınıza hizmet sorumlusu ekleme hakkında bilgi edinin. Bunun için azure ad uygulaması (hizmet sorumlusu) İş Ortağı Merkezi.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 3698032a632384e8416664c9564819d7c4da9c38
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551563"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="5c1ce-104">Azure AD uygulaması (hizmet sorumlusu) İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="5c1ce-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="5c1ce-105">**Uygun roller:** Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="5c1ce-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="5c1ce-106">İş Ortağı Merkezi'daki Ticari Market programında artık Microsoft Azure Active Directory (Azure AD) uygulamasını (hizmet sorumlusu) kullanıcı olarak İş Ortağı Merkezi.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-106">In the Commercial Marketplace program in Partner Center, you are now able to add a Microsoft Azure Active Directory (Azure AD) application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="5c1ce-107">(Daha önce Bulut İş Ortağı Portalı (CPP) hesabınızla bunu yapasınız.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-107">(You were able to do so previously in your Cloud Partner Portal (CPP) account.</span></span> <span data-ttu-id="5c1ce-108">İş Ortağı Merkezi'a geçiş İş Ortağı Merkezi CPP hesabı salt okunur olur.)</span><span class="sxs-lookup"><span data-stu-id="5c1ce-108">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="5c1ce-109">Hizmet sorumlusu, Azure AD uygulamasıyla eş anlamlıdır.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-109">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="5c1ce-110">Azure AD uygulaması ekleme (hizmet sorumlusu)</span><span class="sxs-lookup"><span data-stu-id="5c1ce-110">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="5c1ce-111">Panodan İş Ortağı Merkezi'yi ve **ardından** Geliştirici **ayarları'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="5c1ce-111">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="5c1ce-112">**Kullanıcılar'ı** ve ardından **Azure AD Uygulamaları Ekle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="5c1ce-112">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="5c1ce-113">Mevcut bir Azure AD uygulamasını seçin veya yeni bir uygulama oluşturun.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-113">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="5c1ce-114">Yeni bir Azure AD uygulaması sanız aşağıdaki bilgileri dahil edin:</span><span class="sxs-lookup"><span data-stu-id="5c1ce-114">If you create a new Azure AD application, include the following information:</span></span>  

   - <span data-ttu-id="5c1ce-115">**Yanıt URL'si:** Kullanıcıların Azure AD uygulamalarınızı kullanmak için oturum açmasını istediğiniz URL.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-115">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="5c1ce-116">**Uygulama Kimliği URI'si:** Azure AD'ye çoklu oturum açma isteği gönderdiği zaman sunulan Azure AD uygulaması için mantıksal tanımlayıcı.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-116">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="5c1ce-117">**Güvenlik rolleri:** Rol **Yöneticisi** (CPP'de 'Sahip' rolüyle aynı) ve **Geliştirici** (CPP'de 'Katkıda Bulunan' rolüyle aynı) İş Ortağı Merkezi'daki Ticari Market programı için geçerlidir ve bu Azure AD Uygulaması ile ilişkilendirilebilir.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-117">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="5c1ce-118">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="5c1ce-118">Next steps</span></span>

- [<span data-ttu-id="5c1ce-119">İş Ortağı Merkezi'da ticari markete genel bakış</span><span class="sxs-lookup"><span data-stu-id="5c1ce-119">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)