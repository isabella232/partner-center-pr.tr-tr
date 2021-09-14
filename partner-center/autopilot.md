---
title: Cihazın ilk çalışma deneyimini özelleştirme
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Müşterinin yeni cihazı teslimmeden önce, Windows Autopilot profillerini kullanarak cihazın ilk kullanım deneyimini (OOBE) özelleştirilebilir veya önceden yapılandırabilirsiniz.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 95a201c53fc2eaf230d08bb4cfdd03a5747b5c05
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/13/2021
ms.locfileid: "126248355"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Yeni cihazlarda Windows Otomatik Pilot profillerini kullanarak müşterinin kullanıma hazır deneyimini özelleştirme

**Uygun roller:** Yönetici aracısı | Genel yönetici | Satış aracısı | Kullanıcı yönetimi yöneticisi

Müşteri cihazlarını yönetecek olursanız, müşterinin kullanıcıları için ilk deneyimi (OOBE) özelleştirmeniz gerekir. Yeni cihazları müşterilere teslimmeden önce Windows Autopilot profilleriyle önceden yapılandırabilirsiniz ve müşterilerin önceden satın aldığınız cihazlara yeni profiller uygulayabilirsiniz. 

OEM'ler Autopilot cihaz kutusunun dışında cihazın Ürün Anahtarı Kimliğini **(PKID)** gösteren bir sevkiyat etiketi dahil etmeye başlamıştır.  Bu 1 boyutlu, okunabilir barkod, aşağı akış iş ortaklarına cihazları autopilot'a kaydetmenin ve cihaz kimliğini alternatif yolla toplamaya gerek kalmadan kaydetmelerini sağlar.

Bu makalede, autopilot profillerini oluşturma ve bu cihazlarda cihazlara uygulama İş Ortağı Merkezi.

Autopilot hakkında bilgi sahibi değilsanız şu makalelerde yer alan bilgileri gözden geçirebilirsiniz:

