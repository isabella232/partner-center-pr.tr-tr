---
title: Azure rezervasyonları & sunucu abonelikleri
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Müşteriler için Bulut Çözümü Sağlayıcısı Azure rezervasyonlarını ve Sunucu aboneliklerini edinme, sağlama ve yönetme fırsatlarını öğrenin.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 18b52fe72614ef6c0b501af4ecb4aafffd0150d89eaf50f255663aa6f831345d
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2021
ms.locfileid: "115680694"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a>Müşteriler için Azure ayrılmış vm & (RI) + sunucu aboneliklerini edinme, sağlama ve yönetme


**Uygun roller:** Yönetici aracısı | Genel yönetici | Yardım masası aracısı | Satış aracısı | Kullanıcı yönetimi yöneticisi


## <a name="what-are-azure-reservations"></a>Azure Ayırmaları nedir?

Azure Rezervasyonları bir yıllık veya üç yıllık sanal makine, SQL Veritabanı işlem kapasitesi, Azure Cosmos DB aktarım hızı veya diğer Azure kaynakları için ön ödemeyle tasarruf etmeye yardımcı olur. Önceden ödeme yapmak, kullanmakta olduğu kaynaklarda indirim elde etmek için kullanılabilir. Rezervasyonlar, sanal makinenizi, SQL veritabanı işlem, Azure Cosmos DB ve diğer kaynak maliyetlerinizi, kullanım başına öde fiyatlarına kıyasla %72'ye varan oranda düşürebilirsiniz. Rezervasyonlar bir faturalandırma indirimi sağlar ve kaynaklarınızın çalışma zamanı durumunu etkilemez. Daha fazla bilgi için [bkz. Azure Rezervasyonları nedir?](/azure/billing/billing-save-compute-costs-reservations)

## <a name="why-should-customers-buy-a-reservation"></a>Müşteriler neden rezervasyon satın alsın?

Müşterilerin sanal makineleri, Azure Cosmos DB veya SQL uzun süre çalıştıran veritabanları varsa, rezervasyon satın almak onlara en uygun maliyetli seçeneği sunar. Örneğin, bir müşteri sürekli olarak rezervasyon olmadan bir hizmetin dört örneğini çalıştırırsa, bu müşteri, öde öde fiyatlarıyla ücret öder. Bu kaynaklar için rezervasyon satın almaları durumunda hemen rezervasyon indirimi elde edilir. Kaynaklar artık kullandıkça öde tarifelerine göre ücretlendirilmez.

### <a name="compelling-new-azure-offer-in-csp"></a>CSP'de Cazip Yeni Azure teklifi

Microsoft, Azure Rezervasyonları ve Sunucu Aboneliklerini CSP programına getirerek, iş ortaklarının yüksek oranda tahmin edilebilir, kalıcı bulut iş yüklerini desteklemek için daha uygun maliyetli çözümlere yönelik hızlı büyüyen müşteri talebini karşılamak için daha iyi bir seçenektir. CSP programı, iş ortaklarının Microsoft İş Ortağı Merkezi ve Azure portal aracılığıyla ticari müşteriler adına Azure Rezervasyonları ve Sunucu Abonelikleri satın Azure portal.
Hatta CSP programımızda iş ortaklarına Azure rezervasyonlarının nasıl satın alınarak satın alınlarına yardımcı olabiliriz. CSP iş ortakları bir müşteri adına [Azure](azure-reservations-buying.md) rezervasyonları satın alabilir veya müşterinin, iş ortağının kendileri için satın aldıklarından önceki bir Azure aboneliğinden kendi rezervasyonlarını satın almalarına olanak sağlar. [](give-customers-permission.md)

Azure Rezervasyonları müşterilere geliştirme ve test etme, uygulamaları çalıştırma ve veri merkezini genişletme gibi çok çeşitli bilgi işlem çözümleri için sanallaştırma esnekliği sağlar.

