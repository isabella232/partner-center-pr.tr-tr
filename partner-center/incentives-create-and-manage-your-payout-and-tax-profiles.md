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
ms.openlocfilehash: 1e97e2e9db798e5ef90858cf96dc06602bbfe427
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492475"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="edfdf-104">Iş Ortağı Merkezi 'nde teşvikleri ödeme ve vergi profilleri oluşturma ve yönetme</span><span class="sxs-lookup"><span data-stu-id="edfdf-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="edfdf-105">**Uygulama hedefi:**</span><span class="sxs-lookup"><span data-stu-id="edfdf-105">**Applies to:**</span></span>

- <span data-ttu-id="edfdf-106">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="edfdf-106">Partner Center</span></span>

<span data-ttu-id="edfdf-107">**Uygun roller:**</span><span class="sxs-lookup"><span data-stu-id="edfdf-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="edfdf-108">Teşvikleri Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="edfdf-108">Incentives admin</span></span>
- <span data-ttu-id="edfdf-109">Hesap yöneticisi</span><span class="sxs-lookup"><span data-stu-id="edfdf-109">Account admin</span></span>
- <span data-ttu-id="edfdf-110">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="edfdf-110">Global admin</span></span>

<span data-ttu-id="edfdf-111">Belirli bir MPN konumuna ilişkin teşvik programlarınızda ödeme alabilmeniz için önce geçerli bir ödeme ve vergi profilini programla ve MPN konumuyla ilişkilendirerek kaydınızı tamamlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-111">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="edfdf-112">Microsoft ödemeleri yapmak için bu ödeme ve vergi profilini kullanacaktır.</span><span class="sxs-lookup"><span data-stu-id="edfdf-112">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="edfdf-113">Teşvik programının kurallarına bağlı olarak ödeme için elektronik banka transferi veya alacak dekontu kullanmanıza izin verilebilir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-113">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="edfdf-114">Roller, para birimleri ve diğer Microsoft programları</span><span class="sxs-lookup"><span data-stu-id="edfdf-114">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="edfdf-115">Ödeme ve vergi profiliniz ile çalışmaya başlamadan önce aşağıdaki bilgileri anlamanız önemlidir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-115">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="edfdf-116">Roller ve izinler</span><span class="sxs-lookup"><span data-stu-id="edfdf-116">Roles and permissions</span></span>

<span data-ttu-id="edfdf-117">Teşvik ödemeleri için banka ve vergi bilgilerini girmek üzere bir teşvikleri yöneticisi olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-117">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="edfdf-118">MPN/Account yöneticisiyseniz, kendinizi ve/veya iş arkadaşını teşvikleri Yöneticisi olacak şekilde atayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="edfdf-118">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="edfdf-119">Teşvikleri yönetici izinleri istemeniz gerekiyorsa MPN yöneticinizle veya genel yöneticinizle iletişime geçin. [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açarak şirketinizde kimlerin bu rolleri olduğunu bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="edfdf-119">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="edfdf-120">Sağ üst köşedeki **Ayarlar** simgesinden **Kullanıcı yönetimi** ' ni seçin ve ardından Genel yönetici ' ye filtre uygulayın.</span><span class="sxs-lookup"><span data-stu-id="edfdf-120">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="edfdf-121">Teşvikleri kullanıcılar, teşvik kazanç ve ödeme ayrıntılarını ve raporlarını görüntüleyebilir, ancak banka ve vergi ayrıntılarını düzenleyemez.</span><span class="sxs-lookup"><span data-stu-id="edfdf-121">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="edfdf-122">Tediye para birimini seçin</span><span class="sxs-lookup"><span data-stu-id="edfdf-122">Choose your disbursement currency</span></span>

