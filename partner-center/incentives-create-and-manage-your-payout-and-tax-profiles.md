---
title: İş Ortağı Merkezi'ndeki ödeme ve vergi profilleri
ms.topic: how-to
ms.date: 11/12/2020
description: Teşvikleri çalışmanız için ödeme yapabilmeniz için ödeme ve vergi profilinizi oluşturun ve yönetin. Farklı profillerin oluşturulmasını, yönetilmesini ve kullanılmasını içerir.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 282fdacc8689ff71e885a2f0ea01ce9570611707
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624247"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="933a3-104">Iş Ortağı Merkezi 'nde teşvikleri ödeme ve vergi profilleri oluşturma ve yönetme</span><span class="sxs-lookup"><span data-stu-id="933a3-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>


<span data-ttu-id="933a3-105">**Uygun roller:**</span><span class="sxs-lookup"><span data-stu-id="933a3-105">**Appropriate roles:**</span></span>

- <span data-ttu-id="933a3-106">Teşvikleri Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="933a3-106">Incentives admin</span></span>
- <span data-ttu-id="933a3-107">Hesap yöneticisi</span><span class="sxs-lookup"><span data-stu-id="933a3-107">Account admin</span></span>
- <span data-ttu-id="933a3-108">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="933a3-108">Global admin</span></span>

<span data-ttu-id="933a3-109">Belirli bir MPN konumuna ilişkin teşvik programlarınızda ödeme alabilmeniz için önce geçerli bir ödeme ve vergi profilini programla ve MPN konumuyla ilişkilendirerek kaydınızı tamamlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="933a3-109">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="933a3-110">Microsoft ödemeleri yapmak için bu ödeme ve vergi profilini kullanacaktır.</span><span class="sxs-lookup"><span data-stu-id="933a3-110">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="933a3-111">Teşvik programının kurallarına bağlı olarak ödeme için elektronik banka transferi veya alacak dekontu kullanmanıza izin verilebilir.</span><span class="sxs-lookup"><span data-stu-id="933a3-111">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="933a3-112">Roller, para birimleri ve diğer Microsoft programları</span><span class="sxs-lookup"><span data-stu-id="933a3-112">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="933a3-113">Ödeme ve vergi profiliniz ile çalışmaya başlamadan önce aşağıdaki bilgileri anlamanız önemlidir.</span><span class="sxs-lookup"><span data-stu-id="933a3-113">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="933a3-114">Roller ve izinler</span><span class="sxs-lookup"><span data-stu-id="933a3-114">Roles and permissions</span></span>

