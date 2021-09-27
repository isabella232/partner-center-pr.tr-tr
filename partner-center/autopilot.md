---
title: Bir cihazın kullanıma hazır deneyimini özelleştirme
ms.topic: how-to
ms.date: 09/21/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: müşterinin yeni cihazını teslim etmeden önce, Windows Autopilot profillerini kullanarak cihazın kullanıma hazır deneyimini (OOBE) özelleştirebilir veya önceden yapılandırabilirsiniz.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 1d8b0f346a3e3d23fcfeb4f24911c479fd7c1071
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129074210"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Yeni cihazlarda Windows Otomatik Pilot profillerini kullanarak müşterinin kullanıma hazır deneyimini özelleştirme

**Uygun roller**: yönetici Aracısı | Genel yönetici | Satış Aracısı | Kullanıcı Yönetimi Yöneticisi

Müşteri cihazlarını yönetiyorsanız, müşterinin kullanıcıları için hazır olmayan deneyimi (OOBE) özelleştirmeniz gerekebilir. cihazları müşterilere teslim etmeden önce Windows Autopilot profilleriyle yeni cihazları önceden yapılandırabilir ve müşterilerin zaten satın almış olduğu cihazlara yeni profiller uygulayabilirsiniz. 

OEM 'Lerin, cihazın **ürün anahtarı kimliğini (PKıD)** gösteren Autopilot cihaz kutusunun dışında bir sevkiyat etiketi de dahil başlatıldığını unutmayın.  Bu 1 boyutlu, okunabilir bir barkod, cihazların bir listesini kaldırmak zorunda kalmadan ve cihaz KIMLIĞINI alternatif yollarla ayırarak Autopilot için cihazları kaydetmek için bir yol ile aşağı akış ortakları sağlar.

Bu makalede, Autopilot profillerinin Iş Ortağı Merkezi 'nde cihazlara nasıl oluşturulacağı ve uygulanacağı açıklanır.

Zaten Autopilot hakkında bilgi sahibi değilseniz, bu makalelerdeki bilgileri gözden geçirin:

