---
title: Bir cihazın kullanıma hazır deneyimini özelleştirme
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Müşterinin yeni cihazını teslim etmeden önce, Windows Autopilot profillerini kullanarak cihazın kullanıma hazır deneyimini (OOBE) özelleştirebilir veya önceden yapılandırabilirsiniz.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 5294495403be729adecb5a7814ade4f9d454a0f6
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149834"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Yeni cihazlarda Windows Otomatik Pilot profillerini kullanarak müşterinin kullanıma hazır deneyimini özelleştirme

**Uygun roller**: yönetici Aracısı | Genel yönetici | Satış Aracısı | Kullanıcı Yönetimi Yöneticisi

Müşteri cihazlarını yönetiyorsanız, müşterinin kullanıcıları için hazır olmayan deneyimi (OOBE) özelleştirmeniz gerekebilir. Cihazları müşterilere teslim etmeden önce Windows Autopilot profilleriyle yeni cihazları önceden yapılandırabilir ve müşterilerin zaten satın almış olduğu cihazlara yeni profiller uygulayabilirsiniz. 

OEM 'Lerin, cihazın **ürün anahtarı kimliğini (PKıD)** gösteren Autopilot cihaz kutusunun dışında bir sevkiyat etiketi de dahil başlatıldığını unutmayın.  Bu 1 boyutlu, okunabilir bir barkod, cihazların bir listesini kaldırmak zorunda kalmadan ve cihaz KIMLIĞINI alternatif yollarla ayırarak Autopilot için cihazları kaydetmek için bir yol ile aşağı akış ortakları sağlar.

Bu makalede, Autopilot profillerinin Iş Ortağı Merkezi 'nde cihazlara nasıl oluşturulacağı ve uygulanacağı açıklanır.

Zaten Autopilot hakkında bilgi sahibi değilseniz, bu makalelerdeki bilgileri gözden geçirin:

