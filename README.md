# BİK Uyumlu Haber Sitesi Rehberi

> Türkiye'de bir internet haber sitesinin Basın İlan Kurumu (BİK) mevzuatına ve
> ilgili yasal düzenlemelere uyumlu çalışması için pratik bir başvuru rehberi.
> Bu depo **eğitici içeriktir**, kod içermez. Hukuki tavsiye değildir; güncel
> mevzuat için resmi kaynaklara başvurun.

İçindekiler:

1. [Neden BİK Uyumu?](#1-neden-bik-uyumu)
2. [Temel Kavramlar ve Kurumlar](#2-temel-kavramlar-ve-kurumlar)
3. [İnternet Haber Sitesi Olmanın Yasal Koşulları](#3-internet-haber-sitesi-olmanin-yasal-kosullari)
4. [Zorunlu "Künye" (İletişim/Bilgilendirme) Yapısı](#4-zorunlu-künye-yapisi)
5. [Mahreç (Kaynak Gösterme) Yönetimi](#5-mahreç-kaynak-gösterme-yönetimi)
6. [Resmi İlan ve Reklam Yayını Şartları](#6-resmi-ilan-ve-reklam-yayini-şartlari)
7. [İçerik Arşivi ve Erişilebilirlik](#7-içerik-arşivi-ve-erişilebilirlik)
8. [Düzeltme, Cevap ve İçerik Kaldırma](#8-düzeltme-cevap-ve-içerik-kaldirma)
9. [KVKK ve Kişisel Veri](#9-kvkk-ve-kişisel-veri)
10. [İYS ve Ticari Elektronik İleti](#10-iys-ve-ticari-elektronik-ileti)
11. [Google News ve Teknik Uyum](#11-google-news-ve-teknik-uyum)
12. [Uygulama Kontrol Listesi](#12-uygulama-kontrol-listesi)
13. [Resmi Kaynaklar](#13-resmi-kaynaklar)

---

## 1. Neden BİK Uyumu?

Türkiye'de resmi ilan ve reklam yayınlama hakkı, Basın İlan Kurumu (BİK)
tarafından belirlenen şartları karşılayan yayın organlarına tanınır. Bir
internet haber sitesinin resmi ilan alabilmesi, sürekliliği ve kamu nezdindeki
güvenilirliği için bu uyum önemlidir. Uyum aynı zamanda yayıncıyı 5187 sayılı
Basın Kanunu ve 7418 sayılı Kanun ile getirilen internet haberciliği
düzenlemeleri karşısında hukuki riskten korur.

Bu rehber, teknik ekiplerin ve editörlerin bir haber sitesini kurarken ya da
mevcut siteyi güncellerken gözden geçirmesi gereken uyum başlıklarını derler.

## 2. Temel Kavramlar ve Kurumlar

| Kısaltma | Açılım | İlgi Alanı |
|---|---|---|
| **BİK** | Basın İlan Kurumu | Resmi ilan/reklam dağıtımı, yayın şartları |
| **RTÜK** | Radyo ve Televizyon Üst Kurulu | Radyo/TV ve isteğe bağlı yayın hizmetleri |
| **KVKK** | Kişisel Verileri Koruma Kurumu | Kişisel veri işleme |
| **KVK Kanunu** | 6698 sayılı Kişisel Verilerin Korunması Kanunu | Veri koruma çerçevesi |
| **İYS** | İleti Yönetim Sistemi | Ticari elektronik ileti izinleri |
| **Basın Kanunu** | 5187 sayılı Kanun (7418 ile güncellendi) | Süreli yayın, künye, mahreç, cevap-düzeltme |

**Not:** Mevzuat değişebilir. Yükümlülüklerin güncel hâli için Bölüm 13'teki
resmi kaynakları esas alın.

## 3. İnternet Haber Sitesi Olmanın Yasal Koşulları

7418 sayılı Kanun ile internet haber siteleri süreli yayın kapsamına alınmıştır.
Uyum için genel başlıklar:

- **Sorumlu müdür** ataması ve yetkilerinin belirlenmesi.
- **Yayın sahibi** bilgilerinin açık ve doğru olması.
- Yayının yapıldığı **iş yeri adresi** ve **elektronik iletişim** bilgilerinin
  bulunması.
- Beyan ve bildirim yükümlülüklerinin ilgili Cumhuriyet başsavcılığına
  yapılması.
- İçeriklerin **belirli bir süre arşivlenmesi** (bkz. Bölüm 7).

Teknik açıdan bu koşullar; sitede sabit bir künye sayfası, doğru iletişim
bilgileri ve arşiv/erişim altyapısı gerektirir.

## 4. Zorunlu "Künye" Yapısı

Künye, yayının kim tarafından ve nasıl yapıldığını gösteren şeffaflık
bloğudur. Genellikle ayrı bir **"Künye" / "İletişim"** sayfasında ve/veya site
alt bilgisinde (footer) yer alır.

Künyede tipik olarak bulunması beklenenler:

- Yayının **adı** ve **sahibi** (gerçek/tüzel kişi),
- **Sorumlu müdür** adı,
- **Adres** (iş yeri),
- **Telefon** ve **e-posta**,
- Varsa **ticaret sicil / mersis** bilgisi,
- Yayın ilkeleri / etik ilkeler bağlantısı.

**Teknik ipucu:** Künye sayfasını statik ve kalıcı bir URL'de tutun
(`/kunye` gibi), footer'dan her sayfadan erişilebilir yapın ve sayfayı
`sitemap.xml`'e ekleyin. Böylece hem kullanıcılar hem de denetim kolayca
ulaşır.

## 5. Mahreç (Kaynak Gösterme) Yönetimi

**Mahreç**, bir haberin kaynağını (örneğin bir haber ajansını veya ilk yayınlayan
yayın organını) belirtme yükümlülüğüdür. Ajans içeriği kullanan siteler için
kritik bir uyum ve etik başlığıdır.

İyi bir mahreç yönetimi:

- Her haberde kaynağın **görünür şekilde** belirtilmesi (örn. haber girişinde
  veya sonunda "Kaynak: …").
- Ajans aboneliği kapsamında alınan içeriklerde **ajansın adının** kurallara
  uygun gösterilmesi.
- Kaynağı belirsiz içeriklerin yayınlanmaması.
- Alıntı ve derleme haberlerde **özgün kaynağa bağlantı** verilmesi.

**Teknik ipucu:** İçerik yönetiminde her habere yapısal bir "kaynak/mahreç"
alanı ekleyin (serbest metin yerine seçilebilir kaynak + opsiyonel URL). Bu
hem tutarlılık sağlar hem de otomatik künye/rozet basımını mümkün kılar. Aynı
alan `NewsArticle` yapısal verisinde de değerlendirilebilir.

## 6. Resmi İlan ve Reklam Yayını Şartları

Resmi ilan yayınlama hakkı; BİK'in belirlediği süreklilik, içerik üretimi,
personel ve teknik ölçütleri karşılayan yayın organlarına tanınır. Genel
beklentiler (özet):

- **Düzenli ve özgün içerik üretimi** (yalnızca kopya/derleme değil).
- Yayının **kesintisiz sürekliliği**.
- Asgari **kadro / muhabir** ve editoryal yapı.
- Resmi ilanların, alındıkları hâliyle ve **belirtilen sürede** yayımlanması.
- İlan ve reklamın haber içeriğinden **ayırt edilebilir** olması.

**Teknik ipucu:** Resmi ilanlar için ayrı bir bölüm/etiket ve kalıcı arşiv URL'i
oluşturun; ilan yayın tarih-saatini ve yayın süresini kayıt altına alın. Reklam
alanlarını içerikten görsel olarak ayrıştırın ve "reklam/ilan" etiketi kullanın.

## 7. İçerik Arşivi ve Erişilebilirlik

İnternet haber siteleri için içeriklerin **belirli bir süre boyunca**
değiştirilmeden saklanması ve talep hâlinde erişilebilir olması beklenir.

Uygulama önerileri:

- Yayınlanan her içeriğin **tarih-saat damgası** ile saklanması.
- İçerik güncellenirse **güncelleme kaydının** tutulması (kim, ne zaman, ne
  değişti).
- Silinen/düzeltilen içerik için **iz kaydı** bırakılması.
- Arşivin yedeklenmesi ve makul sürede geri getirilebilir olması.

**Teknik ipucu:** İçerik tablosunda `created_at`, `updated_at` ve bir **revizyon
geçmişi** tutun. Böylece bir içeriğin belirli tarihteki hâli gösterilebilir; bu
hem yasal arşiv hem de editoryal şeffaflık için değerlidir.

## 8. Düzeltme, Cevap ve İçerik Kaldırma

Basın mevzuatı, kişilerin **cevap ve düzeltme** hakkını düzenler. Bir haberden
etkilenen kişi, usulüne uygun başvurduğunda cevap/düzeltme metninin yayımlanması
gerekebilir.

Süreç için öneriler:

- Sitede **erişilebilir bir iletişim/başvuru kanalı** bulundurun.
- Gelen cevap/düzeltme taleplerini **kayıt altına alın** (tarih, talep, karar).
- Yayımlanan düzeltmeyi ilgili haberle **ilişkilendirin** (haberin altında not
  veya bağlantı).
- İçerik kaldırma/erişim engeli kararlarında **iz kaydı** tutun.

**Teknik ipucu:** Düzeltme/cevap metinlerini ayrı bir içerik tipi olarak
modelleyin ve ilgili orijinal haberle bağlayın. Otomatik "Bu haberde düzeltme
yayımlanmıştır" rozeti şeffaflığı artırır.

## 9. KVKK ve Kişisel Veri

Haber sitesi; ziyaretçi, üye, yorum yapan kullanıcı ve muhabir verileri işler.
6698 sayılı KVK Kanunu kapsamında dikkat edilecekler:

- **Aydınlatma metni** (privacy notice) yayımlanması.
- Gerektiğinde **açık rıza** alınması (örn. bülten aboneliği, bazı çerezler).
- **Çerez yönetimi**: zorunlu olmayan çerezler için onay bariyeri.
- Kullanıcıya **veri silme / düzeltme** talebi imkânı.
- **VERBİS** kayıt yükümlülüğünün değerlendirilmesi.
- Veri ihlali durumunda **bildirim** yükümlülüğü.

**Teknik ipucu:** Onay kayıtlarını (kim, ne zaman, hangi metin sürümü) saklayın;
çerez onayını sunucu tarafında da doğrulayın. Ayrıntılı bir geliştirici rehberi
için: `alestaweb/kvkk-icin-web-gelistirici-rehberi`.

## 10. İYS ve Ticari Elektronik İleti

Haber sitesi bülten/SMS gönderiyorsa, ticari elektronik iletiler için **İleti
Yönetim Sistemi (İYS)** yükümlülükleri devreye girer.

- Ticari ileti için **önceden onay** (opt-in) alınması.
- Onayların **İYS'ye kaydedilmesi**.
- Her iletide **kolay ret (opt-out)** imkânı.
- Ret taleplerinin gecikmeden işlenmesi.

**Teknik ipucu:** Bülten aboneliğinde çift onay (double opt-in) kullanın; abone
listesini İYS durumu ile senkron tutun ve her gönderimden önce ret listesini
kontrol edin.

## 11. Google News ve Teknik Uyum

Yasal uyum ile teknik görünürlük birbirini besler. Google News ve arama
motorları için öne çıkan başlıklar:

- **Schema.org `NewsArticle`** yapısal verisi (yayıncı, yazar, tarih).
- **`NewsMediaOrganization`** yayıncı işaretlemesi (künye ile tutarlı).
- **`sitemap-news.xml`** (son ~48 saatlik içerik penceresi).
- **Kanonik URL** ve tekrar eden içeriğin yönetimi.
- Doğru **`datePublished` / `dateModified`** (saat dilimi dahil).
- **IndexNow** ile Bing/Yandex'e hızlı bildirim.

**Not:** Yapısal verideki yayıncı/iletişim bilgileri, sitedeki künye ile
**tutarlı** olmalıdır. Tutarsızlık hem güven hem de zengin sonuç uygunluğu
açısından risklidir.

## 12. Uygulama Kontrol Listesi

Bir haber sitesini yayına almadan önce gözden geçirin:

- [ ] Kalıcı **künye/iletişim** sayfası var ve footer'dan erişilebilir.
- [ ] Sorumlu müdür ve yayın sahibi bilgileri doğru.
- [ ] Her haberde **mahreç/kaynak** alanı dolduruluyor.
- [ ] Resmi ilan/reklam içerikten **ayırt edilebilir** ve etiketli.
- [ ] İçerikler **tarih-saat damgası** ve **revizyon geçmişi** ile saklanıyor.
- [ ] **Düzeltme/cevap** başvuru kanalı ve kayıt süreci mevcut.
- [ ] **Aydınlatma metni** + **çerez onayı** yayımlandı, onaylar saklanıyor.
- [ ] Bülten/SMS için **İYS** ve **opt-out** akışı hazır.
- [ ] `NewsArticle` + `NewsMediaOrganization` + `sitemap-news.xml` uygulandı.
- [ ] Yapısal veri, künyedeki bilgilerle **tutarlı**.
- [ ] Arşiv **yedekleniyor** ve geri getirilebiliyor.

## 13. Resmi Kaynaklar

Yükümlülüklerin güncel ve bağlayıcı hâli için:

- **Basın İlan Kurumu (BİK)** — https://www.bik.gov.tr
- **Kişisel Verileri Koruma Kurumu (KVKK)** — https://www.kvkk.gov.tr
- **İleti Yönetim Sistemi (İYS)** — https://iys.org.tr
- **RTÜK** — https://www.rtuk.gov.tr
- **Resmî Gazete** (mevzuat metinleri) — https://www.resmigazete.gov.tr
- **Mevzuat Bilgi Sistemi** — https://www.mevzuat.gov.tr

---

## Katkı

Rehberde eksik gördüğünüz veya güncellenmesi gereken bir başlık varsa issue
açabilirsiniz. Bu depo yalnızca **eğitici/rehber** niteliğindedir; hukuki
görüş için ilgili meslek mensuplarına ve resmi kaynaklara başvurun.

## Lisans

MIT — serbestçe kullanabilir, kopyalayabilir ve uyarlayabilirsiniz.