- [Windows Autopilot’a genel bakış](/windows/deployment/windows-10-auto-pilot)
- [Autopilot dağıtım başvurusu Kılavuzu](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Genel Bakış

iş ortağı merkezi 'nde Windows Autopilot özelliği ile müşteri cihazlarına uygulanacak özel profiller oluşturabilirsiniz. Aşağıdaki profil ayarları, bu makalenin yayımlandığı sırada mevcuttur:

- Gizlilik ayarlarını atlayın. Bu isteğe bağlı Autopilot profili ayarı, kuruluşların OOBE işlemi sırasında gizlilik ayarlarını istememesini sağlar.

- Cihazda yerel yönetici hesabı oluşturmayı devre dışı bırakın. Kuruluşlar, işlem tamamlandıktan sonra cihazı ayarlamaya yönelik kullanıcının yönetici erişimine sahip olup olmadığına karar verebilir.

- Cihazı iş veya okul için otomatik olarak ayarlayın. Autopilot ile kaydedilen tüm cihazlar otomatik olarak iş veya okul cihazları olarak kabul edilir. bu nedenle, bu soru, OOBE işlemi sırasında istenmez.

- Cortana, OneDrive ve OEM kayıt kurulum sayfalarını atlayın. Autopilot ile kaydedilen tüm cihazlar, kullanıma hazır deneyim (OOBE) işlemi sırasında bu sayfaları otomatik olarak atlar.

- Son Kullanıcı Lisans Sözleşmesi 'Ni (EULA) atlayın. Windows 10 sürüm 1709 ' den başlayarak kuruluşlar, OOBE işlemi sırasında sunulan EULA sayfasını atlamaya karar verebilir. Windows kurulum sırasında eula sayfasını atlamayı göz önünde bulundurmanız gereken önemli bilgiler için bkz. [Windows Autopilot EULA](#windows-autopilot-eula-dismissal) yok.

Aşağıdaki profil ve cihaz yönetim izinleri ve sınırlamaları geçerlidir:

- CSP iş ortakları aralarında bayi ilişkileri olan mevcut müşteriler için, müşteri iş ortağının temsilci yönetim ayrıcalıklarını kaldırmış olsa bile, Otomatik Pilot profillerini yönetmeye devam edebilir.

- Müşterilerinizin eklediği mevcut cihazları müşterileriniz için yönetebilirsiniz.

- Müşterinizin Microsoft Store İş'e veya Microsoft Intune Portalına yüklediği cihazları yönetemezsiniz.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Autopilot profillerini Iş Ortağı Merkezi 'nde oluşturma ve yönetme

iş ortağı merkezi 'nde, Windows Autopilot dağıtım profilleri oluşturabilir ve bunları cihazlara uygulayabilirsiniz.

> [!NOTE]
> Yalnızca yönetici aracıları profil oluşturabilir ve uygulayabilir.

### <a name="create-a-new-autopilot-profile"></a>Yeni bir Autopilot profili oluşturun

#### <a name="workspaces-view"></a>[Çalışma alanları görünümü](#tab/workspaces-view)

1. [Iş Ortağı Merkezi panosunda](https://partner.microsoft.com/dashboard) oturum açın ve **müşteriler** kutucuğunu seçin.

2. Müşterinin ayrıntı sayfasında **cihazlar**' ı seçin.

3. **Windows Autopilot profilleri** altında **yeni profil ekle**' yi seçin.

4. Profilin adını ve açıklamasını girip OOBE ayarlarını yapılandırın. Aşağıdakilerden birini seçin:  

   - Kurulum 'da gizlilik ayarlarını atla

   - Kurulumda yerel yönetici hesabını devre dışı bırak
  
   - Kurulum 'da sayfaları otomatik olarak atla<br>
        ( *iş veya okul için kurulumu otomatik olarak seç* ve *Cortana, OneDrive ve OEM kayıt kurulum sayfalarını atla*)
  
   - Son Kullanıcı Lisans Sözleşmesi 'ni (EULA) atla<br> 
       >[!IMPORTANT] 
       >Windows kurulum sırasında eula sayfasını atlamayı göz önünde bulundurmanız gereken önemli bilgiler için bkz. [Windows Autopilot EULA](#windows-autopilot-eula-dismissal) yok.

5. Bittiğinde **Gönder** ' i seçin.

#### <a name="current-view"></a>[Geçerli görünüm](#tab/current-view)

1. Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından Autopilot profilini oluşturduğunuz müşteriyi seçin.

2. Müşterinin ayrıntı sayfasında **cihazlar**' ı seçin.

3. **Windows Autopilot profilleri** altında **yeni profil ekle**' yi seçin.

4. Profilin adını ve açıklamasını girip OOBE ayarlarını yapılandırın. Aşağıdakilerden birini seçin:  

   - Kurulum 'da gizlilik ayarlarını atla

   - Kurulumda yerel yönetici hesabını devre dışı bırak
  
   - Kurulum 'da sayfaları otomatik olarak atla<br>
        ( *iş veya okul için kurulumu otomatik olarak seç* ve *Cortana, OneDrive ve OEM kayıt kurulum sayfalarını atla*)
  
   - Son Kullanıcı Lisans Sözleşmesi 'ni (EULA) atla<br> 
       >[!IMPORTANT] 
       >Windows kurulum sırasında eula sayfasını atlamayı göz önünde bulundurmanız gereken önemli bilgiler için bkz. [Windows Autopilot EULA](#windows-autopilot-eula-dismissal) yok.

5. Bittiğinde **Gönder** ' i seçin.

* * * 

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Müşteri cihazlarına bir Autopilot profili uygulama

>[!NOTE]
>Aşağıdaki yönergelerde, müşterinin cihazlarını Iş Ortağı Merkezi 'ne eklediğiniz ve cihaz listesine erişebileceğiniz varsayılmaktadır. Müşterinin cihazlarını henüz eklemediyseniz, [müşterinin hesabına cihaz ekleme](#add-devices-to-a-customers-account) ' deki yönergeleri izleyin ve ardından aşağıdaki adımları izleyin.

Bir müşteri için Autopilot profili oluşturduktan sonra, bunu müşterinin cihazlarına uygulayabilirsiniz.

1. Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından Autopilot profilini oluşturduğunuz müşteriyi seçin.

2. Müşterinin ayrıntı sayfasında **cihazlar**' ı seçin.

3. **Cihazları cihazlara Uygula** altında, profil eklemek istediğiniz cihazları veya cihaz gruplarını seçin ve ardından **profili Uygula**' yı seçin. Yeni uyguladığınız profil **profil** sütununda görünür.

4. Profilin cihaza başarıyla uygulanacağını doğrulamak için aşağıdaki adımları izleyin.

    a.  bir cihazı ağa Bağlan ve açın.

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

Müşterinin cihazı internet 'e bağlandığı zaman, OOBE işlemi sırasında en son profil sürümünü indirir. Ayrıca, bir müşteri bir cihazı fabrika varsayılan ayarlarına geri yüklediğinde, bu cihaz, OOBE işlemi sırasında en son profil sürümünü yeniden indirir.

1. Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından bir Autopilot profilini değiştirmenizi isteyen müşteriyi seçin.

2. Müşterinin ayrıntı sayfasında **cihazlar**' ı seçin.

3. **Windows Autopilot profilleri** altında, güncelleştirmeniz gereken profili seçin. Gerekli değişiklikleri yapıp **Gönder**' i seçin.

Bu profili silmek için sayfanın sağ üst köşesinden **Profili Sil** ' i seçin.

### <a name="add-devices-to-a-customers-account"></a>Müşterinin hesabına cihaz ekleme

>[!NOTE]
>Satış aracıları ve yönetici aracıları, bir müşterinin hesabına cihaz ekleyebilir.

Müşteri cihazlarına özel Autopilot profilleri uygulayabilmeniz için önce müşterinin cihaz listesine erişebiliyor olmanız gerekir.

OEM adı, seri numarası ve model birleşimini kullanmayı planlıyorsanız, bu sınırlamalara dikkat edin:

- Bu tanımlama grubu yalnızca daha yeni cihazlar (örneğin, 4k karmaları) için geçerlidir ve 128b karmaları (RS2 ve önceki cihazlar) için desteklenmez.

- Demet kaydı, büyük/küçük harfe duyarlıdır, bu nedenle dosyadaki verilerin, ***tam*** olarak OEM sağlayıcısı (donanım sağlayıcısı) tarafından sağlandığı şekilde model ve üretici adlarıyla eşleşmesi gerekir.

Iş Ortağı Merkezi 'nde bir müşterinin hesabına cihaz eklemek için aşağıdaki yönergeleri izleyin.

1. Iş Ortağı Merkezi menüsünden **müşteriler** ' i seçin ve ardından cihazlarını yönetmek istediğiniz müşteriyi seçin.

2. Müşterinin ayrıntı sayfasında **cihazlar**' ı seçin.

3. **Cihazlara profil Uygula** altında **Cihaz Ekle**' yi seçin.

4. Cihaz listesi için bir ad girin ve ardından, müşteri listesini (.csv dosya biçiminde) Iş Ortağı Merkezi 'ne yüklemek için **Gözden** geçirme ' yi seçin.

    >[!NOTE]
    >Bu .csv dosyasını cihazınızın satın almanızdan almış olmanız gerekir. bir .csv dosyası almadıysanız, [Windows Autopilot 'e cihaz ekleme](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)bölümündeki adımları izleyerek kendiniz bir tane oluşturabilirsiniz.  

5. .csv dosyasını Upload ve ardından **kaydet**' i seçin.

Bir .csv dosyasını karşıya yüklemeye çalışırken hata iletisi alıyorsanız, dosyanın biçimini denetleyin. Yalnızca donanım karmasını veya OEM adı, seri numarası ve model (bu sütun sırasıyla) veya Windows Ürün Kimliğini kullanabilirsiniz. Cihaz listesi oluşturmak için cihaz **ekleme** ' nin yanındaki bağlantıdan sunulan örnek .csv dosyasını da kullanabilirsiniz.

.csv dosyanız şuna benzemelidir:

> **cihaz seri numarası, Windows ürün kimliği, donanım karması, üretici adı, cihaz modeli**

> **{serialNumber},,, Microsoft Corporation, Surface Laptop**

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

Windows Autopilot, müşterileriniz için yönettiğiniz cihazlarda Windows özelleştirilmiş yüklemelerini yapılandırmanıza olanak tanır. müşteri tarafından bu şekilde yetkilendirilirse, EULA (son kullanıcı lisans sözleşmesi) kabul ekranı dahil olmak üzere Windows ayarlanırken, normalde kullanıcılara sunulan belirli kurulum ekranlarını göstermez veya gizleyebilirsiniz.

Bu işlevi kullanarak, kullanıcılara bildirim veya koşulların kabul edilmesini sağlamak için tasarlanan tüm ekranları gizlemeyi veya gizlemeyi kabul etmiş olursunuz. Bu durumda, koşulları gizleyecek ve müşterinizin adına (örneğin, bir kuruluşun veya tek bir kullanıcının olması gibi)  herhangi bir bildirim onayı ve müşteriniz için geçerli olan tüm koşulları kabul edin. Bu, lisans hüküm ve koşullarına yönelik anlaşmayı ve bu aracı kullanarak gizlemeyin veya gizleyemediyseniz kullanıcıya sunulacak bildirimi içerir. müşteri, Microsoft 'tan veya lisanslı dağıtıcılardan yazılım için geçerli bir lisans almadıysanız, bu cihazlarda müşteriniz Windows yazılımını kullanmayabilir.