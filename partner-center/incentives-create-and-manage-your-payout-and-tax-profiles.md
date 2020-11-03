---
title: İş Ortağı Merkezi'ndeki ödeme ve vergi profilleri
ms.topic: how-to
ms.date: 09/11/2020
description: Teşvikleri çalışmanız için ödeme yapabilmeniz için ödeme ve vergi profilinizi oluşturun ve yönetin. Farklı profillerin oluşturulmasını, yönetilmesini ve kullanılmasını içerir.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: ca2ffe992ff92b98546934f4a249779f39179acb
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532087"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="a9626-104">Iş Ortağı Merkezi 'nde teşvikleri ödeme ve vergi profilleri oluşturma ve yönetme</span><span class="sxs-lookup"><span data-stu-id="a9626-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="a9626-105">**Aşağıdakiler cihazlar için geçerlidir:**</span><span class="sxs-lookup"><span data-stu-id="a9626-105">**Applies to:**</span></span>

- <span data-ttu-id="a9626-106">İş Ortağı Merkezi</span><span class="sxs-lookup"><span data-stu-id="a9626-106">Partner Center</span></span>

<span data-ttu-id="a9626-107">**Uygun roller:**</span><span class="sxs-lookup"><span data-stu-id="a9626-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="a9626-108">Teşvikleri Yöneticisi</span><span class="sxs-lookup"><span data-stu-id="a9626-108">Incentives admin</span></span>
- <span data-ttu-id="a9626-109">Faturalama yöneticisi</span><span class="sxs-lookup"><span data-stu-id="a9626-109">Billing admin</span></span>
- <span data-ttu-id="a9626-110">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="a9626-110">Global admin</span></span>

<span data-ttu-id="a9626-111">Belirli bir MPN konumuna ilişkin teşvik programlarınızda ödeme alabilmeniz için önce geçerli bir ödeme ve vergi profilini programla ve MPN konumuyla ilişkilendirerek kaydınızı tamamlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="a9626-111">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="a9626-112">Microsoft ödemeleri yapmak için bu ödeme ve vergi profilini kullanacaktır.</span><span class="sxs-lookup"><span data-stu-id="a9626-112">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="a9626-113">Teşvik programının kurallarına bağlı olarak ödeme için elektronik banka transferi veya alacak dekontu kullanmanıza izin verilebilir.</span><span class="sxs-lookup"><span data-stu-id="a9626-113">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="a9626-114">Roller, para birimleri ve diğer Microsoft programları</span><span class="sxs-lookup"><span data-stu-id="a9626-114">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="a9626-115">Ödeme ve vergi profiliniz ile çalışmaya başlamadan önce aşağıdaki bilgileri anlamanız önemlidir.</span><span class="sxs-lookup"><span data-stu-id="a9626-115">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="a9626-116">Roller ve izinler</span><span class="sxs-lookup"><span data-stu-id="a9626-116">Roles and permissions</span></span>

<span data-ttu-id="a9626-117">Teşvik ödemeleri için banka ve vergi bilgilerini girmek üzere bir teşvikleri yöneticisi olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="a9626-117">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="a9626-118">MPN/Account yöneticisiyseniz, kendinizi ve/veya iş arkadaşını teşvikleri Yöneticisi olacak şekilde atayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a9626-118">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="a9626-119">Teşvikleri yönetici izinleri istemeniz gerekiyorsa MPN yöneticinizle veya genel yöneticinizle iletişime geçin. [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açarak şirketinizde kimlerin bu rolleri olduğunu bulabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a9626-119">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="a9626-120">Sağ üst köşedeki **Ayarlar** simgesinden **Kullanıcı yönetimi** ' ni seçin ve ardından Genel yönetici ' ye filtre uygulayın.</span><span class="sxs-lookup"><span data-stu-id="a9626-120">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="a9626-121">Teşvikleri kullanıcılar, teşvik kazanç ve ödeme ayrıntılarını ve raporlarını görüntüleyebilir, ancak banka ve vergi ayrıntılarını düzenleyemez.</span><span class="sxs-lookup"><span data-stu-id="a9626-121">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="a9626-122">Tediye para birimini seçin</span><span class="sxs-lookup"><span data-stu-id="a9626-122">Choose your disbursement currency</span></span>