<span data-ttu-id="edfdf-123">Ödemeler, ödeme profilinizi ayarlarken seçtiğiniz para birimiyle yapılır.</span><span class="sxs-lookup"><span data-stu-id="edfdf-123">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="edfdf-124">Ödemeler, Microsoft tarafından aylık olarak ayarlanan bir döviz kuru kullanılarak hesaplanır.</span><span class="sxs-lookup"><span data-stu-id="edfdf-124">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="edfdf-125">Seçilen para birimi nedeniyle, değerde yapılan değişikliklerden sorumlu olacaksınız.</span><span class="sxs-lookup"><span data-stu-id="edfdf-125">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="edfdf-126">Farklı Microsoft programları için farklı profiller kullanma</span><span class="sxs-lookup"><span data-stu-id="edfdf-126">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="edfdf-127">Şirketiniz birden çok teşvik programında kaydedildiyse, hepsi için aynı ödeme hesabını kullanabilir veya farklı programlar için farklı ödeme hesapları kullanmayı tercih edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="edfdf-127">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="edfdf-128">Iş Ortağı Merkezi 'nde ödeme ve vergi profilleri oluşturma ve yönetme</span><span class="sxs-lookup"><span data-stu-id="edfdf-128">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="edfdf-129">Aşağıdaki bölümler, Iş Ortağı Merkezi 'nde ödeme ve vergi profilleri oluşturma ve yönetme sürecinde size yol gösterecektir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-129">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="edfdf-130">Iş Ortağı Merkezi 'nde ödeme profilleri oluşturmak veya yönetmek için bir teşvik yöneticisi olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-130">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="edfdf-131">Her bir teşvik programı altındaki her bir MPN konumuna bir rol atanması gerekir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-131">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="edfdf-132">Iş Ortağı Merkezi 'ne teşvik yöneticileri ekleme hakkında daha fazla bilgi için bkz. [Kullanıcı hesapları oluşturma](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="edfdf-132">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="edfdf-133">Iş Ortağı Merkezi 'nde ödeme ve vergi kısmına erişin</span><span class="sxs-lookup"><span data-stu-id="edfdf-133">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="edfdf-134">Azure Active Directory (Azure AD) hesabınızı (Şirket hesabı) veya atanmış bir e-posta adresini kullanarak [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="edfdf-134">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="edfdf-135">Birden çok etki alanı, bir Azure AD hesabında kaydedilebilir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-135">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="edfdf-136">Hangi etki alanlarının ilişkilendirildiğini öğrenmek için genel yöneticinizle iletişime geçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-136">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="edfdf-137">Yalnızca etki alanı ile oturum açabiliyor @onmicrosoft.com , Azure AD hesabına ek etki alanları eklemek Için hesap yöneticinize başvurun.</span><span class="sxs-lookup"><span data-stu-id="edfdf-137">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="edfdf-138">**İş veya okul hesabı** ya da **kişisel hesap**' i seçmeniz istenirse **iş veya okul hesabı**' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-138">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="edfdf-139">Dişli simgesini seçerek **Ayarlar** menüsünü açın ve ardından **iş ortağı ayarları**' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-139">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="edfdf-140">**Hesap ayarları** menüsünde, **ödeme ve vergi**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-140">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="edfdf-141">Ayrı programlara ödeme ve vergi profilleri atama</span><span class="sxs-lookup"><span data-stu-id="edfdf-141">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="edfdf-142">[Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açın ve sonra da dişli simgesini seçerek **Ayarlar** menüsünü açın.</span><span class="sxs-lookup"><span data-stu-id="edfdf-142">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="edfdf-143">**Iş ortağı ayarları**' nı seçin, **ödeme ve vergi bölümünü** genişletin ve ardından **ödeme ve vergi profili ataması**' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-143">Select **Partner settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="edfdf-144">Programlarınızın bir listesi görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-144">A list of your programs will be displayed.</span></span> <span data-ttu-id="edfdf-145">Profil ayrıntılarını görmek için bir programın yanındaki oku seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-145">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="edfdf-146">**Vergi profili** açılan menüsünde istediğiniz vergi profilini seçin veya yeni bir profil oluşturma seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-146">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="edfdf-147">Yeni bir profil oluşturma seçeneğini belirlediğinizde uygun şekilde yeniden yönlendirilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="edfdf-147">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="edfdf-148">Açılır pencerede devam ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-148">Select Continue in the pop-up window.</span></span> <span data-ttu-id="edfdf-149">Yeni bir vergi profili oluşturma işlemi aşağıda verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-149">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="edfdf-150">**Ödeme yöntemini** seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-150">Select **Payment method**.</span></span>

   - <span data-ttu-id="edfdf-151">Ödeme yönteminiz olarak **elektronik banka aktarımı** ' nı seçtiyseniz, istediğiniz ödeme profilini seçin veya yeni bir profil oluşturma seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-151">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="edfdf-152">Yeni bir profil oluşturma seçeneğini belirlediğinizde uygun şekilde yeniden yönlendirilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="edfdf-152">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="edfdf-153">Açılır pencerede devam ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-153">Select Continue in the pop-up window.</span></span> <span data-ttu-id="edfdf-154">Yeni bir ödeme profili oluşturma işlemi aşağıda verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-154">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="edfdf-155">Ödeme yönteminiz olarak **kredi dekontunu** seçtiyseniz doğrulamayı tamamlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="edfdf-155">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="edfdf-156">Bu, başvurulan SAP numarasının kuruluşunuza ait olduğunu onaylar.</span><span class="sxs-lookup"><span data-stu-id="edfdf-156">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="edfdf-157">Listelenen birden fazla Microsoft iş varlığı varsa, her varlık için bir ödeme profili seçmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-157">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="edfdf-158">Ödeme yöntemi kullanılabilirliği, teşvik programının kurallarına bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="edfdf-158">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="edfdf-159">**Para birimini** seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-159">Select the **Currency**.</span></span>

