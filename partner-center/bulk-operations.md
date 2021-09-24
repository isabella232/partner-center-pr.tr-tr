---
title: başvurularda Excel/csv dosyaları aracılığıyla ortak satış fırsatlarını toplu dışa aktarma ve içeri aktarma
description: iş ortağı merkezi 'nde Excel (CSV) dosyalarını kullanarak ortak satış fırsatlarını indirme, oluşturma veya güncelleştirme hakkında bilgi edinin
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 09/08/2021
ms.openlocfilehash: a87b44bb2730faf87bfaaf25b5e051b0ce4f6f30
ms.sourcegitcommit: fb9ca808f6362e81d65a6ba5770dc8820834a0ed
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/24/2021
ms.locfileid: "128360194"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Virgülle ayrılmış değer (CSV) dosyaları kullanan ortak satış fırsatları için toplu işlemler

**Uygun roller**: başvuru Yöneticisi | Başvuru kullanıcısı

İş Ortağı Merkezi'ndeki toplu işlemler şirketinizin ortak satış fırsatı verilerini dışarı ve içeri aktarmasına yardımcı olur. Sayfa başlığı başlığının sağ üst köşesindeki **içeri** ve **dışarı aktarma** bağlantılarını bulmak için **ortak satış fırsatları** sayfasına gidin. Hem **Referans yöneticisi** hem de **Referans Kullanıcısı** izinleri olan kullanıcılar bu işlevselliği kullanabilir.

> [!IMPORTANT]
> Toplu içeri aktarma aracılığıyla gerçekleştirilen oluşturma/güncelleştirme eylemleri geri alınamaz. Çok fazla sayıda kaydı değiştirir veya oluştururken dikkatli olun. Satış anlaşması oluşturulduktan sonra alanların yalnızca bir alt kümesi değiştirilebilir. **Satış anlaşması Reddedildi/Süresi Doldu/Kazanıldı/Kaybedildi gibi bir son duruma ulaştığında hiçbir eyleme izin verilmez.**

## <a name="export-co-sell-opportunities"></a>Ortak satış fırsatlarını dışarı aktarma

Aşağıdaki bilgiler dışa aktarma işlevini açıklar:

