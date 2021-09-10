---
title: Azure CSP’de sağlanan Azure hizmetleri
description: Bu makalede, Azure Bulut Çözümü Sağlayıcısı (CSP) programında mevcut Bulut Çözümü Sağlayıcısı Azure hizmetleri açıklanmıştır.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: amitravat
ms.author: amrava
ms.localizationpriority: high
ms.date: 05/13/2020
ms.custom: SEOMAY.20
ms.openlocfilehash: 6037044a72bd9bd71131ddbc66fec0555bbd5f86
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961215"
---
# <a name="azure-services-available-in-the-azure-cloud-solution-provider-csp-program"></a>Azure Bulut Çözümü Sağlayıcısı (CSP) programında kullanılabilir Azure hizmetleri

**Uygun roller:** Yönetici aracısı | Faturalama yöneticisi | Genel yönetici | Yardım masası aracısı | Satış aracısı | Kullanıcı yönetimi yöneticisi

## <a name="available-azure-services-in-azure-csp"></a>Azure CSP’de sağlanan Azure hizmetleri

Bu makalede, Azure Bulut Çözümü Sağlayıcısı (CSP) programında mevcut Bulut Çözümü Sağlayıcısı Azure hizmetleri listelemektedir. Ayrıca Almanya ve Microsoft Azure Government gibi ulusal [bulutlarda hizmet](https://azure.microsoft.com/overview/clouds/germany/) [kullanılabilirliğini Microsoft Azure tartışmaktadır.](https://azure.microsoft.com/overview/clouds/government/)

>[!Note]
> [Azure Çin,](https://www.azure.cn/) Azure CSP kullanılamaz.

## <a name="global-cloud"></a>Küresel Bulut

Bu modeli temel Azure Resource Manager tüm hizmetler CSP Program'da kullanılabilir.  Klasik Azure Resource Manager hizmetleri gibi özel olmayan hizmetler CSP programında kullanılamaz.  

## <a name="csp-specific-service-configurations"></a>CSP-Specific Hizmeti Yapılandırmaları

Aşağıdaki hizmetler CSP'de özel yapılandırmalar gerektirir:

- [StorSimple](/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](/azure/active-directory-domain-services/active-directory-ds-csp)

- [Anahtar Kasası](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx)

- [Azure Time Series Analizler](https://azure.microsoft.com/services/time-series-insights/) Yalnızca müşteri kiracısı kullanıcıları Zaman Serisi veri Analizler erişebilirsiniz. İş ortakları varsayılan olarak müşterilerinin Zaman Serisi Analizler ortamını yönetebilir, ancak bu ortamdaki verilere erişmeleri gerekirse bunların müşteri kiracısına eklenmeleri gerekir.

- Sertifika aracılığıyla Azure SDK kitaplıklarını kimlik doğrulamaya için Yönetim Sertifikaları CSP modelinde desteklenmiyor.  Bunun yerine Azure AD hizmet sorumlusu kimlik doğrulamasını ve Azure.Identity kitaplığını kullanın.  [.NET için Azure SDK ile kimlik doğrulaması başvurusu](/dotnet/azure/sdk/authentication)

## <a name="visual-studio-marketplace"></a>Visual Studio Market

Artık üçüncü taraf uzantıları dışında Visual Studio Market'te listelenen öğeleri satın alabilirsiniz.

- [Azure DevOps](https://www.visualstudio.com/team-services/)

- [Visual Studio abonelikleri](https://www.visualstudio.com/subscriptions/)

- [Xamarin University eğitim](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

Çalışmaya başlamanıza yardımcı olmak için, CSP'de çalışmalarınızı [ayarlama,](/vsts/billing/csp/set-up-csp-customer) satın alma ve yönetme hakkında Azure DevOps belgeler oluşturduk.

## <a name="azure-marketplace-items-in-azure-csp"></a>Azure CSP’de Azure Market öğeleri

Tüm Azure Market öğeler şu anda aboneliklerde Azure CSP değildir.

- Microsoft tabanlı Azure hizmetleri: Bu hizmetler kullanılabilir. Önceki tabloyu ve yorumları gözden geçirme.

- Kendi lisansını getir (BYOL) öğeleri: Bu öğeler kullanılabilir. BYOL özellikli tüm Azure Market öğelerinin tam listesi, [Azure Market SAYFASıNDA mevcuttur.](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)

- Git Olarak Öde üçüncü taraf Azure Market öğeler: Sağlayıcı CSP kanalında yayımladığı sürece bu öğeler kullanılabilir. Daha fazla bilgi için [bkz. Ürünlerine abonelik Azure Market.](csp-commercial-marketplace-overview.md)

- Citrix XenApp Essentials: İş ortakları CSP'XenApp Essentials müşteriler için lisans satın alınabilir. Daha fazla bilgi için şu Citrix bloguna bakın: [XenApp Essentials dağıtımı artık Microsoft Bulut Çözümü Sağlayıcısı Kanalı üzerinden kullanılabilir.](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/)

## <a name="national-clouds"></a>Ulusal bulutlar

Aşağıdaki tabloda, ulusal bulutlarda CSP için kullanılabilir birinci taraf Azure ürünlerinin, hizmetlerinin ve özelliklerinin düzenli olarak güncelleştirilmiş bir listesi görüntülenir.

| Azure ürünü, hizmeti veya özelliği | ABD Kamu | Almanya |
| ------ | :-----------: | :-----------: |
|  **İşlem**  |    |    |
|  Sanal Makineler  |  X  |  X  |
|  Cloud Services  |    |    |
|  Sanal makine ölçek kümeleri  |  X  |  X  |
|  İşlevler  |    |    |
|  Azure Container Service  |    |    |
|  **Ağ**  |    |    |
|  Azure DNS  |    |    |
|  Content Delivery Network  |    |    |
|  Traffic Manager  |    |    |
|  ExpressRoute  |  X  |  X  |
|  Sanal Ağ  |  X  |  X  |
|  Load Balancer  |  X  |  X  |
|  VPN Gateway  |  X  |  X  |
|  Application Gateway  |  X  |  X  |
|  Ağ İzleyicisi  |  X  |  X  |
|  **Depolama**  |    |    |
|  Depolama  |  X  |  X  |
|  Backup  |  X  |  X  |
|  StorSimple  |    |  X  |
|  Site Recovery  |  X  |  X  |
|  Data Lake Storage  |    |    |
|  Yönetilen Diskler  |  X  |  X  |
|  **Web ve Mobil**  |    |    |
|  App Service  |  X  |  X  |
|  Linux’ta App Service  |    |  X  |
|  API Management  |  X  |    |
|  Content Delivery Network  |    |    |
|  Media Services  |  X  |  X  |
|  Notification Hubs  |  X  |  X  |
|  Azure Search  |    |    |
|  Azure App Service Logic Apps özelliği  |    |    |
|  **Kapsayıcılar**  |    |    |
|  App Service  |  X  |  X  |
|  Linux’ta App Service  |    |  X  |
|  Batch  |  X  |  X  |
|  Container Registry  |    |    |
|  Container Instances  |    |    |
|  Service Fabric  |  X  |  X  |
|  Kapsayıcı Hizmeti  |    |    |
|  **Veritabanları**  |    |    |
|  SQL Veritabanı  |  X  |  X  |
|  Azure Cosmos DB  |  X  |  X  |
|  SQL Veri Ambarı  |  X  |  X  |
|  Redis Cache  |  X  |  X  |
|  SQL Server Stretch Database  |  X  |  X  |
|  MySQL için Azure Veritabanı  |    |    |
|  PostgreSQL için Azure Veritabanı  |    |    |
|  **Veriler ve Analizler**  |    |    |
|  Databricks  |    |    |
|  HDInsight  |  X  |  X  |
|  Stream Analytics  |    |  X  |
|  Data Factory  |    |    |
|  Log Analytics  |  X  |    |
|  Veri Kataloğu  |    |    |
|  Data Lake Storage  |    |    |
|  Data Lake Analytics  |    |    |
|  Azure Analysis Services  |    |    |
|  Power BI Embedded  |    |    |
|  **AI ve Bilişsel Hizmetler**  |    |    |
|  Machine Learning  |    |  X  |
|  Azure Bot Hizmeti  |    |    |
|  Bilişsel Hizmetler  |    |    |
|  Azure Batch AI  |    |    |
|  **Nesnelerin İnterneti**  |    |    |
|  IoT Hub  |  X  |  X  |
|  IoT Central  |    |    |
|  Machine Learning  |    |  X  |
|  Stream Analytics  |    |  X  |
|  Event Hubs  |  X  |  X  |
|  Location-Based Hizmetleri  |    |    |
|  Notification Hubs  |  X  |  X  |
|  Time Series Insights  |    |    |
|  **Enterprise Tümleştirme**  |    |    |
|  StorSimple  |  X  |    |
|  API Management  |    |    |
|  Event Grid  |    |    |
|  Data Factory  |    |    |
|  Service Bus  |  X  |  X  |
|  Veri Kataloğu  |    |    |
|  SQL Server Stretch Database  |    |  X  |
|  Azure App Service Logic Apps özelliği  |    |    |
|  **Güvenlik ve Kimlik**  |    |    |
|  Azure Active Directory  |  X  |  X  |
|  Azure Active Directory B2C  |    |    |
|  Multi-Factor Authentication  |    |    |
|  Azure Active Directory Domain Services  |    |    |
|  Key Vault  |  X  |  X  |
|  Güvenlik Merkezi  |  X  |  X  |
|  **Geliştirici Araçları**  |    |    |
|  Visual Studio Team Services  |    |    |
|  Application Insights  |    |    |
|  DevTest Labs  |    |    |
|  Visual Studio App Center  |    |    |
|  Xamarin University  |    |    |
|  **İzleme ve Yönetim**  |    |    |
|  Advisor  |    |    |
|  Backup  |  X  |  X  |
|  Site Recovery  |  X  |  X  |
|  Scheduler  |  X  |  X  |
|  Otomasyon  |  X  |  X  |
|  Log Analytics  |  X  |    |
|  Azure İzleyici  |    |    |
|  Azure-Managed uygulamalar  |    |    |
|  Azure Geçişi  |    |    |
|  Yönetim Grupları  |    |  

## <a name="next-steps"></a>Sonraki adımlar

- Iş Ortağı Merkezi 'nde Azure için kullanılabilen yetenekler hakkında [bilgi edinin](/azure/cloud-solution-provider/overview/partner-center-overview) .

- Azure CSP 'de ilk müşteriyi [oluşturun](/azure/cloud-solution-provider/customer-management/create-new-customer) ve Azure hizmetlerini dağıtın.