- [Windows Autopilot’a genel bakış](/windows/deployment/windows-10-auto-pilot)
- [Autopilot dağıtım başvuru kılavuzu](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Genel Bakış

Windows Autopilot özelliğiyle İş Ortağı Merkezi cihazlara uygulanacak özel profiller oluşturabilirsiniz. Bu makale yayımlanırken aşağıdaki profil ayarları kullanılabilir durumdadır:

- Gizlilik ayarlarını atla. Bu isteğe bağlı Autopilot profil ayarı, kuruluşların OOBE işlemi sırasında gizlilik ayarlarını sormamalarını sağlar.

- Cihazda yerel yönetici hesabı oluşturma özelliğini devre dışı bırakma. Kuruluşlar, işlem tamamlandıktan sonra cihazı ayarlayan kullanıcının yönetici erişimine sahip olup olmadığına karar verir.

- İş veya okul için cihazı otomatik olarak ayarlama. Autopilot'a kayıtlı tüm cihazlar otomatik olarak iş veya okul cihazları olarak kabul edilir, bu nedenle bu soru OOBE işlemi sırasında sorulmayacak.

- Cortana, OneDrive ve OEM kayıt kurulum sayfalarını atla. Autopilot'a kayıtlı tüm cihazlar, ilk deneyim (OOBE) işlemi sırasında bu sayfaları otomatik olarak atlar.

- Son Kullanıcı Lisans Sözleşmesi'ne (EULA) atla. 1709 Windows 10 başlayarak, kuruluşlar OOBE işlemi sırasında sunulan EULA sayfasını atlamayı karar kılamaz. Kurulum Windows EULA sayfasını atlama hakkında dikkate alınması gereken önemli bilgiler için aşağıdaki [Autopilot EULA](#windows-autopilot-eula-dismissal) Windows bakın.

Aşağıdaki profil ve cihaz yönetim izinleri ve sınırlamaları geçerlidir:

- CSP iş ortakları aralarında bayi ilişkileri olan mevcut müşteriler için, müşteri iş ortağının temsilci yönetim ayrıcalıklarını kaldırmış olsa bile, Otomatik Pilot profillerini yönetmeye devam edebilir.

- Müşterilerinizin eklediği mevcut cihazları müşterileriniz için yönetebilirsiniz.

- Müşterinizin Microsoft Store İş'e veya Microsoft Intune Portalına yüklediği cihazları yönetemezsiniz.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>İş Ortağı Merkezi'de Autopilot profilleri oluşturma ve yönetme

Bu İş Ortağı Merkezi, autopilot Windows profillerini oluşturabilir ve cihazlara uygulayabilirsiniz.

>[!NOTE]
>Profiller yalnızca yönetici aracıları oluşturabilir ve uygulayabilir.

### <a name="create-a-new-autopilot-profile"></a>Yeni bir Autopilot profili oluşturma

1. İş Ortağı Merkezi  menüsünden Müşteriler'i ve ardından Autopilot profilini oluşturmakta olduğunu müşteriyi seçin.

2. Müşterinin ayrıntı sayfasında Cihazlar'ı **seçin.**

3. **Autopilot Windows altında Yeni profil** **ekle'yi seçin.**

4. Profilin adını ve açıklamasını girin ve ardından OOBE ayarlarını yapılandırabilirsiniz. Aşağıdakilerden birini seçin:  

   - Kurulumda gizlilik ayarlarını atla

   - Kurulumda yerel yönetici hesabını devre dışı bırakma
  
   - Kurulumda sayfaları otomatik olarak atlama<br>
        (İş *veya okul için kurulumu otomatik olarak seçme ve* Cortana, OneDrive ve OEM kaydı kurulum sayfalarını *atla dahil)*
  
   - Son kullanıcı lisans sözleşmelerini (EULA) atla<br> 
       >[!IMPORTANT] 
       >Kurulum Windows EULA sayfasını atlama hakkında dikkate alınması gereken önemli bilgiler için aşağıdaki [Autopilot EULA](#windows-autopilot-eula-dismissal) Windows bakın.

5. Tamamlandığında **Gönder'i** seçin.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Müşteri cihazlarına Autopilot profili uygulama

>[!NOTE]
>Aşağıdaki yönergelerde müşterinin cihazlarını önceden İş Ortağı Merkezi ve cihaz listesine erişebilirsiniz. Müşterinin cihazlarını henüz eklemedıysanız, Müşterinin hesabına cihaz [](#add-devices-to-a-customers-account) ekleme'de verilen yönergeleri izleyin ve ardından aşağıdaki adımları izleyin.

Bir müşteri için Bir Autopilot profili oluşturdukta, bunu müşterinin cihazlarına uygulayabilirsiniz.

1. İş Ortağı Merkezi  menüsünden Müşteriler'i seçin ve ardından Autopilot profilini oluşturduğunuz müşteriyi seçin.

2. Müşterinin ayrıntı sayfasında Cihazlar'ı **seçin.**

3. Cihazlara **profil uygula altında,** profil eklemek istediğiniz cihazları veya cihaz gruplarını seçin ve ardından Profili uygula'ya **tıklayın.** Az önce uyguladık profil Profil **sütununda** görünür.

4. Profilin cihaza başarıyla uygulanacak olduğunu doğrulamak için aşağıdaki adımları izleyin.

    a.  Bağlan cihazı ağa açın ve açın.

    b.  Uygun OOBE ekranlarının (varsa) görüntü olduğunu doğrulayın.

    c.  OOBE işlemi durduğunda, cihazı yeni bir kullanıcıya hazırlamak için cihazı fabrika varsayılan ayarlarına sıfırlayın.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Müşterinin cihazından Autopilot profilini kaldırma

1. İş Ortağı Merkezi  menüsünden Müşteriler'i seçin ve ardından Autopilot profilini oluşturduğunuz müşteriyi seçin.

2. Müşterinin ayrıntı sayfasında Cihazlar'ı **seçin.**

3. Cihazlara **profil uygula altında,** profili kaldırmak istediğiniz cihazları seçin ve ardından Profili kaldır'ı **seçin.**

   >[!NOTE]
   >Cihazdan profil kaldırmak, profili listenizden silemez. Bir profili silmek için Bir Autopilot profilini güncelleştirme [veya silme yönergelerini izleyin.](#update-or-delete-an-autopilot-profile)

### <a name="update-or-delete-an-autopilot-profile"></a>Autopilot profilini güncelleştirme veya silme

Bir müşteri, cihazları onlara verdikten sonra ilk kez deneyimi değiştirmek istiyorsa, cihazı geri almak için profili İş Ortağı Merkezi.

Müşterinin cihazı İnternet'e bağlandığında, OOBE işlemi sırasında en son profil sürümünü indirir. Ayrıca, bir müşteri bir cihazı fabrika varsayılan ayarlarına geri yükleyene kadar, cihaz OOBE işlemi sırasında en son profil sürümünü yeniden indirir.

1. İş Ortağı Merkezi  menüsünden Müşteriler'i seçin ve ardından Autopilot profilini değiştirmenizi isteyen müşteriyi seçin.

2. Müşterinin ayrıntı sayfasında Cihazlar'ı **seçin.**

3. **Autopilot Windows altında** güncelleştirmeniz gereken profili seçin. Gerekli değişiklikleri yapın ve Gönder'i **seçin.**

Bu profili silmek için **sayfanın sağ üst** köşesinden Profili sil'i seçin.

### <a name="add-devices-to-a-customers-account"></a>Müşterinin hesabına cihaz ekleme

>[!NOTE]
>Satış temsilcileri ve yönetici temsilcileri, bir müşterinin hesabına cihaz ekleyebilir.

Müşteri cihazlarına özel Autopilot profilleri uygulayamadan önce müşterinin cihaz listesine erişebilirsiniz.

OEM adı, seri numarası ve model birleşimini kullanmayı planlıyorsanız şu sınırlamalara dikkat edin:

- Bu tuple yalnızca daha yeni cihazlarda (örneğin 4k karmalar) çalışır ve 128b karmalar (RS2 ve önceki cihazlar) için desteklanmaz.

- Kayıt, büyük/büyük/büyük harfe duyarlıdır, bu nedenle dosyada yer alan verilerin, oem sağlayıcısı (donanım sağlayıcısı) tarafından sağlanan model ve üretici adlarına tam olarak eşleşmesi gerekir. 

Aşağıdaki yönergeleri izleyerek cihazları bir müşterinin hesaplarında İş Ortağı Merkezi.

1. İş Ortağı Merkezi  menüsünden Müşteriler'i seçin ve ardından cihazlarını yönetmek istediğiniz müşteriyi seçin.

2. Müşterinin ayrıntı sayfasında Cihazlar'ı **seçin.**

3. Cihazlara **profil uygula altında Cihaz ekle'yi** **seçin.**

4. Cihaz listesi için bir ad  girin ve ardından Gözat'ı seçerek müşterinin listesini (.csv biçiminde) İş Ortağı Merkezi.

    >[!NOTE]
    >Bu dosyanın cihaz satın .csv almış olması gerekir. Yeni bir dosya .csv, Autopilot'a cihaz ekleme adımlarını takip [Windows oluşturabilirsiniz.](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)  

5. Upload dosyasını .csv kaydet'i **seçin.**

Bir .csv dosyasını karşıya yüklemeye çalışırken hata iletisi alıyorsanız, dosyanın biçimini denetleyin. Yalnızca donanım karmasını veya OEM adı, seri numarası ve model (bu sütun sırasıyla) veya Windows Ürün Kimliğini kullanabilirsiniz. Cihaz listesi oluşturmak için cihaz .csv yanındaki bağlantıdan sağlanan örnek dosya **dosyasını** da kullanabilirsiniz.

.csv dosyanız şuna benzer şekilde görünüyor:

> **Cihaz Seri Numarası,Windows Kimliği,Donanım Karması,Üretici adı,Cihaz modeli**

> **{serialNumber},,,Microsoft Corporation,Surface Laptop**

>[!NOTE]
> "Üretici adı" ve "Cihaz modeli" büyük/büyük/büyük harfe duyarlıdır.

Üretici adı ve Cihaz Modeli için hangi değeri koyacaklarını bilmiyorsanız, doğru değerleri toplamak için bunu cihazda çalıştırabilirsiniz:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA'yı devreden çıkarma

### <a name="important-information"></a>ÖNEMLİ BILGILER

Windows Autopilot, müşterileriniz için yönetebileceğiniz cihazlarda Windows özelleştirilmiş yüklemeleri yapılandırmanıza olanak tanır. Müşteri bunu yapma yetkisine sahipse, EULA (Son Kullanıcı Lisans Sözleşmesi) kabul ekranı dahil olmak üzere Windows ayarlarken normalde kullanıcılara sunulan bazı ayar ekranlarını gizleyebilirsiniz.

Bu işlevi kullanarak, kullanıcılara koşulların bildirimini veya kabulünü sağlamak için tasarlanmış ekranları gizlemenin veya gizlemenin, müşteriden koşulları gizlemek için yeterli onay ve yetkilendirme elde ettiğiniz anlamına geldiğini ve sizin müşteriniz adına (örneğin, bir kuruluş veya tek bir kullanıcı) gizlemeniz anlamına geldiğini kabul etmiş olursunuz.  tüm bildirimlere onay ve müşteriniz için geçerli olan koşulları kabul etme. Bu, lisansın hüküm ve koşullarına ya da bu aracı kullanarak lisansı gizlemez veya gizlemezse kullanıcıya sunulacak bildirimle ilgili sözleşmeyi içerir. Müşteri Microsoft'tan veya Windows dağıtımcılarından yazılım için geçerli bir lisans edinmediyse, müşteriniz bu cihazlarda Windows yazılımlarını kullanamayabilirsiniz.