- [Windows Autopilot’a genel bakış](/windows/deployment/windows-10-auto-pilot)
- [Autopilot dağıtım başvurusu Kılavuzu](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Genel Bakış

Iş Ortağı Merkezi 'ndeki Windows Autopilot özelliği ile müşteri cihazlarına uygulanacak özel profiller oluşturabilirsiniz. Aşağıdaki profil ayarları, bu makalenin yayımlandığı sırada mevcuttur:

- Gizlilik ayarlarını atlayın. Bu isteğe bağlı Autopilot profili ayarı, kuruluşların OOBE işlemi sırasında gizlilik ayarlarını istememesini sağlar.

- Cihazda yerel yönetici hesabı oluşturmayı devre dışı bırakın. Kuruluşlar, işlem tamamlandıktan sonra cihazı ayarlamaya yönelik kullanıcının yönetici erişimine sahip olup olmadığına karar verebilir.

- Cihazı iş veya okul için otomatik olarak ayarlayın. Autopilot ile kaydedilen tüm cihazlar otomatik olarak iş veya okul cihazları olarak kabul edilir. bu nedenle, bu soru, OOBE işlemi sırasında istenmez.

- Cortana, OneDrive ve OEM kayıt kurulum sayfalarını atlayın. Autopilot'a kayıtlı tüm cihazlar, ilk deneyim (OOBE) işlemi sırasında bu sayfaları otomatik olarak atlar.

- Son Kullanıcı Lisans Sözleşmesi'ne (EULA) atla. 1709 Windows 10 başlayarak, kuruluşlar OOBE işlemi sırasında sunulan EULA sayfasını atlamayı karar kabilirsiniz. Windows [Windows Autopilot EULA sayfasını atlama hakkında](#windows-autopilot-eula-dismissal) dikkate alınması gereken önemli bilgiler için aşağıdaki EULA'yı çıkarma sayfasına bakın.

Aşağıdaki profil ve cihaz yönetim izinleri ve sınırlamaları geçerlidir:

- CSP iş ortakları aralarında bayi ilişkileri olan mevcut müşteriler için, müşteri iş ortağının temsilci yönetim ayrıcalıklarını kaldırmış olsa bile, Otomatik Pilot profillerini yönetmeye devam edebilir.

- Müşterilerinizin eklediği mevcut cihazları müşterileriniz için yönetebilirsiniz.

- Müşterinizin Microsoft Store İş'e veya Microsoft Intune Portalına yüklediği cihazları yönetemezsiniz.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>İş Ortağı Merkezi'da Autopilot profilleri oluşturma ve yönetme

Bu İş Ortağı Merkezi, dağıtım Windows Autopilot oluşturabilir ve bunları cihazlara uygulayabilirsiniz.

>[!NOTE]
>Profiller yalnızca yönetici aracıları oluşturabilir ve uygulayabilir.

### <a name="create-a-new-autopilot-profile"></a>Yeni bir Autopilot profili oluşturma

1. İş Ortağı Merkezi  menüsünden Müşteriler'i seçin ve ardından Autopilot profilini oluşturmakta olduğunu müşteriyi seçin.

2. Müşterinin ayrıntı sayfasında Cihazlar'ı **seçin.**

3. Profil **Windows Autopilot altında Yeni profil** **ekle'yi seçin.**

4. Profilin adını ve açıklamasını girin ve ardından OOBE ayarlarını yapılandırabilirsiniz. Aşağıdakilerden birini seçin:  

   - Kurulumda gizlilik ayarlarını atla

   - Kurulumda yerel yönetici hesabını devre dışı bırakma
  
   - Kurulumda sayfaları otomatik olarak atlama<br>
        (İş *veya okul için kurulumu otomatik olarak seçme ve* Cortana, OneDrive ve OEM kayıt kurulum sayfalarını *atla'yı içerir)*
  
   - Son kullanıcı lisans sözleşmelerini (EULA) atla<br> 
       >[!IMPORTANT] 
       >Windows [Windows Autopilot EULA sayfasını atlama hakkında](#windows-autopilot-eula-dismissal) dikkate alınması gereken önemli bilgiler için aşağıdaki EULA'yı çıkarma sayfasına bakın.

5. Tamamlandığında **Gönder'i** seçin.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Müşteri cihazlarına Autopilot profili uygulama

>[!NOTE]
>Aşağıdaki yönergelerde, müşterinin cihazlarını Iş Ortağı Merkezi 'ne eklediğiniz ve cihaz listesine erişebileceğiniz varsayılmaktadır. Müşterinin cihazlarını henüz eklemediyseniz, [müşterinin hesabına cihaz ekleme](#add-devices-to-a-customers-account) ' deki yönergeleri izleyin ve ardından aşağıdaki adımları izleyin.

Bir müşteri için Autopilot profili oluşturduktan sonra, bunu müşterinin cihazlarına uygulayabilirsiniz.

1. Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından Autopilot profilini oluşturduğunuz müşteriyi seçin.

2. Müşterinin ayrıntı sayfasında **cihazlar**' ı seçin.

3. **Cihazları cihazlara Uygula** altında, profil eklemek istediğiniz cihazları veya cihaz gruplarını seçin ve ardından **profili Uygula**' yı seçin. Yeni uyguladığınız profil **profil** sütununda görünür.

4. Profilin cihaza başarıyla uygulanacağını doğrulamak için aşağıdaki adımları izleyin.

    a.  Bir cihazı ağa bağlayın ve açın.

    b.  Uygun OOBE ekranlarının (varsa) göründüğünü doğrulayın.

    c.  OOBE işlemi durdurulduğunda, yeni bir kullanıcı için hazırlamak üzere cihazı fabrika varsayılan ayarlarına sıfırlayın.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Bir Autopilot profilini müşterinin cihazından kaldırma

1. Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından Autopilot profilini oluşturduğunuz müşteriyi seçin.

2. Müşterinin ayrıntı sayfasında **cihazlar**' ı seçin.

3. **Cihazlara profilleri Uygula** altında, profili kaldırmak istediğiniz cihazları seçin ve ardından **Profili Kaldır**' ı seçin.

   >[!NOTE]
   >Bir cihazın cihazdan kaldırılması, profili listenizden silmez. Bir profili silmek istiyorsanız, [Autopilot profilini güncelleştirme veya silme](#update-or-delete-an-autopilot-profile)bölümündeki yönergeleri izleyin.

### <a name="update-or-delete-an-autopilot-profile"></a>Autopilot profilini güncelleştirme veya silme

Müşteriler cihazları gönderdikten sonra, kullanıma hazır deneyimini değiştirmek isterse, Iş Ortağı Merkezi ' nde profili değiştirebilirsiniz.

Müşterinin cihazı internet 'e bağlandığı zaman, OOBE işlemi sırasında en son profil sürümünü indirir. Ayrıca, bir müşteri bir cihazı fabrika varsayılan ayarlarına geri yükleyene kadar, OOBE işlemi sırasında cihaz yeniden en son profil sürümünü indirir.

1. İş Ortağı Merkezi  menüsünden Müşteriler'i seçin ve ardından Autopilot profilini değiştirmenizi isteyen müşteriyi seçin.

2. Müşterinin ayrıntı sayfasında Cihazlar'ı **seçin.**

3. **Profiller Windows Autopilot altında** güncelleştirmeniz gereken profili seçin. Gerekli değişiklikleri yapın ve gönder'i **seçin.**

Bu profili silmek için sayfanın **sağ üst** köşesinden Profili sil'i seçin.

### <a name="add-devices-to-a-customers-account"></a>Müşterinin hesabına cihaz ekleme

>[!NOTE]
>Satış temsilcileri ve yönetici temsilcileri, bir müşterinin hesabına cihaz ekleyebilir.

Müşteri cihazlarına özel Autopilot profilleri uygulayamadan önce müşterinin cihaz listesine erişebilirsiniz.

OEM adını, seri numarasını ve model birleşimini kullanmayı planlıyorsanız şu sınırlamalara dikkat edin:

- Bu tuple yalnızca daha yeni cihazlarda (örneğin 4k karmalar) çalışır ve 128b karmalar (RS2 ve önceki cihazlar) için desteklanmaz.

- Kayıt, büyük/büyük/büyük harfe duyarlıdır, bu nedenle dosyada yer alan verilerin, OEM sağlayıcısı (donanım sağlayıcısı) tarafından sağlanan model ve üretici adlarına tam olarak eşleşmesi gerekir. 

Aşağıdaki yönergeleri izleyerek cihazları bir müşterinin hesabıyla İş Ortağı Merkezi.

1. İş Ortağı Merkezi  menüsünden Müşteriler'i seçin ve ardından cihazlarını yönetmek istediğiniz müşteriyi seçin.

2. Müşterinin ayrıntı sayfasında Cihazlar'ı **seçin.**

3. Cihazlara **profil uygula altında Cihaz ekle'yi** **seçin.**

4. Cihaz listesi için bir ad  girin ve ardından Gözat'ı seçerek müşterinin listesini (.csv dosya biçiminde) İş Ortağı Merkezi.

    >[!NOTE]
    >Bu .csv dosyasını cihaz satın alma ile almış olması gerekir. Bir .csv dosyası almadıysanız, Bir .csv dosyasına cihaz ekleme'de yer alan [adımları Windows Autopilot.](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)  

5. .csv dosyasını karşıya yükleyin ve Kaydet'i **seçin.**

Bir .csv dosyasını karşıya yüklemeye çalışırken hata iletisi alıyorsanız, dosyanın biçimini denetleyin. Yalnızca donanım karmasını veya OEM adı, seri numarası ve model (bu sütun sırasıyla) veya Windows Ürün Kimliğini kullanabilirsiniz. Cihaz listesi oluşturmak için cihaz **Ekle** ' nin yanındaki bağlantıdan sunulan Sample. csv dosyasını da kullanabilirsiniz.

. Csv dosyanız şuna benzer görünmelidir:

> **Cihaz seri numarası, Windows ürün KIMLIĞI, donanım karması, üretici adı, cihaz modeli**

> **{serialNumber},,, Microsoft Corporation, Surface dizüstü bilgisayar**

>[!NOTE]
> "Üretici adı" ve "cihaz modeli" büyük/küçük harfe duyarlıdır.

Üretici adı ve cihaz modeli için hangi değeri koyacağınızı bilmiyorsanız, doğru değerleri toplamak için bunu cihazda çalıştırabilirsiniz:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA

### <a name="important-information"></a>ÖNEMLI BILGILER

Windows Autopilot, müşterileriniz için yönettiğiniz cihazlarda özelleştirilmiş Windows yüklemelerini yapılandırmanıza olanak tanır. Müşteri tarafından bu şekilde yetkilendirilirse, EULA (Son Kullanıcı Lisans Sözleşmesi) kabul ekranı dahil olmak üzere Windows 'u ayarlarken kullanıcılara sunulan belirli kurulum ekranlarını göstermez veya gizleyebilirsiniz.

Bu işlevi kullanarak, kullanıcılara bildirim veya koşulların kabul etmesini sağlamak için tasarlanan tüm ekranları gizlemeyi veya gizlemeyi kabul etmiş olursunuz. koşulları, müşterinizin adına (bir kuruluşun veya bireysel kullanıcı gibi), herhangi bir uyarıyı onaylamak ve müşteriniz için geçerli olan koşulları kabul etmek için müşterinize yeterli izin ve yetkilendirme elde ettiğinizi kabul edersiniz. Bu, lisans hüküm ve koşullarına yönelik anlaşmayı ve bu aracı kullanarak gizlemeyin veya gizleyemediyseniz kullanıcıya sunulacak bildirimi içerir. Müşteri, Microsoft 'tan veya lisanslı dağıtıcılarından yazılım için geçerli bir lisans almadıysanız, müşteriniz bu cihazlarda Windows yazılımlarını kullanmayabilir.