<span data-ttu-id="a9626-123">Varsayılan olarak, teşvikleri ödemeleri ilgili varlıkların yerel para birimiyle yapılır.</span><span class="sxs-lookup"><span data-stu-id="a9626-123">By default, incentives payments are made in the local currency of each respective entity.</span></span> <span data-ttu-id="a9626-124">Profil kurulumu sırasında farklı bir para birimi belirtebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a9626-124">You can specify a different currency during profile setup.</span></span> <span data-ttu-id="a9626-125">Ödemeler, Microsoft tarafından aylık olarak ayarlanan bir döviz kuru kullanılarak hesaplanır.</span><span class="sxs-lookup"><span data-stu-id="a9626-125">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="a9626-126">Seçilen para birimi nedeniyle, değerde yapılan değişikliklerden sorumlu olacaksınız.</span><span class="sxs-lookup"><span data-stu-id="a9626-126">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="bank-and-tax-information-and-other-programs"></a><span data-ttu-id="a9626-127">Banka ve vergi bilgileri ve diğer programlar</span><span class="sxs-lookup"><span data-stu-id="a9626-127">Bank and tax information and other programs</span></span>

<span data-ttu-id="a9626-128">Microsoft, ödeme için banka verilerinizi zaten kullanıyor olsa da, aşağıda açıklanan bilgileri sağlayın.</span><span class="sxs-lookup"><span data-stu-id="a9626-128">Provide the information described below even if Microsoft already uses your bank data for payments.</span></span> <span data-ttu-id="a9626-129">Bu, profilinizi yeni araca kopyalarken hassas bilgileri kullanıma sunabileceğinden, şirketinizin verilerinin gizliliğini ve güvenliğini sağlamaya yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="a9626-129">This helps ensure the privacy and security of your company’s data, since copying your profile to the new tool could expose sensitive information.</span></span> <span data-ttu-id="a9626-130">Bu işlemin ardından, verilerin eksiksiz ve doğru olduğundan emin olmak için de iyi bir fırsattır.</span><span class="sxs-lookup"><span data-stu-id="a9626-130">Going through this process is also a good opportunity to ensure the data is complete and accurate.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="a9626-131">Farklı Microsoft programları için farklı profiller kullanma</span><span class="sxs-lookup"><span data-stu-id="a9626-131">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="a9626-132">Perakende olarak, beş perakende teşvik programının her birine yönelik ödemeler aynı banka hesabına gidebilir.</span><span class="sxs-lookup"><span data-stu-id="a9626-132">Within retail, payments for each of the five retail incentive programs can go to the same bank account.</span></span> <span data-ttu-id="a9626-133">Alternatif olarak, Retail Xbox ödemelerinin bir banka hesabına gitmesini, perakende ofis farklı bir banka hesabına ödeme yaparken de seçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a9626-133">Alternatively, you can choose to have Retail Xbox payments go into one bank account while Retail Office is paid to a different bank account.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="a9626-134">Iş Ortağı Merkezi 'nde ödeme ve vergi profilleri oluşturma ve yönetme</span><span class="sxs-lookup"><span data-stu-id="a9626-134">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="a9626-135">Aşağıdaki bölümler, Iş Ortağı Merkezi 'nde ödeme ve vergi profilleri oluşturma ve yönetme sürecinde size yol gösterecektir.</span><span class="sxs-lookup"><span data-stu-id="a9626-135">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="a9626-136">Iş Ortağı Merkezi 'nde ödeme profilleri oluşturmak veya yönetmek için bir teşvik yöneticisi olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="a9626-136">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="a9626-137">Her bir teşvik programı altındaki her bir MPN konumuna bir rol atanması gerekir.</span><span class="sxs-lookup"><span data-stu-id="a9626-137">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="a9626-138">Iş Ortağı Merkezi 'ne teşvik yöneticileri ekleme hakkında daha fazla bilgi için bkz. [Kullanıcı hesapları oluşturma](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="a9626-138">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="a9626-139">Iş Ortağı Merkezi 'nde ödeme ve vergi kısmına erişin</span><span class="sxs-lookup"><span data-stu-id="a9626-139">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="a9626-140">Azure Active Directory (Azure AD) hesabınızı (Şirket hesabı) veya atanmış bir e-posta adresini kullanarak [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/) oturum açın.</span><span class="sxs-lookup"><span data-stu-id="a9626-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="a9626-141">Birden çok etki alanı, bir Azure AD hesabında kaydedilebilir.</span><span class="sxs-lookup"><span data-stu-id="a9626-141">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="a9626-142">Hangi etki alanlarının ilişkilendirildiğini öğrenmek için genel yöneticinizle iletişime geçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-142">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="a9626-143">Yalnızca etki alanı ile oturum açabiliyor @onmicrosoft.com , Azure AD hesabına ek etki alanları eklemek Için hesap yöneticinize başvurun.</span><span class="sxs-lookup"><span data-stu-id="a9626-143">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="a9626-144">**İş veya okul hesabı** ya da **kişisel hesap** ' i seçmeniz istenirse **iş veya okul hesabı** ' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-144">If you're prompted to select **Work or school account** or **Personal Account** , select **Work or school account** .</span></span>