6. <span data-ttu-id="edfdf-160">Ödeme alanlarını tamamladıktan sonra **Gönder**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-160">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="edfdf-161">Banka profilinizi oluşturma</span><span class="sxs-lookup"><span data-stu-id="edfdf-161">Create your bank profile</span></span>

<span data-ttu-id="edfdf-162">Banka profilleri bir kuruluş düzeyinde oluşturulur.</span><span class="sxs-lookup"><span data-stu-id="edfdf-162">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="edfdf-163">Bu, bir banka profilinin bir kuruluştaki birden fazla MPN KIMLIĞI ile atanmasını ve bu programları teşvik etmesine olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="edfdf-163">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="edfdf-164">Farklı bankacılık ve vergi kuralları uygulanabildiği için bankacılık profili farklı ülkelere uygulanırken özel durumlar olabilir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-164">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="edfdf-165">Aşağıdaki sayfalarda, yıldız işareti olan alanlar gereklidir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-165">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="edfdf-166">Bir alanın ne olduğunu bilmiyorsanız, bilgi simgesini seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-166">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="edfdf-167">**Ayrıntılar** sayfasında, şu alanları doldurun: **profil adı:** bu ödeme profilini tanımlamak için benzersiz bir ad girin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-167">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="edfdf-168">**Banka hesabı konumu:** Şirketinizin bankasının bulunduğu ülke.</span><span class="sxs-lookup"><span data-stu-id="edfdf-168">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="edfdf-169">**Ödeme yöntemi:** Iş Ortağı Merkezi için tercih edilen ödeme yöntemi elektronik banka aktarmasıdır.</span><span class="sxs-lookup"><span data-stu-id="edfdf-169">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="edfdf-170">**İleri**’yi seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-170">Select **Next**.</span></span>

3. <span data-ttu-id="edfdf-171">**Banka hesabı** sayfasında, bilgilerinizi girin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-171">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="edfdf-172">Bu sayfada gösterilen alanlar ülkeye göre farklılık gösterecektir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-172">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="edfdf-173">**İleri**’yi seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-173">Select **Next**.</span></span>

5. <span data-ttu-id="edfdf-174">**Lehdar** sayfasında, ilgili bilgileri girin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-174">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="edfdf-175">Lehdar, şirketinizdeki kişiden, hesabınızı tartışmaları gerektiğinde bankanın iletişim kurabildikleri kişidir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-175">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="edfdf-176">Alanlar tamamlandığında, **son**' u seçin ve ardından banka profilinizi oluşturmak için **Onayla** ' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-176">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="edfdf-177">**Ödeme ve vergi profilleri** sayfasına yönlendirilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="edfdf-177">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="edfdf-178">Yeni profilinizin durumu, doğrulama tamamlanana kadar **bekleyen Microsoft doğrulamasını** yansıtır.</span><span class="sxs-lookup"><span data-stu-id="edfdf-178">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="edfdf-179">Bu işlem, 48 saate kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-179">This process may take up to 48 hours.</span></span> <span data-ttu-id="edfdf-180">Doğrulama tamamlandıktan sonra, profil durumunuz **onaylanan** veya **eylem gereken eylemi** yansıtır.</span><span class="sxs-lookup"><span data-stu-id="edfdf-180">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="edfdf-181">**Eylem gerekliyse**, gerekli bilgileri sağlamak için yukarıdaki adımları tekrarlayın.</span><span class="sxs-lookup"><span data-stu-id="edfdf-181">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="edfdf-182">Vergi profilinizi oluşturma</span><span class="sxs-lookup"><span data-stu-id="edfdf-182">Create your tax profile</span></span>