<span data-ttu-id="933a3-115">Teşvik ödemeleri için banka ve vergi bilgilerini girmek üzere bir teşvikleri yöneticisi olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="933a3-115">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="933a3-116">MPN/Account yöneticisiyseniz, kendinizi ve/veya iş arkadaşını teşvikleri Yöneticisi olacak şekilde atayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="933a3-116">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="933a3-117">Teşvikleri yönetici izinleri istemeniz gerekiyorsa MPN yöneticinizle veya genel yöneticinizle iletişime geçin. [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açarak şirketinizde kimlerin bu rolleri olduğunu bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="933a3-117">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="933a3-118">Sağ üst köşedeki **Ayarlar** simgesinden **Kullanıcı yönetimi** ' ni seçin ve ardından Genel yönetici ' ye filtre uygulayın.</span><span class="sxs-lookup"><span data-stu-id="933a3-118">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="933a3-119">Teşvikleri kullanıcılar, teşvik kazanç ve ödeme ayrıntılarını ve raporlarını görüntüleyebilir, ancak banka ve vergi ayrıntılarını düzenleyemez.</span><span class="sxs-lookup"><span data-stu-id="933a3-119">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="933a3-120">Tediye para birimini seçin</span><span class="sxs-lookup"><span data-stu-id="933a3-120">Choose your disbursement currency</span></span>

<span data-ttu-id="933a3-121">Ödemeler, ödeme profilinizi ayarlarken seçtiğiniz para birimiyle yapılır.</span><span class="sxs-lookup"><span data-stu-id="933a3-121">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="933a3-122">Ödemeler, Microsoft tarafından aylık olarak ayarlanan bir döviz kuru kullanılarak hesaplanır.</span><span class="sxs-lookup"><span data-stu-id="933a3-122">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="933a3-123">Seçilen para birimi nedeniyle, değerde yapılan değişikliklerden sorumlu olacaksınız.</span><span class="sxs-lookup"><span data-stu-id="933a3-123">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="933a3-124">Farklı Microsoft programları için farklı profiller kullanma</span><span class="sxs-lookup"><span data-stu-id="933a3-124">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="933a3-125">Şirketiniz birden çok teşvik programında kaydedildiyse, hepsi için aynı ödeme hesabını kullanabilir veya farklı programlar için farklı ödeme hesapları kullanmayı tercih edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="933a3-125">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="933a3-126">Iş Ortağı Merkezi 'nde ödeme ve vergi profilleri oluşturma ve yönetme</span><span class="sxs-lookup"><span data-stu-id="933a3-126">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="933a3-127">Aşağıdaki bölümler, Iş Ortağı Merkezi 'nde ödeme ve vergi profilleri oluşturma ve yönetme sürecinde size yol gösterecektir.</span><span class="sxs-lookup"><span data-stu-id="933a3-127">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="933a3-128">Iş Ortağı Merkezi 'nde ödeme profilleri oluşturmak veya yönetmek için bir teşvik yöneticisi olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="933a3-128">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="933a3-129">Her bir teşvik programı altındaki her bir MPN konumuna bir rol atanması gerekir.</span><span class="sxs-lookup"><span data-stu-id="933a3-129">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="933a3-130">Iş Ortağı Merkezi 'ne teşvik yöneticileri ekleme hakkında daha fazla bilgi için bkz. [Kullanıcı hesapları oluşturma](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="933a3-130">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="933a3-131">Iş Ortağı Merkezi 'nde ödeme ve vergi kısmına erişin</span><span class="sxs-lookup"><span data-stu-id="933a3-131">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="933a3-132">Azure Active Directory (Azure AD) hesabınızı (Şirket hesabı) veya atanmış bir e-posta adresini kullanarak [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="933a3-132">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="933a3-133">Birden çok etki alanı, bir Azure AD hesabında kaydedilebilir.</span><span class="sxs-lookup"><span data-stu-id="933a3-133">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="933a3-134">Hangi etki alanlarının ilişkilendirildiğini öğrenmek için genel yöneticinizle iletişime geçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-134">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="933a3-135">Yalnızca etki alanı ile oturum açabiliyor @onmicrosoft.com , Azure AD hesabına ek etki alanları eklemek Için hesap yöneticinize başvurun.</span><span class="sxs-lookup"><span data-stu-id="933a3-135">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="933a3-136">**İş veya okul hesabı** ya da **kişisel hesap**' i seçmeniz istenirse **iş veya okul hesabı**' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-136">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="933a3-137">Dişli simgesini seçerek **Ayarlar** menüsünü açın ve **Hesap ayarları**' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-137">Select the gear icon to open the **Settings** menu, and then select **Account settings**.</span></span>

3. <span data-ttu-id="933a3-138">**Hesap ayarları** menüsünde, **ödeme ve vergi**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-138">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="933a3-139">Ayrı programlara ödeme ve vergi profilleri atama</span><span class="sxs-lookup"><span data-stu-id="933a3-139">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="933a3-140">[Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açın ve sonra da dişli simgesini seçerek **Ayarlar** menüsünü açın.</span><span class="sxs-lookup"><span data-stu-id="933a3-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="933a3-141">**Hesap ayarları**' nı seçin, **ödeme ve vergi bölümünü** genişletin ve ardından **ödeme ve vergi profili ataması**' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-141">Select **Account settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="933a3-142">Programlarınızın bir listesi görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="933a3-142">A list of your programs will be displayed.</span></span> <span data-ttu-id="933a3-143">Profil ayrıntılarını görmek için bir programın yanındaki oku seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-143">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="933a3-144">**Vergi profili** açılan menüsünde istediğiniz vergi profilini seçin veya yeni bir profil oluşturma seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="933a3-144">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="933a3-145">Yeni bir profil oluşturma seçeneğini belirlediğinizde uygun şekilde yeniden yönlendirilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="933a3-145">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="933a3-146">Açılır pencerede devam ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-146">Select Continue in the pop-up window.</span></span> <span data-ttu-id="933a3-147">Yeni bir vergi profili oluşturma işlemi aşağıda verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="933a3-147">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="933a3-148">**Ödeme yöntemini** seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-148">Select **Payment method**.</span></span>

   - <span data-ttu-id="933a3-149">Ödeme yönteminiz olarak **elektronik banka aktarımı** ' nı seçtiyseniz, istediğiniz ödeme profilini seçin veya yeni bir profil oluşturma seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="933a3-149">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="933a3-150">Yeni bir profil oluşturma seçeneğini belirlediğinizde uygun şekilde yeniden yönlendirilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="933a3-150">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="933a3-151">Açılır pencerede devam ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-151">Select Continue in the pop-up window.</span></span> <span data-ttu-id="933a3-152">Yeni bir ödeme profili oluşturma işlemi aşağıda verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="933a3-152">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="933a3-153">Ödeme yönteminiz olarak **kredi dekontunu** seçtiyseniz doğrulamayı tamamlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="933a3-153">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="933a3-154">Bu, başvurulan SAP numarasının kuruluşunuza ait olduğunu onaylar.</span><span class="sxs-lookup"><span data-stu-id="933a3-154">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="933a3-155">Listelenen birden fazla Microsoft iş varlığı varsa, her varlık için bir ödeme profili seçmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="933a3-155">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="933a3-156">Ödeme yöntemi kullanılabilirliği, teşvik programının kurallarına bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="933a3-156">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="933a3-157">**Para birimini** seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-157">Select the **Currency**.</span></span>

6. <span data-ttu-id="933a3-158">Ödeme alanlarını tamamladıktan sonra **Gönder**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-158">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="933a3-159">Banka profilinizi oluşturma</span><span class="sxs-lookup"><span data-stu-id="933a3-159">Create your bank profile</span></span>

<span data-ttu-id="933a3-160">Banka profilleri bir kuruluş düzeyinde oluşturulur.</span><span class="sxs-lookup"><span data-stu-id="933a3-160">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="933a3-161">Bu, bir banka profilinin bir kuruluştaki birden fazla MPN KIMLIĞI ile atanmasını ve bu programları teşvik etmesine olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="933a3-161">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="933a3-162">Farklı bankacılık ve vergi kuralları uygulanabildiği için bankacılık profili farklı ülkelere uygulanırken özel durumlar olabilir.</span><span class="sxs-lookup"><span data-stu-id="933a3-162">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="933a3-163">Aşağıdaki sayfalarda, yıldız işareti olan alanlar gereklidir.</span><span class="sxs-lookup"><span data-stu-id="933a3-163">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="933a3-164">Bir alanın ne olduğunu bilmiyorsanız, bilgi simgesini seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-164">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="933a3-165">**Ayrıntılar** sayfasında, şu alanları doldurun: **profil adı:** bu ödeme profilini tanımlamak için benzersiz bir ad girin.</span><span class="sxs-lookup"><span data-stu-id="933a3-165">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="933a3-166">**Banka hesabı konumu:** Şirketinizin bankasının bulunduğu ülke.</span><span class="sxs-lookup"><span data-stu-id="933a3-166">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="933a3-167">**Ödeme yöntemi:** Iş Ortağı Merkezi için tercih edilen ödeme yöntemi elektronik banka aktarmasıdır.</span><span class="sxs-lookup"><span data-stu-id="933a3-167">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="933a3-168">**İleri**’yi seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-168">Select **Next**.</span></span>

3. <span data-ttu-id="933a3-169">**Banka hesabı** sayfasında, bilgilerinizi girin.</span><span class="sxs-lookup"><span data-stu-id="933a3-169">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="933a3-170">Bu sayfada gösterilen alanlar ülkeye göre farklılık gösterecektir.</span><span class="sxs-lookup"><span data-stu-id="933a3-170">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="933a3-171">**İleri**’yi seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-171">Select **Next**.</span></span>

5. <span data-ttu-id="933a3-172">**Lehdar** sayfasında, ilgili bilgileri girin.</span><span class="sxs-lookup"><span data-stu-id="933a3-172">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="933a3-173">Lehdar, şirketinizdeki kişiden, hesabınızı tartışmaları gerektiğinde bankanın iletişim kurabildikleri kişidir.</span><span class="sxs-lookup"><span data-stu-id="933a3-173">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="933a3-174">Alanlar tamamlandığında, **son**' u seçin ve ardından banka profilinizi oluşturmak için **Onayla** ' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-174">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="933a3-175">**Ödeme ve vergi profilleri** sayfasına yönlendirilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="933a3-175">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="933a3-176">Yeni profilinizin durumu, doğrulama tamamlanana kadar **bekleyen Microsoft doğrulamasını** yansıtır.</span><span class="sxs-lookup"><span data-stu-id="933a3-176">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="933a3-177">Bu işlem, 48 saate kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="933a3-177">This process may take up to 48 hours.</span></span> <span data-ttu-id="933a3-178">Doğrulama tamamlandıktan sonra, profil durumunuz **onaylanan** veya **eylem gereken eylemi** yansıtır.</span><span class="sxs-lookup"><span data-stu-id="933a3-178">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="933a3-179">**Eylem gerekliyse**, gerekli bilgileri sağlamak için yukarıdaki adımları tekrarlayın.</span><span class="sxs-lookup"><span data-stu-id="933a3-179">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="933a3-180">Vergi profilinizi oluşturma</span><span class="sxs-lookup"><span data-stu-id="933a3-180">Create your tax profile</span></span>

<span data-ttu-id="933a3-181">Microsoft 'un kuruluşunuz için gereken vergi bilgilerini sağlamak için aşağıdaki yordamı kullanın.</span><span class="sxs-lookup"><span data-stu-id="933a3-181">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="933a3-182">Bu bölümdeki sayfalar dinamiktir ve ülkeniz ya da bölgenize göre değişir.</span><span class="sxs-lookup"><span data-stu-id="933a3-182">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="933a3-183">Doğru vergi bilgilerini tanımlamaya yönelik yardıma ihtiyacınız varsa, ülkenizde uygun kamu kaynaklarıyla iletişim kurun.</span><span class="sxs-lookup"><span data-stu-id="933a3-183">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="933a3-184">Kuzey iş ortağı şirketleri için, W8 veya W9 formlarını tamamlamada bilgi almanız gerekiyorsa, aşağıdaki adresler size ıRS sitesine götürür:</span><span class="sxs-lookup"><span data-stu-id="933a3-184">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="933a3-185">Şirketiniz için yalnızca ayrıntıları girin.</span><span class="sxs-lookup"><span data-stu-id="933a3-185">Enter only details for your company.</span></span> <span data-ttu-id="933a3-186">Kişisel ayrıntıları hiçbir şekilde girmeyin.</span><span class="sxs-lookup"><span data-stu-id="933a3-186">Never enter personal details.</span></span>

1. <span data-ttu-id="933a3-187">**Iş profili** sayfasında, gerekli alanları tamamlayıp **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-187">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="933a3-188">**Kurulum** sayfasında, şirketiniz için geçerli olan seçeneği belirleyin.</span><span class="sxs-lookup"><span data-stu-id="933a3-188">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="933a3-189">Şirketiniz yalnızca Birleşik Devletler veya bu profil bir bireyin varsa, sol taraftaki seçeneği belirleyin.</span><span class="sxs-lookup"><span data-stu-id="933a3-189">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="933a3-190">Şirketinizin Birleşik Devletler dışına dahil olması durumunda sağ taraftaki seçeneği seçin ve ardından listeden bulunduğunuz ülkeyi/bölgenizi seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-190">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="933a3-191">**İleri**’yi seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-191">Select **Next**.</span></span> 

4. <span data-ttu-id="933a3-192">**Vergi durumu** sayfasında, gerekli bilgileri girin ve ardından **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-192">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="933a3-193">Bu sayfadaki alanlar ülkeye göre değişiklik gösterecektir.</span><span class="sxs-lookup"><span data-stu-id="933a3-193">Fields on this page will vary by country.</span></span> <span data-ttu-id="933a3-194">ayrıntılarınız.</span><span class="sxs-lookup"><span data-stu-id="933a3-194">your details.</span></span> 

5. <span data-ttu-id="933a3-195">**Ek belgeler** sayfasında gerekli alanlar ' ı seçin ve **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-195">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="933a3-196">Ülkeniz veya bölgeniz için gereken tüm belgeleri karşıya yüklemek için **Araştır** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-196">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="933a3-197">Belge adı gösterildiğinde **karşıya yükle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-197">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="933a3-198">Belgeyi kaldırmanız gerekirse **Kaldır**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-198">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="933a3-199">Kaydetmek ve devam etmek için **son**' u seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-199">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="933a3-200">Açılan iletide **Onayla** ' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="933a3-200">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="933a3-201">**Ödeme ve vergi kurulumu** sayfasına geri yönlendirilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="933a3-201">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="933a3-202">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="933a3-202">Next steps</span></span>

- [<span data-ttu-id="933a3-203">Ödemeler ve vergiler hakkında sık sorulan sorular</span><span class="sxs-lookup"><span data-stu-id="933a3-203">Common questions about payouts and taxes</span></span>](payout-faq.md)