Örneğin [Azure Ayrılmış VM Örnekleri](https://azure.microsoft.com/pricing/reserved-vm-instances/) müşteriler artık yalnızca 1 veya 3 yıllık bir süre için sanal makineyi satın alarak veya "satın alarak" azure VM fiyatlandırması yerine %72'ye varan tasarruflar kullanabilir. Windows Azure Hibrit Avantajı ile birlikte Yazılım Güvencesi sunucu müşterileri, %80'e varan tasarruflar ve öde fiyatlandırması ile karşı karşıyadır.

Cazip fiyatlandırma ve eşleşmeyen dağıtım esnekliğinin eşleşmeyen bir bileşimiyle, müşteriler Azure Rezervasyonları'ı seçtikleriyle genel olarak en iyi değeri elde eder.

- [Bkz.](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) Azure Portal'da Rezervasyon satın alma.

- Yazılım abonelikleri ve Linux ISV **yıllık abonelikleri** için Microsoft Azure [](https://partner.microsoft.com/dashboard/sell/pricingandoffers) Fiyatlandırma ve Teklifler sayfasındaki Ayrılmış Örnekler İş Ortağı Merkezi kategorisi altındaki Azure **RI CSP** Ticari Fiyat Listesi'ne bakın.


 
**Linux ISV yıllık abonelikleri**

- SUSE Linux
- Red Hat Enterprise Linux
- Azure Red Hat OpenShift

**ISV yıllık abonelikleri**

- CloudSimple tarafından sunulan Azure VMware Çözümü

## <a name="getting-started"></a>Başlarken

Azure Rezervasyonlarını müşterilerinizle nasıl konumlandırmanız ve mümkün olan en kısa sürede çalışır duruma getirin ve çalışır duruma getirin, hazırlık malzemelerini gözden geçirmek için aşağıdaki yaklaşımı öneririz:

1. Yeni ticaret operasyonları kılavuzunu [İş Ortağı Merkezi ve anlıyoruz.](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)

2. [İş Ortağı Merkezi API'sinde (API/SDK) Azure Rezervasyonları ve Sunucu Abonelikleri güncelleştirmelerini anlama.](/partner-center/develop/purchase-azure-reserved-vm-instances)


### <a name="sales-readiness"></a>Satış için hazır olma

- [Uzak Masaüstü Hizmetleri (RDS) İstemci Erişim Lisansı (CAL) (duyuru)](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [Azure Ayrılmış VM Örnekleri (Azure portal)](/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [Sunucu Abonelikleri](./csp-software-subscriptions.md)

- [SQL VERITABANı Ayırmaları (Azure portal)](/azure/sql-database/sql-database-reserved-capacity)

- [Azure Cosmos DB (Azure portal)](/azure/cosmos-db/cosmos-db-reserved-capacity)

- [SQL Yönetilen Örnek (Azure portal)](/azure/sql-database/sql-database-managed-instance)

- [SUSE ve Red Hat Enterprise Linux (Azure portal)](/azure/virtual-machines/linux/prepay-suse-software-charges)

- [Azure'da Red Hat Linux](https://azure.com/redhat)

- [Azure'da SUSE Linux](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [Azure’da Linux](https://azure.microsoft.com/overview/linux-on-azure/)

- [Azure Fiyatlandırmaya Genel Bakış](https://azure.microsoft.com/pricing/)

- [Azure Fiyatlandırma Hesaplayıcısı](https://azure.microsoft.com/pricing/calculator)

- [Azure Databricks rezervasyonları](/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a>Eğitim

Ticari Lisans [hazırlığı web seminerlerini ve isteğe bağlı olayları](https://commercial-licensing.eventbuilder.com/FY2019_ALL) görüntülemek için kaydolabilirsiniz.
Önceden kaydedilen Lisanslama Hazırlığı isteğe bağlı olayları şunlar gibi konuları içerir:

- CSP Online Services, CSP Azure ve Azure dahil olmak üzere genel lisans güncelleştirmeleri (Kasım 2018)

- SQL VERITABANı Ayrılmış Kapasitesi & Örnek Boyutu Esnekliği (Ağustos 2018)

- CSP'de Sunucu Abonelikleri (Temmuz 2018)

- CSP'de Azure Rezervasyonlara Genel Bakış (Mayıs 2018)

## <a name="operations"></a>Operations

[İş Ortağı Merkezi](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)ticari işlemler kılavuzu: Sözleşmeler, İş Ortağı Merkezi aracılığıyla sipariş, fatura, fiyat listesi ayrıntıları, teşvikler, mutabakat dosyası, API/SDK, Korumalı Alan ve Azure İş Ortağı Paylaşılan Hizmetleri.

## <a name="azure-hybrid-benefit"></a>Azure Hibrit Avantajı

Bu [Azure Hibrit Avantajı,](https://azure.microsoft.com/pricing/hybrid-benefit) Yazılım Güvencesi lisansı olan müşteriler için fiyatlandırma avantajıdır. Bu avantaj, Azure'a geçen mevcut şirket içi Windows Server ve/veya SQL Server lisans yatırımlarının değerini en üst düzeye çıkarmanıza yardımcı olur. Uygun müşteriler Azure Sanal Makinelerde (hizmet olarak altyapı veya IaaS SQL Server) %40'a varan tasarruflar ve Azure Hibrit Avantajı Azure SQL Veritabanı (hizmet olarak platform veya PaaS) ile Azure Sanal Makinelerde (IaaS) %55'e varan tasarruflar ve Azure Ayrılmış Örnekleri ile birleştirildiklarında %80'e varan bir artış sağlar.

## <a name="next-steps"></a>Sonraki adımlar

- [Azure Hibrit Avantajı Hakkında SSS](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

*Gerçek tasarruflar bölgeye, örnek türüne veya kullanıma göre değişiklik gösterebilir.