- **Dışarı aktar** düğmesine tıklayarak **en fazla 5000 kaydı** dışarı aktarabilirsiniz.
- İndirilen anlaşmalar erişim düzeylerinizi temel alır. Başvuru yöneticileri ve başvuru kullanıcıları, kapsamlarına bağlı olarak farklı sonuçlar alabilir ve ekipteki ekip üyeleri olarak dahil edebilir. [Başvurular izinleri](permissions-overview.md#manage-referrals)hakkında daha fazla bilgi edinin.
- Dışa aktarma işlevi, ortak satış fırsatları sayfasında geçerli sekmeyi ve uygulanan filtreleri hesaba göre alır.
- Uygulanan filtreleri temel alan tüm verileri içeren bir CSV dosyası oluşturulacaktır.
- Kayıtların indirilmesi bir dakika kadar sürebilir.
- İndirme eyleminin tamamlanmasını beklemeniz gerekmez. Iş Ortağı Merkezi 'nde diğer sayfalara gitseniz bile, dışa aktarma işlevi tamamlandıktan hemen sonra dosya indirilir.
- İndirilen dosyayı, işlem ayrıntılarını değiştirmek ve kayıtları güncelleştirmek üzere karşıya yüklemek için yeniden kullanabilirsiniz.

## <a name="import-co-sell-opportunities"></a>Ortak satış fırsatlarını içeri aktarma

- İçeri aktarma işlevini kullanarak **en fazla 1000 kayıt** oluşturabilir veya güncelleyebilirsiniz.
- Şablonu, Iş ortağı merkezindeki Içeri aktarma sayfasından indirerek sıfırdan oluşturabilirsiniz.
- Ayrıca, var olan kayıtları indirmek ve güncelleştirmek için dışarı aktarma işlevini de kullanabilirsiniz.
- Dosyada 1000 'den fazla kayıt varsa, işlem işlenemiyor.
- Dosya işlendikten sonra, oluşturulan, güncellenen ve işlenmemiş başvuruların sayısına sahip bir Özet, son işlem dosyası kartında gösterilir.
- İşlenen kayıtların ayrıntılarını indirebilir, hataları giderebilir ve önceki çalıştırmada başarısız olan kayıtları oluşturmak veya güncelleştirmek için aynı dosyayı karşıya yükleyebilirsiniz. **Önceki çalıştırmada başarısız olan düzeltilen kayıtları karşıya yüklemeden önce dosyadaki tüm başarılı kayıtları kaldırın.**
- Daha fazla çözüm eklemek için, çözüm 1 ' in yanına ek sütunlar ekleyin ve sütun adını çözüm X olarak kullanın; burada X, anlaşma içindeki çözümün numarasını temsil eder. Örneğin, çözüm 2, çözüm 3.
- Bir başa 50 çözüm ekleyebilirsiniz.
- Daha fazla takım üyesi eklemek için, takım üyesi 1 ' in yanına ek sütunlar ekleyin ve sütun adını takım üyesi X olarak kullanın; burada X, anlaşma içindeki takım üyesinin numarasını temsil eder. Örneğin, takım üyesi 2, takım üyesi 3.
- Bir anlaşma için en fazla 50 takım üyesi ekleyebilirsiniz.

> [!NOTE]
> İşlemin tamamlanmasını beklemeniz gerekmez. İşlenen son dosyanın ayrıntıları, işlem tamamlandıktan sonra indirilecektir. **1000 kayıtla dosya yüklüyorsanız, bu işlem 10 dakikaya kadar sürebilir.**

> [!IMPORTANT]
> Tüm yönergeleri dikkatle okuyun ve Iş Ortağı Merkezi 'nde CSV dosyalarını kullanarak anlaşmalar oluşturmadan veya güncelleştirmeden önce aşağıdaki tablodaki her bir sütunun biçimini denetleyin.

Şablondaki her alan düzenlenemez. Her zaman salt okunurdur, bazıları başvuru oluşturulduktan sonra salt okuma durumuna değişecektir ve bazıları belirli bir değerle değiştirildikten sonra salt yazılır olarak değişecektir.

### <a name="fields-that-are-always-read-only"></a>Her zaman salt okunan alanlar

- Hatalar
- Katılım KIMLIĞI
- Referans kimliği
- Microsoft başvuru durumu
- Microsoft MSX KIMLIĞI
- Geçirilen PSC anlaşma KIMLIĞI
- Microsoft takım üyesi

### <a name="fields-that-will-become-read-only-after-you-create-the-referral"></a>Başvuruyu oluşturduktan sonra Salt okunabilir olacak alanlar

- Müşteri Adı
- Müşteri adresi satırı 1
- Müşteri adresi satırı 2
- Müşteri şehri
- Müşteri durumu
- Müşteri posta kodu
- Müşteri ülkesi
- Müşteri D-U-N-S KIMLIĞI
- Müşteri/Iş ortağı ilgili kişisini paylaşma onayı
- MPN Kimliği

### <a name="fields-that-will-become-read-only-after-you-first-share-them"></a>İlk paylaşmadan sonra salt okunan alanlar

- Ortak satış başvurusu oluşturma veya yükseltme ayrıntılarını gönderdikten sonra **Müşteri Iletişim adı Ilk adı** salt okunurdur.
- Ortak satış başvurusu oluşturma veya yükseltme ayrıntılarını gönderdikten sonra **Müşteri Irtibat son adı** salt okunurdur.
- ortak satış başvurusu oluşturma veya yükseltme ayrıntılarını gönderdikten sonra **müşteri iletişim Telefon numarası** salt okunurdur.
- Ortak satış başvurusu oluşturma veya yükseltme ayrıntılarını gönderdikten sonra **Müşteri Iletişim e-posta adresi** salt okunurdur.
- **Microsoft yardımı gerekli mi?** , Evet olarak işaretlendikten sonra salt okunurdur
- **Microsoft 'a özgü yardım nedir?** , belirtilen biçimde bir sayı girdikten sonra salt okunurdur
- **Microsoft satış ekibi Ile paylaşma** , Evet olarak işaretlendikten sonra salt okunurdur.
- Ortak satış başvurusu oluşturma veya yükseltme için notları gönderdikten sonra, **Microsoft 'A notlar** salt okunurdur.

Tüm sütunların ayrıntıları ve örnek değerleri aşağıdaki tabloda verilmiştir.

|**Sütun adı**|**Zorunlu mu?**|**Açıklama**|**Örnek değer (ler)**|
|-----|:-----|:---------|:---|
Hatalar|No|Başvurular için oluşturma/güncelleştirme işlemleriyle ilgili varsa hatalar bu sütuna dahil edilir. Birden çok hata varsa, bunların hepsi noktalı virgülle ayrılmış olarak listelenir.|Zorunlu alan çözümü 1 eksik|
Katılım KIMLIĞI|Yes|Katılım KIMLIĞI, Microsoft Iş Ortağı Merkezi başvuruları sistemi tarafından oluşturulur. Yeni başvuru oluşturma için gerekli değildir. Bir kaydı güncelleştiriyorsanız, var olan katılım KIMLIĞINI kullanabilirsiniz.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Referans kimliği|Yes|Başvuru KIMLIĞI, Microsoft Iş Ortağı Merkezi başvuruları sistemi tarafından oluşturulur. Yeni başvuru oluşturma için gerekli değildir. Mevcut bir kaydı güncelleştiriyorsanız, bunu referans KIMLIĞIYLE doldurabilirsiniz.|ebacdkdc-0b84-4ac4-B4EA-5b2587d42cee
Anlaşma adı|Yes|Başvurunuz için anlaşma için kolay ad.|UK yay
Müşteri Adı|Yes|Müşteri şirketinin adı. Microsoft tarafında hızlı eşleştirme için kuruluşun yasal adını kullanın.|Contoso Corporation
Müşteri Adres Satırı 1|Yes|Müşteri şirketinin 1. satırına adresle. |Tek Contoso Yolu
Müşteri Adres Satırı 2|No|Müşteri şirketinin 2. adres satırı.|NE 148 sokağı
Customer City|Yes|Müşteri kuruluşlarının bulunduğu şehir.|Redmond
Müşteri Durumu|No|Müşteri kuruluşlarının bulunduğu yeri ifade.|Washington
Müşteri Posta Kodu|No|Müşteri kuruluşlarının bulunduğu bölgenin Posta Kodu.|98052
Müşteri Ülkesi|Yes|Müşteri kuruluşlarının bulunduğu Ülke/Bölge. Ülke kodları listesinde *iki harfli Alfa-2* [kodunu kullanın.](https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)|ABD
Müşteri D-U-N-S Kimliği|No|Müşteri kuruluşlarının DUNS kimliğini getirmeye çalışma. Bu, Microsoft tarafında müşteri kuruluşlarının daha hızlı eşleşmesi için yardımcı olur ve bu da satıcı atamalarının daha hızlı tamamlansa da yardımcı olur. [D-U-N-S](https://www.dnb.com/duns-number/lookup.html)Numarası Arama sayfasından DUNS ID ÜCRETSİZ elde edebilirsiniz.|81466849
Müşteri Kişisi Adı|-Sına bağ -lıdır|Ad yalnızca Microsoft yardıma ihtiyacınız varsa zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil ilgili kişinin adı.|John
Müşteri Kişisi Soyadı|-Sına bağ -lıdır|Soyadı yalnızca Microsoft yardıma ihtiyacınız varsa zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil ilgili kişinin soyadı.|Müşteri
Müşteri İletişim Telefon numarası|-Sına bağ -lıdır|Telefon numarası yalnızca Microsoft yardıma ihtiyacınız varsa zorunludur. Telefon satış anlaşması üzerinde çalışan müşteri kuruluşundan birincil ilgili kişinin numarasını girin.|9999999999
Müşteri İletişim e-posta Adresi|-Sına bağ -lıdır|E-posta adresi yalnızca Microsoft yardıma ihtiyacınız varsa zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil ilgili kişinin e-posta adresi.|john.customer@contoso.com
İş Ortağı Referans Durumu|Yes|Şirketin bakış açısından anlaşma durumunu gösterir. Bir referans oluşturmak veya değiştirmek için çalışıyorsanız gereklidir. Yeni **bir** satış anlaşması oluşturmak için Yeni'leri kullanın. Kullanabileceğiniz değerler Referans [kaynakları'nda listelenir.](/partner/develop/referral-resources#referralstatus)|Etkin
İş Ortağı Referansı Alt İstatistikleri|Yes|Anlaşmanın tam durumunu gösterir. Yeni bir satış anlaşması oluşturmak için **Accepted** kullanın. Mevcut bir referansı değiştirirken de gereklidir. Kullanabileceğiniz değerler Referans [kaynakları'nda listelenir.](/partner/develop/referral-resources#referralsubstatus)|Kabul edildi
Microsoft Referans Durumu|-Sına bağ -lıdır|Yardım almak için Microsoft'a gönderdiğiniz ortak satış isteğinin durumunu gösterir. Bu salt okunur bir alandır. Veriler içeri aktarılırken bu alanda yapılan tüm değişiklik yoksayılır.| Beklemede
Reddedildi/Neden kaybedildi|-Sına bağ -lıdır| Bu bilgileri yalnızca alanınıza ilişkin alt durumu Reddedildi veya Kayıp olarak değiştirerek sağlamanız gerekir. Aksi takdirde bu sütunu yoksayabilirsiniz. <br/> **Aşağıdaki seçeneklere göre bir sayı girin** <br/><br/> **1**- Project bütçe yeterli değil  <br/> **2**- Müşteri yanıt vermedi  <br/> **3**- Müşteri başka bir satıcı seçti  <br/> **4** - Müşteri gereksinimi karşılanmaz  <br/> **5** - Müşteri değil <br/> **6**- Önerilen zaman çizgisi çok kısa <br/> **7** - Kötüye kullanım, istenmeyen posta veya kimlik avı olarak bildirme <br/> **8** - Diğer |6|
Satış Aşaması|No|Bu, referans için ayrıntılı satış aşamalarını gösteren alandır. Satış aşamaları hakkında daha fazla bilgi için [şu makaleyi okuyun:](./manage-co-sell-opportunities.md) İş Ortağı Merkezi|40
Tahmini Satış Değeri|Yes|Müşteriyle yapılan ilk konuşmaları temel alan satış anlaşması değeri. Anlaşma kazanildi veya kaybedildi terminal durumlarından biri olana kadar bu **değiştirilebilir.** |12563
Para Birimi|Yes|Anlaşma değerinin girilir olduğu para birimi. Para birimi kodlarını [ISO 4217 Wikipedia sayfasında bulabilirsiniz.](https://en.wikipedia.org/wiki/ISO_4217)|USD
Tahmini Kapatma Tarihi|Yes|AA/D/YYYY biçiminde müşteriyle yapılan ilk konuşmaları temel alarak satış anlaşması tahmini kapanış tarihi. <br/> **Tarih UTC saat diliminde olmalıdır. Kullanıcı arabiriminde görüntülenen İş Ortağı Merkezi tarihler yerelleştirilmiş saat dilimlerini temel almaktadır. UTC saat diliminde tarihi temin edilen referansa bakıyorsanız kullanıcı arabiriminde +/- İş Ortağı Merkezi bir günlük fark olabilir.**|1/30/2020
CRM Kimliği|No|Varsa CRM sisteminize bu referansı tanımlayıcı. Bu, serbest biçimli bir metin girişi alanıdır.|34234324-sdfsdf-345345-sfd
Pazarlama Kampanyası Kimliği|No|Bu alan, pazarlama kampanyasının bu referansla sonuçlanmasına neden olduğunu gösterir. Genellikle yatırım getiri hesaplaması için kullanılır|BingSummer2020
Notlar|No|Referansla ilgili güncelleştirmeleri gösteren ayrıntılı notlar|Bu örnek bir not
Microsoft yardım gerekiyor mu?|Yes|Bu, Microsoft'un bu ortak satış isteği için size yardımcı olup olmadığını belirtmektir|Yes
Microsoft'tan hangi özel yardım?|-Sına bağ -lıdır|Microsoft'un size yardımcı olmak için altı farklı yoldan biri. Bu yalnızca "Microsoft yardımı gerekiyor mu? sorusu için Evet'i seçerseniz geçerlidir. " <br/> **Aşağıdaki seçeneklere göre bir sayı girin** <br/><br/> **1**- İş yükü - belirli bir değer teklifi  <br/> **2**- Müşteri teknik mimarisi  <br/> **3**- Kavram kanıtı /Tanıtım  <br/> **4**- Teklifler ve Lisanslama  <br/> **5**- Gönderi - satış müşteri başarısı  <br/> **6**- Genel veya diğer|1|
Microsoft satış ekibiyle paylaşma|Yes|Bu, satış anlaşmasıyla ilgili ayrıntıları Microsoft satış ekibiyle paylaşmak isteyip istemeyebilirsiniz. Bu yalnızca "Microsoft yardımı gerekiyor mu? sorusu için Hayır'ı seçerseniz geçerlidir. "|Yes
Microsoft'a notlar|No|Microsoft'tan yardıma ihtiyacınız varsa Microsoft'a özgü notlar|Contoso müşterisi için POC ile ilgili yardım gerekiyor
Müşteri/İş Ortağı kişisi paylaşma onayı|Yes|Müşterinin iletişim ayrıntılarını ve şirket çalışanlarının anlaşma üzerinde çalışan kişi ayrıntılarını paylaşma onayı. **Bu sütun için Hayır'ı seçerseniz anlaşmalar oluşturulmaz veya güncelleştirilmez.** |Yes
CLA Numarası|-Sına bağ -lıdır|IOT anlaşması oluşturulurken veya güncelleştirilken CLA numarası gerekli değildir. Tasarım kazanma aşamasına geçilende gerekli hale gelir.
Cihaz Kategorisi|No|Tüm IoT cihaz kategorilerinin listesi. Aşağıdaki seçeneklerden bir kategori seçin <br>Bilgisayar/Tüketici Oyun Cihazı <br> ATM <br> Otomotiv & Taşımacılık Sistemleri <br> Azure Sphere Panosu<br> Azure Sphere Bileşeni <br> Azure Sphere Koruyucu<br> Azure Sphere Modülü <br> Bina Otomasyonu<br> Gaming Oyun Cihazı <br> İletişim Cihazları<br> Tüketici İnternet Cihazı <br> Tüketici Yıpranabilir<br> Dijital Resim Çerçevesi <br> Dijital Tabela <br> Ağ geçidi <br> HHT/Mobil<br> Endüstriyel Otomasyon Cihazı<br> Sektör Tableti (POS Olmayan) <br> Bilgi noktası<br> Media Player<br> Medya Cihazı <br> Mobil POS <br> Gezinti Cihazı<br> Ağ Projektörü<br> Diğer<br> Diğer Bankacılık Cihazı<br> Diğer Tüketici Elektronik Cihazı<br> Diğer Cihaz<br> Diğer Enterprise Cihaz<br>  Diğer Algılayıcı/Düğüm <br> Satış Noktası Cihazı<br> Cihazı Yazdırma <br> Güvenlik/İzleme <br>  Sunucu<br> Set-Top Box<br> Akıllı TV <br> Test ve Ölçüm Cihazı<br> İnce İstemci Cihazı <br/>
Silikon Türü|No|Aşağıdaki listeden bir seçenek seçerek Yonga kümesi modeli bilgilerini girin <br> AMD - A10 <br> AMD - A4 <br> AMD - A6 <br> AMD - A8 <br> AMD - E2 <br> AMD - FX 7500 <br> AMD - FX 7600P <br> AMD - FX 9370 <br> AMD - FX 9590 <br> AMD - G Serisi <br> AMD - Diğerleri <br> AMD - R Serisi <br> AMD - FX Modellerinin Geri Kalanı <br> Intel - Atom <br> Intel - Celeron - N1900 <br> Intel - Celeron - N2807 <br> Intel - Celeron - N2930 <br> Intel - Celeron - N3060 <br> Intel - Celeron - N3160 <br> Intel - Core i3 <br> Intel - Core i5 <br> Intel - Core i7 <br> Intel - Core M <br> Intel - Diğerleri <br> Intel - Pentium <br> Intel - Celeron'un geri kalanı <br> Intel - XEON <br> MediaTek MT3620 <br> NXP 8ULP-CS <br> Diğer <br/>
Azure Sertifikalı Cihaz|No|Bu, cihaz için Azure uyumluluk sertifikasının sağlanmıştır
Hizmet Ekleme|No|Bu, Azure hizmetlerinin dağıtım sırasında IoT çözümüyle paketlen mi olacağını belirtmektir
Microsoft MSX Kimliği|No|Microsoft MSX sisteminde yalnızca ortak satış fırsatları için kullanılabilen bir satış anlaşması kimliği
Geçirilen PSC Anlaşma Kimliği|No|PSC anlaşma kimliği, yalnızca PSC'den PC'ye geçirilen bir anlaşma için kullanılabilir
MPN Kimliği|No|Ortak satış fırsatlarının oluşturulacak olduğu kuruluşun MPN kimliği
1\. Çözüm|Yes|Çözüm Kimliği (gerekli), Anlaşma değerinin girilir olduğu para birimi (isteğe bağlı). Para birimi [kodlarını,](https://en.wikipedia.org/wiki/ISO_4217)SKU'nun fiyatını (isteğe bağlı) ve SKU miktarı (isteğe bağlı) bulabilirsiniz  |SOL-1234-PQRS, USD, 10, 100
Takım üyesi 1|Yes|İlgili ekip üyesinin ad, Soyadı, mobil numarası ve e-posta kimliği.| Bob, Partner, 999999, Bob.partner@Contoso.com
Microsoft ekip üyesi 1|No|Ortak satış fırsatı üzerinde çalışan ilgili Microsoft ekip üyesinin ad, Soyadı, mobil numarası ve e-posta kimliği.| Sam, Seller, 999999, Sam.seller@Microsoft.com

## <a name="next-steps"></a>Sonraki adımlar

CRM sistemlerinizin İş Ortağı Merkezi Microsoft ile ortak satış yapmak için bu ortak satış bağlayıcılarını kullanabilirsiniz.

- [Dynamics 365 CRM için ortak satış bağlayıcısı – Genel Bakış](connector-dynamics.md)
- [Salesforce CRM için ortak satış bağlayıcısı - genel bakış](connector-salesforce.md)