2. <span data-ttu-id="a9626-145">Dişli simgesini seçerek **Ayarlar** menüsünü açın ve ardından **iş ortağı ayarları** ' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-145">Select the gear icon to open the **Settings** menu, and then select **Partner settings** .</span></span>

3. <span data-ttu-id="a9626-146">**Hesap ayarları** menüsünde, **ödeme ve vergi** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-146">In the **Account settings** menu, select **Payout and tax** .</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="a9626-147">Ayrı programlara ödeme ve vergi profilleri atama</span><span class="sxs-lookup"><span data-stu-id="a9626-147">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="a9626-148">[Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard/)oturum açın ve sonra da dişli simgesini seçerek **Ayarlar** menüsünü açın.</span><span class="sxs-lookup"><span data-stu-id="a9626-148">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="a9626-149">**Iş ortağı ayarları** ' nı seçin, **ödeme ve vergi bölümünü** genişletin ve ardından **ödeme ve vergi profili ataması** ' nı seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-149">Select **Partner settings** , expand the **Payout and tax section** , and then select **Payout and tax profile assignment** .</span></span> 
   
   <span data-ttu-id="a9626-150">Programlarınızın bir listesi görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="a9626-150">A list of your programs will be displayed.</span></span> <span data-ttu-id="a9626-151">Profil ayrıntılarını görmek için bir programın yanındaki oku seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-151">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="a9626-152">**Vergi profili** açılan menüsünde istediğiniz vergi profilini seçin veya yeni bir profil oluşturma seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="a9626-152">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="a9626-153">Yeni bir profil oluşturma seçeneğini belirlediğinizde uygun şekilde yeniden yönlendirilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a9626-153">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="a9626-154">Açılır pencerede devam ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-154">Select Continue in the pop-up window.</span></span> <span data-ttu-id="a9626-155">Yeni bir vergi profili oluşturma işlemi aşağıda verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="a9626-155">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="a9626-156">**Ödeme yöntemini** seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-156">Select **Payment method** .</span></span>

   - <span data-ttu-id="a9626-157">Ödeme yönteminiz olarak **elektronik banka aktarımı** ' nı seçtiyseniz, istediğiniz ödeme profilini seçin veya yeni bir profil oluşturma seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="a9626-157">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="a9626-158">Yeni bir profil oluşturma seçeneğini belirlediğinizde uygun şekilde yeniden yönlendirilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a9626-158">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="a9626-159">Açılır pencerede devam ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-159">Select Continue in the pop-up window.</span></span> <span data-ttu-id="a9626-160">Yeni bir ödeme profili oluşturma işlemi aşağıda verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="a9626-160">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="a9626-161">Ödeme yönteminiz olarak **kredi dekontunu** seçtiyseniz doğrulamayı tamamlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a9626-161">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="a9626-162">Bu, başvurulan SAP numarasının kuruluşunuza ait olduğunu onaylar.</span><span class="sxs-lookup"><span data-stu-id="a9626-162">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="a9626-163">Listelenen birden fazla Microsoft iş varlığı varsa, her varlık için bir ödeme profili seçmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="a9626-163">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="a9626-164">Ödeme yöntemi kullanılabilirliği, teşvik programının kurallarına bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="a9626-164">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="a9626-165">**Para birimini** seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-165">Select the **Currency** .</span></span>

