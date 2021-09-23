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
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/23/2021
ms.locfileid: "128322428"
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
Müşteri adresi satırı 1|Yes|Müşteri şirketinin Adres satırı 1. |Tek contoso yöntemi
Müşteri adresi satırı 2|No|Müşteri şirketinin Adres satırı 2.|NE 148 Caddesi
Müşteri şehri|Yes|Müşteri kuruluşunun bulunduğu şehir.|Redmond
Müşteri durumu|No|Müşteri kuruluşunun bulunduğu eyalet.|Washington
Müşteri posta kodu|No|Müşteri kuruluşunun bulunduğu bölgenin posta kodu.|98052
Müşteri ülkesi|Yes|Müşteri kuruluşunun bulunduğu ülke/bölge. Bu [Ülke kodları listesinde](https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes), Iki harfli *Alfa-2 kodunu* kullanın.|ABD
Müşteri D-U-N-S KIMLIĞI|No|Müşteri kuruluşunun DÇALıŞTıRAL KIMLIĞINI getirmeye çalışın. Bu, daha hızlı satıcı atamasına yardımcı olan Microsoft tarafında müşteri kuruluşunun daha hızlı eşleştirmesine yardımcı olur. [D-U-N-S numara arama SAYFASıNDAN](https://www.dnb.com/duns-number/lookup.html)DELLER kimliğini ücretsiz olarak edinebilirsiniz.|81466849
Müşterinin kişi adı soyadı|Şekline|İlk adı yalnızca Microsoft Yardım 'a ihtiyacınız varsa zorunludur. Müşteri kuruluşundan bu anlaşma üzerinde çalışan birincil kişinin adı.|John
Müşterinin kişi adı soyadı|Şekline|Soyadı yalnızca Microsoft Yardım gerekirse zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil kişinin soyadı.|Müşteri
müşteri iletişim Telefon numarası|Şekline|Telefon numarası yalnızca Microsoft yardım gerekirse zorunludur. bu işlem sırasında çalışan müşteri kuruluşundaki birincil ilgili kişinin Telefon numarası.|9999999999
Müşteri Iletişim e-posta adresi|Şekline|E-posta adresi yalnızca Microsoft Yardım 'a ihtiyacınız varsa zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil kişinin e-posta adresi.|john.customer@contoso.com
İş ortağı başvuru durumu|Yes|Şirketinizin perspektifinden ilgili durumunu gösterir. Bir başvuruyu oluşturmaya veya değiştirmeye çalışıyorsanız gereklidir. Yeni bir anlaşma oluşturmaya çalışıyorsanız **Yeni** ' ye kullanın. Kullanabileceğiniz değerler [başvuru kaynaklarında](/partner/develop/referral-resources#referralstatus)listelenmiştir.|Etkin
İş ortağı başvurusu alt durumu|Yes|İşlem durumunun tam durumunu gösterir. Yeni bir anlaşma oluşturmaya çalışıyorsanız **kabul edildi** ' i kullanın. Mevcut bir başvuruyu değiştiriyorsanız de gereklidir. Kullanabileceğiniz değerler [başvuru kaynaklarında](/partner/develop/referral-resources#referralsubstatus)listelenmiştir.|Kabul edildi
Microsoft başvuru durumu|Şekline|Microsoft arama yardımı 'na gönderdiğiniz ortak satış isteğinin durumunu gösterir. Bu salt okunurdur. Verilerin içeri aktarılması sırasında bu alanda yapılan herhangi bir değişiklik yok sayılır.| Beklemede
Reddedilen/kayıp nedeni|Şekline| Bu bilgileri yalnızca, alanın alt durumunu reddedilmiş veya kayıp olarak değiştiriyorsanız sağlamanız gerekir. Bu sütunu, aksi takdirde yoksayabilirsiniz. <br/> **Aşağıdaki seçeneklere göre bir sayı girin** <br/><br/> **1**-Project bütçe yeterli değil  <br/> **2**-müşteri yanıt vermedi  <br/> **3**-müşteri başka bir satıcı seçti  <br/> **4** -müşteri gereksinimi karşılanmadı  <br/> **5** -müşteri değil <br/> **6**-önerilen zaman satırı çok kısa <br/> **7** -kötüye kullanma, istenmeyen posta veya kimlik avı olarak raporla <br/> **8** -diğerleri |6|
Satış Aşaması|No|Bu, başvurunun ayrıntılı satış aşamasını belirten alandır. Satış aşamaları hakkında daha fazla bilgi edinmek için [Iş Ortağı Merkezi 'nde ortak satış fırsatlarını yönetin](./manage-co-sell-opportunities.md)|40
Tahmini anlaşma değeri|Yes|Müşteriyle ilk konuşmaları temel alan işlem değeri. Bu, bu durum, işlem, **kazanılan** veya kaybolan Terminal durumlarından birine ulaştığında değiştirilebilir **.**|12563
Para Birimi|Yes|Anlaşma değerinin girildiği para birimi. Para birimi kodlarını [ıso 4217 vican sayfasında](https://en.wikipedia.org/wiki/ISO_4217)bulabilirsiniz.|USD
Tahmini Kapatma Tarihi|Yes|AA/D/YYYY biçiminde müşteriyle yapılan ilk konuşmaları temel alarak satış anlaşması tahmini kapanış tarihi. <br/> **Tarih UTC saat diliminde olmalıdır. Kullanıcı arabiriminde görüntülenen İş Ortağı Merkezi tarihler yerelleştirilmiş saat dilimlerini temel almaktadır. UTC saat diliminde tarihi temin edilen referansa bakıyorsanız kullanıcı arabiriminde +/- bir gün fark İş Ortağı Merkezi olabilir.**|1/30/2020
CRM Kimliği|No|Varsa CRM sisteminize bu referansı tanımlayıcı. Bu, serbest biçimli bir metin girişi alanıdır.|34234324-sdfsdf-345345-sfd
Pazarlama Kampanyası Kimliği|No|Bu alan, pazarlama kampanyasının bu referansla sonuçlanmasına neden olduğunu gösterir. Genellikle yatırım getiri hesaplaması için kullanılır|BingSummer2020
Notlar|No|Referansla ilgili güncelleştirmeleri gösteren ayrıntılı notlar|Bu örnek bir not
Microsoft yardım gerekiyor mu?|Yes|Bu, Microsoft'un bu ortak satış isteği için size yardımcı olup olmadığını belirtmektir|Yes
Microsoft'tan hangi özel yardım?|-Sına bağ -lıdır|Microsoft'un size yardımcı olmak için altı farklı yoldan biri. Bu yalnızca "Microsoft yardımı gerekiyor mu? sorusu için Evet'i seçerseniz geçerlidir. " <br/> **Aşağıdaki seçeneklere göre bir sayı girin** <br/><br/> **1**- İş yükü - belirli bir değer teklifi  <br/> **2**- Müşteri teknik mimarisi  <br/> **3**- Kavram kanıtı /Tanıtım  <br/> **4**- Teklifler ve Lisanslama  <br/> **5**- Gönderi - satış müşteri başarısı  <br/> **6**- Genel veya diğer|1|
Microsoft satış ekibiyle paylaşma|Yes|Bu, satış anlaşmasıyla ilgili ayrıntıları Microsoft satış ekibiyle paylaşmak isteyip istemeyebilirsiniz. Bu yalnızca "Microsoft yardımı gerekiyor mu? sorusu için Hayır'ı seçerseniz geçerlidir. "|Yes
Microsoft'a notlar|No|Microsoft'tan yardıma ihtiyacınız varsa Microsoft'a özgü notlar|Contoso müşterisi için POC ile ilgili yardım gerekiyor
Müşteri/İş Ortağı kişisi paylaşma onayı|Yes|Müşterinin iletişim ayrıntılarını ve şirket çalışanlarının anlaşma üzerinde çalışan kişi ayrıntılarını paylaşma onayı. **Bu sütun için Hayır'ı seçerseniz anlaşmalar oluşturulmaz veya güncelleştirilmez.** |Yes
CLA Numarası|-Sına bağ -lıdır|IOT anlaşması oluşturulurken veya güncelleştirilken CLA numarası gerekli değildir. Tasarım kazanma aşamasına geçilende gerekli hale gelir.
Cihaz Kategorisi|No|Tüm IoT cihaz kategorilerinin listesi. Aşağıdaki seçeneklerden bir kategori seçin <br>Bilgisayar/Tüketici Oyun Cihazı <br> ATM <br> Otomotiv & Taşımacılık Sistemleri <br> Azure Sphere Panosu<br> Azure Sphere Bileşeni <br> Azure Sphere Koruyucu<br> Azure Sphere Modülü <br> Bina Otomasyonu<br> Gaming Oyun Cihazı <br> İletişim Cihazları<br> Tüketici İnternet Cihazı <br> Tüketici Yıpranabilir<br> Dijital Resim Çerçevesi <br> Dijital Tabela <br> Ağ geçidi <br> HHT/Mobil<br> Endüstriyel Otomasyon Cihazı<br> Sektör Tableti (POS Olmayan) <br> Bilgi noktası<br> Media Player<br> Medya Cihazı <br> Mobil POS <br> Gezinti Cihazı<br> Ağ Projektörü<br> Diğer<br> Diğer Bankacılık Cihazı<br> Diğer Tüketici Elektronik Cihazı<br> Diğer Cihaz<br> Diğer Enterprise Cihazı<br>  Diğer Algılayıcı/Düğüm <br> Satış Noktası Cihazı<br> Cihazı Yazdırma <br> Güvenlik/İzleme <br>  Sunucu<br> Set-Top Box<br> Akıllı TV <br> Test ve Ölçüm Cihazı<br> İnce İstemci Cihazı <br/>
Silikon Türü|No|Aşağıdaki listeden bir seçenek seçerek Yonga kümesi modeli bilgilerini girin <br> AMD - A10 <br> AMD-A4 <br> AMD-A6 <br> AMD-A8 <br> AMD-E2 <br> AMD-FX 7500 <br> AMD-FX 7600P <br> AMD-FX 9370 <br> AMD-FX 9590 <br> AMD-G serisi <br> AMD-diğerleri <br> AMD-R serisi <br> AMD-FX modellerinin geri kalanı <br> Intel-Atom <br> Intel-Celeron-N1900 <br> Intel-Celeron-N2807 <br> Intel-Celeron-N2930 <br> Intel-Celeron-N3060 <br> Intel-Celeron-N3160 <br> Intel-Core i3 <br> Intel-Core i5 <br> Intel-Core i7 <br> Intel-Core d <br> Intel-diğerleri <br> Intel-Pentium <br> Intel-Celeron 'nin geri kalanı <br> Intel-XEON <br> MediaTek MT3620 <br> NXP 8ULP-CS <br> Diğer <br/>
Azure Sertifikalı cihaz|No|Bu, cihaz için Azure uyumluluk sertifikası 'nın elde edildiğini belirtir
Hizmetleri Ekle|No|Bu, Azure hizmetlerinin dağıtımda IoT çözümüyle birlikte paketlenebilir olduğunu belirtir
Microsoft MSX KIMLIĞI|No|Yalnızca ortak satış fırsatları için kullanılabilen Microsoft MSX sisteminde bir işlem KIMLIĞI
Geçirilen PSC anlaşma KIMLIĞI|No|PSC anlaşma KIMLIĞI, yalnızca PSC 'den BILGISAYARA geçirilen bir anlaşma için kullanılabilir
MPN Kimliği|No|MPN ortak satış fırsatlarının oluşturulduğu kuruluşun KIMLIĞI
1\. Çözüm|Yes|Çözüm KIMLIĞI (gerekli), anlaşma değerinin girildiği para birimi (isteğe bağlı). [Para birimi kodlarını](https://en.wikipedia.org/wiki/ISO_4217), SKU 'nun fiyatını (isteğe bağlı) ve SKU 'nun miktarını bulabilirsiniz (isteğe bağlı)  |NUEVO-1234-PQRS, USD, 10, 100
Takım üyesi 1|Yes|İlgili takım üyesinin adı, soyadı, cep telefonu numarası ve e-posta KIMLIĞI.| Bob, Iş ortağı, 999999, Bob.partner@Contoso.com
Microsoft takım üyesi 1|No|Ortak satış fırsatı üzerinde çalışan ilgili Microsoft ekibi üyesinin adı, soyadı, cep telefonu numarası ve e-posta KIMLIĞI.| Sam, satıcı, 999999, Sam.seller@Microsoft.com

## <a name="next-steps"></a>Sonraki adımlar

Bu Iş Ortağı Merkezi ortak satış bağlayıcılarını, CRM sistemlerinizden Microsoft ile birlikte satın almak için kullanabilirsiniz.

- [Dynamics 365 CRM için ortak satış Bağlayıcısı – genel bakış](connector-dynamics.md)
- [Salesforce için ortak satış Bağlayıcısı CRM-genel bakış](connector-salesforce.md)