<span data-ttu-id="edfdf-183">Microsoft 'un kuruluşunuz için gereken vergi bilgilerini sağlamak için aşağıdaki yordamı kullanın.</span><span class="sxs-lookup"><span data-stu-id="edfdf-183">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="edfdf-184">Bu bölümdeki sayfalar dinamiktir ve ülkeniz ya da bölgenize göre değişir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-184">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="edfdf-185">Doğru vergi bilgilerini tanımlamaya yönelik yardıma ihtiyacınız varsa, ülkenizde uygun kamu kaynaklarıyla iletişim kurun.</span><span class="sxs-lookup"><span data-stu-id="edfdf-185">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="edfdf-186">Kuzey iş ortağı şirketleri için, W8 veya W9 formlarını tamamlamada bilgi almanız gerekiyorsa, aşağıdaki adresler size ıRS sitesine götürür:</span><span class="sxs-lookup"><span data-stu-id="edfdf-186">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="edfdf-187">Şirketiniz için yalnızca ayrıntıları girin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-187">Enter only details for your company.</span></span> <span data-ttu-id="edfdf-188">Kişisel ayrıntıları hiçbir şekilde girmeyin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-188">Never enter personal details.</span></span>

1. <span data-ttu-id="edfdf-189">**Iş profili** sayfasında, gerekli alanları tamamlayıp **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-189">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="edfdf-190">**Kurulum** sayfasında, şirketiniz için geçerli olan seçeneği belirleyin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-190">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="edfdf-191">Şirketiniz yalnızca Birleşik Devletler veya bu profil bir bireyin varsa, sol taraftaki seçeneği belirleyin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-191">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="edfdf-192">Şirketinizin Birleşik Devletler dışına dahil olması durumunda sağ taraftaki seçeneği seçin ve ardından listeden bulunduğunuz ülkeyi/bölgenizi seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-192">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="edfdf-193">**İleri**’yi seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-193">Select **Next**.</span></span> 

4. <span data-ttu-id="edfdf-194">**Vergi durumu** sayfasında, gerekli bilgileri girin ve ardından **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-194">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="edfdf-195">Bu sayfadaki alanlar ülkeye göre değişiklik gösterecektir.</span><span class="sxs-lookup"><span data-stu-id="edfdf-195">Fields on this page will vary by country.</span></span> <span data-ttu-id="edfdf-196">ayrıntılarınız.</span><span class="sxs-lookup"><span data-stu-id="edfdf-196">your details.</span></span> 

5. <span data-ttu-id="edfdf-197">**Ek belgeler** sayfasında gerekli alanlar ' ı seçin ve **İleri**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-197">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="edfdf-198">Ülkeniz veya bölgeniz için gereken tüm belgeleri karşıya yüklemek için **Araştır** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-198">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="edfdf-199">Belge adı gösterildiğinde **karşıya yükle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-199">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="edfdf-200">Belgeyi kaldırmanız gerekirse **Kaldır**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-200">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="edfdf-201">Kaydetmek ve devam etmek için **son**' u seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-201">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="edfdf-202">Açılan iletide **Onayla** ' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="edfdf-202">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="edfdf-203">**Ödeme ve vergi kurulumu** sayfasına geri yönlendirilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="edfdf-203">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="edfdf-204">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="edfdf-204">Next steps</span></span>

- [<span data-ttu-id="edfdf-205">Ödemeler ve vergiler hakkında sık sorulan sorular</span><span class="sxs-lookup"><span data-stu-id="edfdf-205">Common questions about payouts and taxes</span></span>](payout-faq.md)
