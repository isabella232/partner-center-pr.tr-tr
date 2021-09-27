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
ms.openlocfilehash: d224a06304adbac03534eedd03b78f3db78f306e
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/27/2021
ms.locfileid: "129072469"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Ortak satış fırsatları için virgülle ayrılmış değer (CSV) dosyalarının kullanıldığı toplu işlemler

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
Hatalar|Hayır|Başvurular için oluşturma/güncelleştirme işlemleriyle ilgili varsa hatalar bu sütuna dahil edilir. Birden çok hata varsa, bunların hepsi noktalı virgülle ayrılmış olarak listelenir.|Zorunlu alan çözümü 1 eksik|
Katılım KIMLIĞI|Yes|Katılım KIMLIĞI, Microsoft Iş Ortağı Merkezi başvuruları sistemi tarafından oluşturulur. Yeni başvuru oluşturma için gerekli değildir. Bir kaydı güncelleştiriyorsanız, var olan katılım KIMLIĞINI kullanabilirsiniz.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Referans kimliği|Yes|Başvuru KIMLIĞI, Microsoft Iş Ortağı Merkezi başvuruları sistemi tarafından oluşturulur. Yeni başvuru oluşturma için gerekli değildir. Mevcut bir kaydı güncelleştiriyorsanız, bunu referans KIMLIĞIYLE doldurabilirsiniz.|ebacdkdc-0b84-4ac4-B4EA-5b2587d42cee
Anlaşma adı|Yes|Başvurunuz için anlaşma için kolay ad.|UK yay
Müşteri Adı|Yes|Müşteri şirketinin adı. Microsoft tarafında hızlı eşleştirme için kuruluşun yasal adını kullanın.|Contoso Corporation
Müşteri adresi satırı 1|Yes|Müşteri şirketinin Adres satırı 1. |Tek contoso yöntemi
Müşteri adresi satırı 2|Hayır|Müşteri şirketinin Adres satırı 2.|NE 148 Caddesi
Müşteri şehri|Yes|Müşteri kuruluşunun bulunduğu şehir.|Redmond
Müşteri durumu|Hayır|Müşteri kuruluşunun bulunduğu eyalet.|Washington
Müşteri posta kodu|Hayır|Müşteri kuruluşunun bulunduğu bölgenin posta kodu.|98052
Müşteri ülkesi|Yes|Müşteri kuruluşunun bulunduğu ülke/bölge. Bu [Ülke kodları listesinde](https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes), Iki harfli *Alfa-2 kodunu* kullanın.|ABD
Müşteri D-U-N-S KIMLIĞI|Hayır|Müşteri kuruluşunun DÇALıŞTıRAL KIMLIĞINI getirmeye çalışın. Bu, daha hızlı satıcı atamasına yardımcı olan Microsoft tarafında müşteri kuruluşunun daha hızlı eşleştirmesine yardımcı olur. [D-U-N-S numara arama SAYFASıNDAN](https://www.dnb.com/duns-number/lookup.html)DELLER kimliğini ücretsiz olarak edinebilirsiniz.|81466849
Müşterinin kişi adı soyadı|Şekline|İlk adı yalnızca Microsoft Yardım 'a ihtiyacınız varsa zorunludur. Müşteri kuruluşundan bu anlaşma üzerinde çalışan birincil kişinin adı.|John
Müşterinin kişi adı soyadı|Şekline|Soyadı yalnızca Microsoft Yardım gerekirse zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil kişinin soyadı.|Müşteri
müşteri iletişim Telefon numarası|Şekline|Telefon numarası yalnızca Microsoft yardım gerekirse zorunludur. bu işlem sırasında çalışan müşteri kuruluşundaki birincil ilgili kişinin Telefon numarası.|9999999999
Müşteri Iletişim e-posta adresi|Şekline|E-posta adresi yalnızca Microsoft Yardım 'a ihtiyacınız varsa zorunludur. Bu anlaşma üzerinde çalışan müşteri kuruluşundan birincil kişinin e-posta adresi.|john.customer@contoso.com
İş ortağı başvuru durumu|Yes|Şirketinizin perspektifinden ilgili durumunu gösterir. Bir başvuruyu oluşturmaya veya değiştirmeye çalışıyorsanız gereklidir. Yeni bir anlaşma oluşturmaya çalışıyorsanız **Yeni** ' ye kullanın. Kullanabileceğiniz değerler [başvuru kaynaklarında](/partner/develop/referral-resources#referralstatus)listelenmiştir.|Etkin
İş ortağı başvurusu alt durumu|Yes|İşlem durumunun tam durumunu gösterir. Yeni bir anlaşma oluşturmaya çalışıyorsanız **kabul edildi** ' i kullanın. Mevcut bir başvuruyu değiştiriyorsanız de gereklidir. Kullanabileceğiniz değerler [başvuru kaynaklarında](/partner/develop/referral-resources#referralsubstatus)listelenmiştir.|Kabul edildi
Microsoft başvuru durumu|Şekline|Microsoft arama yardımı 'na gönderdiğiniz ortak satış isteğinin durumunu gösterir. Bu salt okunurdur. Verilerin içeri aktarılması sırasında bu alanda yapılan herhangi bir değişiklik yok sayılır.| Beklemede
Reddedilen/kayıp nedeni|Şekline| Bu bilgileri yalnızca, alanın alt durumunu reddedilmiş veya kayıp olarak değiştiriyorsanız sağlamanız gerekir. Bu sütunu, aksi takdirde yoksayabilirsiniz. <br/> **Aşağıdaki seçeneklere göre bir sayı girin** <br/><br/> **1**-Project bütçe yeterli değil  <br/> **2**-müşteri yanıt vermedi  <br/> **3**-müşteri başka bir satıcı seçti  <br/> **4** -müşteri gereksinimi karşılanmadı  <br/> **5** -müşteri değil <br/> **6**-önerilen zaman satırı çok kısa <br/> **7** -kötüye kullanma, istenmeyen posta veya kimlik avı olarak raporla <br/> **8** -diğerleri |6|
Satış Aşaması|Hayır|Bu, başvurunun ayrıntılı satış aşamasını belirten alandır. Satış aşamaları hakkında daha fazla bilgi edinmek için [Iş Ortağı Merkezi 'nde ortak satış fırsatlarını yönetin](./manage-co-sell-opportunities.md)|40
Tahmini anlaşma değeri|Yes|Müşteriyle ilk konuşmaları temel alan işlem değeri. Bu, bu durum, işlem, **kazanılan** veya kaybolan Terminal durumlarından birine ulaştığında değiştirilebilir **.**|12563
Para Birimi|Yes|Anlaşma değerinin girildiği para birimi. Para birimi kodlarını [ıso 4217 vican sayfasında](https://en.wikipedia.org/wiki/ISO_4217)bulabilirsiniz.|USD
Tahmini kapanış tarihi|Yes|Müşterinin AA/GG/YYYY biçiminde ilk konuşmaları temel alan tahmini kapanış tarihi. <br/> **Tarih UTC saat diliminde olmalıdır. Iş Ortağı Merkezi Kullanıcı arabiriminde görüntülenen tüm tarihler yerelleştirilmiş Timezones tabanlıdır. UTC saat diliminde tarihi sağladığınız başvuruya bakıyorsanız, Iş Ortağı Merkezi Kullanıcı arabiriminde +/-bir gün farkı olabilir.**|1/30/2020
CRM KIMLIĞI|Hayır|Varsa, CRM sisteminizde bu özel başvurunun tanımlayıcısı. Bu, ücretsiz bir form metin girişi alanıdır.|34234324-sdfsdf-345345-sfd
Pazarlama kampanyası KIMLIĞI|Hayır|Bu alan, bu özel başvurunun sonucu olan pazarlama kampanyasını gösterir. Genellikle ROı hesaplama için kullanılır|BingSummer2020
Notlar|Hayır|Başvuruya ilişkin güncelleştirmeleri gösteren ayrıntılı notlar|Bu örnek bir notdır
Microsoft yardımı gerekli mi?|Yes|Bu, Microsoft 'un bu ortak satış isteğini yaparken size yardımcı olmasını isteyip istemediğinizi belirtir|Yes
Microsoft 'a özgü yardım nedir?|Şekline|Microsoft 'un size yardımcı olabilecek altı farklı yönden biri. Bu yalnızca, "Microsoft Yardım gerekli" sorusu için Evet ' i seçerseniz geçerlidir. " <br/> **Aşağıdaki seçeneklere göre bir sayı girin** <br/><br/> **1**-iş yüküne özgü değer teklifi  <br/> **2**-müşteri teknik mimarisi  <br/> **3**-kavram kanıtı/demo  <br/> **4**-teklifler ve lisanslama  <br/> **5**-satış sonrası müşteri başarısı  <br/> **6**-genel veya diğer|1|
Microsoft Sales Team ile paylaşma|Yes|Bu, Microsoft satış ekibi ile ilgilenmenin ayrıntılarını paylaşmak isteyip istemediğinizi belirtmek için kullanılır. Bu yalnızca, "Microsoft yardımı gerekli" sorusu için Hayır 'ı seçerseniz geçerlidir. "|Yes
Microsoft 'a notlar|Hayır|Microsoft 'a yönelik yardıma ihtiyacınız varsa Microsoft 'a özgü notlar|Contoso müşterisi için POC ile ilgili yardım gerekiyor
Müşteri/Iş ortağı ilgili kişisini paylaşma onayı|Yes|Müşteri iletişim ayrıntılarını ve şirketinizin çalışanlarınızı paylaşma onayı, anlaşma üzerinde çalışan ayrıntıları ile iletişim kurun. **Bu sütun için Hayır ' ı seçerseniz anlaşmalar oluşturulmaz veya güncellenmez.** |Yes
CLA numarası|Şekline|IOT anlaşmayı oluştururken veya güncelleştirirken CLA numarası gerekli değildir. Design WIN aşamasına geçtiğinizde bu gerekli hale gelir.
Cihaz Kategorisi|Hayır|Tüm IoT cihaz kategorilerinin listesi. Aşağıdaki seçeneklerden bir kategori seçin <br>Aron veya tüketici oyun cihazı <br> ATM <br> & taşımacılık sistemlerini oto <br> Azure Sphere panosu<br> Azure Sphere bileşeni <br> Azure Sphere koruyucu<br> Azure Sphere modülü <br> Otomasyon oluşturma<br> Casino oyun cihazı <br> İletişim cihazları<br> Tüketici Internet cihazı <br> Tüketici takılabilir<br> Dijital resim çerçevesi <br> Dijital Imza <br> Ağ geçidi <br> SST/mobil<br> Endüstriyel otomasyon cihazı<br> Endüstri tabletini (POS dışı) <br> Bilgi noktası<br> Media Player<br> Medya cihazı <br> Mobil POS <br> Gezinti cihazı<br> Ağ projektörü<br> Diğer<br> Diğer bankacılık cihazı<br> Diğer tüketici elektronik cihazı<br> Diğer cihaz<br> diğer Enterprise cihaz<br>  Diğer algılayıcı/düğüm <br> Satış noktası cihazı<br> Yazdırma cihazı <br> Güvenlik/araştırma <br>  Sunucu<br> Set-Top kutusu<br> Akıllı TV <br> Test ve ölçüm cihazı<br> İnce Istemci cihaz <br/>
Silicon Type|Hayır|Aşağıdaki listeden bir seçenek belirleyerek yonga kümesi modeli bilgilerini girin <br> AMD-A10 <br> AMD-A4 <br> AMD-A6 <br> AMD-A8 <br> AMD-E2 <br> AMD-FX 7500 <br> AMD-FX 7600P <br> AMD-FX 9370 <br> AMD-FX 9590 <br> AMD-G serisi <br> AMD-diğerleri <br> AMD-R serisi <br> AMD-FX modellerinin geri kalanı <br> Intel-Atom <br> Intel-Celeron-N1900 <br> Intel-Celeron-N2807 <br> Intel-Celeron-N2930 <br> Intel-Celeron-N3060 <br> Intel-Celeron-N3160 <br> Intel-Core i3 <br> Intel-Core i5 <br> Intel-Core i7 <br> Intel-Core d <br> Intel-diğerleri <br> Intel-Pentium <br> Intel-Celeron 'nin geri kalanı <br> Intel-XEON <br> MediaTek MT3620 <br> NXP 8ULP-CS <br> Diğer <br/>
Azure Sertifikalı cihaz|Hayır|Bu, cihaz için Azure uyumluluk sertifikası 'nın elde edildiğini belirtir
Hizmetleri Ekle|Hayır|Bu, Azure hizmetlerinin dağıtımda IoT çözümüyle birlikte paketlenebilir olduğunu belirtir
Microsoft MSX KIMLIĞI|Hayır|Yalnızca ortak satış fırsatları için kullanılabilen Microsoft MSX sisteminde bir işlem KIMLIĞI
Geçirilen PSC anlaşma KIMLIĞI|Hayır|PSC anlaşma KIMLIĞI, yalnızca PSC 'den BILGISAYARA geçirilen bir anlaşma için kullanılabilir
MPN Kimliği|Hayır|MPN ortak satış fırsatlarının oluşturulduğu kuruluşun KIMLIĞI
1\. Çözüm|Yes|Çözüm KIMLIĞI (gerekli), anlaşma değerinin girildiği para birimi (isteğe bağlı). [Para birimi kodlarını](https://en.wikipedia.org/wiki/ISO_4217), SKU 'nun fiyatını (isteğe bağlı) ve SKU 'nun miktarını bulabilirsiniz (isteğe bağlı)  |NUEVO-1234-PQRS, USD, 10, 100
Takım üyesi 1|Yes|İlgili takım üyesinin adı, soyadı, cep telefonu numarası ve e-posta KIMLIĞI.| Bob, Iş ortağı, 999999, Bob.partner@Contoso.com
Microsoft takım üyesi 1|Hayır|Ortak satış fırsatı üzerinde çalışan ilgili Microsoft ekibi üyesinin adı, soyadı, cep telefonu numarası ve e-posta KIMLIĞI.| Sam, satıcı, 999999, Sam.seller@Microsoft.com

## <a name="next-steps"></a>Sonraki adımlar

Bu Iş Ortağı Merkezi ortak satış bağlayıcılarını, CRM sistemlerinizden Microsoft ile birlikte satın almak için kullanabilirsiniz.

- [Dynamics 365 CRM için ortak satış Bağlayıcısı – genel bakış](connector-dynamics.md)
- [Salesforce için ortak satış Bağlayıcısı CRM-genel bakış](connector-salesforce.md)