6. <span data-ttu-id="a9626-166">Ödeme alanlarını tamamladıktan sonra **Gönder** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-166">When you’ve completed all of the payment fields, select **Submit** .</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="a9626-167">Banka profilinizi oluşturma</span><span class="sxs-lookup"><span data-stu-id="a9626-167">Create your bank profile</span></span>

<span data-ttu-id="a9626-168">Banka profilleri bir kuruluş düzeyinde oluşturulur.</span><span class="sxs-lookup"><span data-stu-id="a9626-168">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="a9626-169">Bu, bir banka profilinin bir kuruluştaki birden fazla MPN KIMLIĞI ile atanmasını ve bu programları teşvik etmesine olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="a9626-169">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="a9626-170">Farklı bankacılık ve vergi kuralları uygulanabildiği için bankacılık profili farklı ülkelere uygulanırken özel durumlar olabilir.</span><span class="sxs-lookup"><span data-stu-id="a9626-170">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="a9626-171">Aşağıdaki sayfalarda, yıldız işareti olan alanlar gereklidir.</span><span class="sxs-lookup"><span data-stu-id="a9626-171">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="a9626-172">Bir alanın ne olduğunu bilmiyorsanız, bilgi simgesini seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-172">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="a9626-173">**Ayrıntılar** sayfasında, şu alanları doldurun: **profil adı:** bu ödeme profilini tanımlamak için benzersiz bir ad girin.</span><span class="sxs-lookup"><span data-stu-id="a9626-173">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="a9626-174">**Banka hesabı konumu:** Şirketinizin bankasının bulunduğu ülke.</span><span class="sxs-lookup"><span data-stu-id="a9626-174">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="a9626-175">**Ödeme yöntemi:** Iş Ortağı Merkezi için tercih edilen ödeme yöntemi elektronik banka aktarmasıdır.</span><span class="sxs-lookup"><span data-stu-id="a9626-175">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="a9626-176">**İleri** ’yi seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-176">Select **Next** .</span></span>

3. <span data-ttu-id="a9626-177">**Banka hesabı** sayfasında, bilgilerinizi girin.</span><span class="sxs-lookup"><span data-stu-id="a9626-177">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="a9626-178">Bu sayfada gösterilen alanlar ülkeye göre farklılık gösterecektir.</span><span class="sxs-lookup"><span data-stu-id="a9626-178">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="a9626-179">**İleri** ’yi seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-179">Select **Next** .</span></span>

5. <span data-ttu-id="a9626-180">**Lehdar** sayfasında, ilgili bilgileri girin.</span><span class="sxs-lookup"><span data-stu-id="a9626-180">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="a9626-181">Lehdar, şirketinizdeki kişiden, hesabınızı tartışmaları gerektiğinde bankanın iletişim kurabildikleri kişidir.</span><span class="sxs-lookup"><span data-stu-id="a9626-181">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="a9626-182">Alanlar tamamlandığında, **son** ' u seçin ve ardından banka profilinizi oluşturmak için **Onayla** ' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-182">When the fields are completed, select **Finish** , and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="a9626-183">**Ödeme ve vergi profilleri** sayfasına yönlendirilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a9626-183">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="a9626-184">Yeni profilinizin durumu, doğrulama tamamlanana kadar **bekleyen Microsoft doğrulamasını** yansıtır.</span><span class="sxs-lookup"><span data-stu-id="a9626-184">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="a9626-185">Bu işlem, 48 saate kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="a9626-185">This process may take up to 48 hours.</span></span> <span data-ttu-id="a9626-186">Doğrulama tamamlandıktan sonra, profil durumunuz **onaylanan** veya **eylem gereken eylemi** yansıtır.</span><span class="sxs-lookup"><span data-stu-id="a9626-186">Once validation has been completed, your profile status will reflect either **Approved** or **Action required** .</span></span> <span data-ttu-id="a9626-187">**Eylem gerekliyse** , gerekli bilgileri sağlamak için yukarıdaki adımları tekrarlayın.</span><span class="sxs-lookup"><span data-stu-id="a9626-187">If **Action Required** , repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="a9626-188">Vergi profilinizi oluşturma</span><span class="sxs-lookup"><span data-stu-id="a9626-188">Create your tax profile</span></span>

