# Meclis Takip Araçları

Bu çalışma [tbmm.gov.tr](https://www.tbmm.gov.tr/) adresinde yayınlanan bilgilerin veri olarak toplanması, yapılandırılması ve aktif sivil kullanıma açılmasını amaçlar.

Şu anda TBMM websitesinde HTML sayfa formatında bilgiler yayınlanmaktadır, dolayısıyla insanların okuması dışında bilgisayar programları tarafından kolayca okuma ve başka sistemler içinde kullanımı mümkün değildir. Halbuki yayınlananlar veri olarak yapılandırılıp bir programatik kullanım arayüzü (API) oluşturulduğunda, meclis hakkında ve meclis işleyişi üzerine sistematik çalışan pek çok yeni sivil araç geliştirilebilir.

Bu sorunu çözebilmek için tbmm.gov.tr adresinde yayınlanan bilgileri HTML sayfalardan ayıklayan, yapısal veriye çeviren, ve herkesin erişimine açık hale getiren araçlar seti geliştirmekteyiz.

Şu anda bulunduğunuz bu github repo alanında organize olmaktayız, forum şeklinde işleyen [issue](https://github.com/meclistakip/tbmm-graph/issues)'larda tartışmalar yapmakta ve [wiki](https://github.com/meclistakip/tbmm-graph/wiki)'de varılan sonuçları düzenlemekteyiz. Geliştirilmekte olan araçlar ise bu organizasyon altında kendi repolarında bulunmaktadırlar.

## Çalışmaya kimler destek olabilir ve faydalanabilir

Çalışma herkesin katılımına açıktır, görüş bildirerek ve programlama becerilerinizle pek çok şekilde desteğiniz olabilir.

Gazeteciyseniz ya da sivil toplum alanında araştırma yapıyorsanız, haber yapmaktan raporlamaya bu çalışmadan faydalanabileceğiniz pek çok nokta var. Yapılanları inceledikten sonra lütfen kullanıma dair özel istekleriniz olursa [issue]()'larda yazın.

Tasarım, sanat, ya da bilgisayar bilimleri alanında çalışıyorsanız, bu araçlarla toplanan verileri infografik yapmaktan, yeni sanat eseri üretmeye, doğal dil işlemekten yapay zeka çalışmalarına pek çok alanda kullanabilirsiniz.

TBMM işleyişlerinde uzman, [TBMM Kütüphane ve Arşiv Hizmetleri Başkanlığı](https://www.tbmm.gov.tr/kutuphane/)'nda bir çalışan, ya da herhangi bir dönem milletvekili iseniz, veri yapılandırma ve derleme işinde desteğinizin çalışmaya çok katkısı olacaktır, bir email ile konuşabiliriz.

## Çalışmanın işleyişi

- Ne tür veriler toplanabiliyor?

- Veri modelinin türleri, özellikleri, ve ilişkileri nelerdir?

- Meclis işleyişi zamana göre sinyal log olarak kaydedilecek.

- Farklı dillerle geliştirilen araçların ortak dili sinyal yapısı olacak.

- Büyük pdf doc vb dosyalar AWS S3'e yerleştirilerek linki veri olarak tutulacak.

## Veri yapısı

Aktörler ve ilişkiler şeklinde düzenlenecek veri yapısı için mecliste şu kategoriler bulunuyor:

#### YAPI

- Milletvekili
- Siyasi Parti
- İl    
- Dönem

#### YASAMA

- Kanun Teklifi
- Kanun
- Karar
- Kanun Hükmünde Kararname
- İhtisas Komisyonu
- Komisyon Raporu

#### DENETİM    

- Soru Önergesi
- Meclis Soruşturma Önergesi
- Meclis Araştırma Önergesi
- Gensoru Önergesi
- Soruşturma Komisyonu
- Araştırma Komisyonu    

#### KONUŞMALAR / GÖRÜŞMELER

https://www.tbmm.gov.tr/develop/owa/takvim.ekran

#### AKTIVITELER

Bir milletvekilinin meclisteki aktiviteleri.

- İlk İmza Sahibi Olduğu Kanun Teklifleri
- İmzası Bulunan Kanun Teklifleri

- Sahibi Olduğu Sözlü Soru Önergeleri 
- Sahibi Olduğu Yazılı Soru Önergeleri

- İlk İmza Sahibi Olduğu Genel Görüşme Önergeleri
- İmzası Bulunan Genel Görüşme Önergeleri

- İlk İmza Sahibi Olduğu Meclis Soruşturma Önergeleri
- İmzası Bulunan Meclis Soruşturma Önergeleri

- İlk İmza Sahibi Olduğu Meclis Araştırma Önergeleri
- İmzası Bulunan Meclis Araştırma Önergeleri

- İlk İmza Sahibi Olduğu Gensoru Önergeleri
- İmzası Bulunan Gensoru Önergeleri

- Genel Kurul Konuşmaları
- Komisyon Konuşmaları


---

####NOTLAR 

https://www.tbmm.gov.tr/kutuphane/ adresinde yer alan istatistiğe göre Ziyaretçi Sayısı 19/12/2008 den itibaren
Kurum Dışı 437057 ve Kurum İçi 331700 adetmiş, buna göre TBMM kütüphane/arşiv websitesi %43 kurum içinde %57 kurum dışında kullanılmakta.
