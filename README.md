# Diskus Üretim Yönetimi

Diskus balığı yetiştiriciliği yapan hobi sahipleri ve işletmeler için tank yönetimi, su kalitesi takibi ve görev planlamasını tek bir panelde toplayan bir web arayüzü.

<!-- Ekran görüntülerini docs/ klasörüne ekleyip yollarını buraya yaz -->
![Yeni Tank Ekle modalı](docs/tank-ekle-modal.png)
![Yeni Görev Ekle modalı](docs/gorev-ekle-modal.png)

🔗 **GitHub:** https://github.com/eminenurclsknl/Diskus-Uretim-Yonetimi-

## Amaç

Diskus balıkları hassas çevresel koşullara ihtiyaç duyan özel bir türdür; bu yüzden tank yönetimi, su kalitesi takibi, yemleme düzeni ve üretim döngüsü gibi işlemlerin düzenli takip edilmesi büyük önem taşır. Bu uygulama tüm bu süreçleri tek bir platformda toplayarak hobi amaçlı yetiştiricilerden profesyonel işletmelere kadar geniş bir kullanıcı kitlesine hitap eder.

## Özellikler

- **Ana panel** — toplam tank sayısı, aktif üreme, boylandırma, su değişimi ve bekleyen görevleri özetleyen bilgi kartları
- **Tank yönetimi** — tank ekleme, türe göre filtreleme (Üreme, Boylandırma, Ana, Boş, Karantina), düzenleme ve detay sayfaları
- **Tank detay sayfaları** — her tank için Genel Bakış, Su Parametreleri (sıcaklık, pH, TDS, ORP), Yemleme, Bakım ve Görevler sekmeleri
- **Görev yönetimi** — görev ekleme, listeleme, filtreleme, tamamlama işaretleme; kurulum durumuna göre (yeni/kurulu tank) otomatik rutin görev önerisi
- **Su Değişimi Gerekli** sayfası — su değişimi bekleyen tankların ayrı listelenmesi
- **Favori Tanklar** — sık kullanılan tanklara hızlı erişim
- Mobil uyumlu (responsive) tasarım

## Kullanılan Teknolojiler

<p>
  <img src="https://img.shields.io/badge/-HTML5-E34F26?logo=html5&logoColor=white" />
  <img src="https://img.shields.io/badge/-CSS3-1572B6?logo=css3&logoColor=white" />
  <img src="https://img.shields.io/badge/-JavaScript-F7DF1E?logo=javascript&logoColor=black" />
</p>

## Nasıl Geliştirildi

Arayüz tamamen HTML, CSS ve JavaScript ile tasarlandı. HTML ile sayfa yapısı (tank ekleme formu, su parametreleri tablosu, görev listesi) semantik etiketlerle oluşturuldu. CSS ile Diskus balığı yetiştiriciliğine uygun bir renk paleti ve responsive düzen (`@media query`) uygulandı. JavaScript ile form doğrulama, tank/görev ekleme, modal açma-kapama ve görev tamamlama işaretleme gibi etkileşimler eklendi.

Veriler şu an yalnızca tarayıcıda geçici olarak tutuluyor; sayfa yenilendiğinde sıfırlanıyor (proje veritabanı entegrasyonu olmadan tamamlandı).

## Kurulum

Projenin herhangi bir backend/derleme adımı yok — statik dosyaları klonlayıp doğrudan tarayıcıda açman yeterli.

```bash
git clone https://github.com/eminenurclsknl/Diskus-Uretim-Yonetimi-.git
cd Diskus-Uretim-Yonetimi-
# index.html dosyasını tarayıcında aç
```

## Proje Yapısı

```
Diskus-Uretim-Yonetimi-/
├── index.html          # Ana panel
├── tanklar/             # Tank listesi ve tür bazlı sayfalar
├── gorevler/            # Görev listeleme ve ekleme
├── css/
├── js/
└── README.md
```

## Yol Haritası

- [ ] Verileri kalıcı hale getirmek için veritabanı entegrasyonu (localStorage veya backend API)
- [ ] Kullanıcı girişi / çoklu kullanıcı desteği
- [ ] Su parametreleri için grafik/geçmiş takibi