<span data-ttu-id="a9626-189">Microsoft 'un kuruluşunuz için gereken vergi bilgilerini sağlamak için aşağıdaki yordamı kullanın.</span><span class="sxs-lookup"><span data-stu-id="a9626-189">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="a9626-190">Bu bölümdeki sayfalar dinamiktir ve ülkeniz ya da bölgenize göre değişir.</span><span class="sxs-lookup"><span data-stu-id="a9626-190">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="a9626-191">Doğru vergi bilgilerini tanımlamaya yönelik yardıma ihtiyacınız varsa, ülkenizde uygun kamu kaynaklarıyla iletişim kurun.</span><span class="sxs-lookup"><span data-stu-id="a9626-191">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="a9626-192">Kuzey iş ortağı şirketleri için, W8 veya W9 formlarını tamamlamada bilgi almanız gerekiyorsa, aşağıdaki adresler size ıRS sitesine götürür:</span><span class="sxs-lookup"><span data-stu-id="a9626-192">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="a9626-193">Şirketiniz için yalnızca ayrıntıları girin.</span><span class="sxs-lookup"><span data-stu-id="a9626-193">Enter only details for your company.</span></span> <span data-ttu-id="a9626-194">Kişisel ayrıntıları hiçbir şekilde girmeyin.</span><span class="sxs-lookup"><span data-stu-id="a9626-194">Never enter personal details.</span></span>

1. <span data-ttu-id="a9626-195">**Iş profili** sayfasında, gerekli alanları tamamlayıp **İleri** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-195">On the **Business Profile** page, complete the required fields and then select **Next** .</span></span> 

2. <span data-ttu-id="a9626-196">**Kurulum** sayfasında, şirketiniz için geçerli olan seçeneği belirleyin.</span><span class="sxs-lookup"><span data-stu-id="a9626-196">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="a9626-197">Şirketiniz yalnızca Birleşik Devletler veya bu profil bir bireyin varsa, sol taraftaki seçeneği belirleyin.</span><span class="sxs-lookup"><span data-stu-id="a9626-197">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="a9626-198">Şirketinizin Birleşik Devletler dışına dahil olması durumunda sağ taraftaki seçeneği seçin ve ardından listeden bulunduğunuz ülkeyi/bölgenizi seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-198">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="a9626-199">**İleri** ’yi seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-199">Select **Next** .</span></span> 

4. <span data-ttu-id="a9626-200">**Vergi durumu** sayfasında, gerekli bilgileri girin ve ardından **İleri** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-200">On the **Tax status** page, enter the required information, and then select **Next** .</span></span> <span data-ttu-id="a9626-201">Bu sayfadaki alanlar ülkeye göre değişiklik gösterecektir.</span><span class="sxs-lookup"><span data-stu-id="a9626-201">Fields on this page will vary by country.</span></span> <span data-ttu-id="a9626-202">ayrıntılarınız.</span><span class="sxs-lookup"><span data-stu-id="a9626-202">your details.</span></span> 

5. <span data-ttu-id="a9626-203">**Ek belgeler** sayfasında gerekli alanlar ' ı seçin ve **İleri** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-203">On the **Additional documentation** page, the required fields and select **Next** .</span></span> 

6. <span data-ttu-id="a9626-204">Ülkeniz veya bölgeniz için gereken tüm belgeleri karşıya yüklemek için **Araştır** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-204">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="a9626-205">Belge adı gösterildiğinde **karşıya yükle** ' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-205">When the document name is shown, select **Upload** .</span></span> 

7. <span data-ttu-id="a9626-206">Belgeyi kaldırmanız gerekirse **Kaldır** ' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-206">If you need to remove the document, select **Remove** .</span></span>

8. <span data-ttu-id="a9626-207">Kaydetmek ve devam etmek için **son** ' u seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-207">To save and continue, select **Finish** .</span></span>

9. <span data-ttu-id="a9626-208">Açılan iletide **Onayla** ' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="a9626-208">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="a9626-209">**Ödeme ve vergi kurulumu** sayfasına geri yönlendirilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a9626-209">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a9626-210">Sonraki adımlar</span><span class="sxs-lookup"><span data-stu-id="a9626-210">Next steps</span></span>

- [<span data-ttu-id="a9626-211">Teşvikleri ödeme ve vergi profili SSS</span><span class="sxs-lookup"><span data-stu-id="a9626-211">Incentives payout and tax profile FAQs</span></span>](incentives-payout-tax-profile-faqs.md)
