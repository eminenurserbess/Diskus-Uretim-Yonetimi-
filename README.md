# Diskus Üretim Yönetimi

Diskus balığı yetiştiriciliği yapan hobi sahipleri ve işletmeler için tank yönetimi, su kalitesi takibi ve görev planlamasını tek bir panelde toplayan bir web arayüzü.

🔗 **GitHub:** https://github.com/eminenurserbess/Diskus-Uretim-Yonetimi-

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

Uygulamanın arayüzü HTML5, CSS3 ve JavaScript kullanılarak geliştirildi. Responsive tasarım için CSS media query yapısı kullanıldı. JavaScript ile form doğrulama, tank ve görev yönetimi, modal işlemleri ve görev durumlarının güncellenmesi sağlandı.

Veriler mevcut sürümde tarayıcı belleğinde geçici olarak tutulmaktadır. Projede henüz veritabanı veya backend entegrasyonu bulunmamaktadır.

## Proje Yapısı

```
Diskus-Uretim-Yonetimi-/
└── tank/
    ├── index.html                    # Ana panel
    ├── login.html                    # Giriş sayfası
    ├── gorevler.html                 # Görev listeleme ve ekleme
    ├── bekleyen-gorevler.html        # Bekleyen görevler
    ├── su-degisimi.html              # Su değişimi gereken tanklar
    ├── toplam-tank.html              # Tüm tanklar listesi
    ├── ana-tank.html / ana-tank-detay.html
    ├── ureme-tank.html / ureme-tank-detay.html
    ├── boylandirma-tank.html / boylandirma-tank-detay.html
    ├── karantina-tank.html / karantina-tank-detay.html
    ├── bos-tank.html / bos-tank-detay.html
    ├── css/                          # Stil dosyaları
    └── image/                        # Görseller
```

## Yol Haritası

- [ ] Verilerin kalıcı olarak saklanması için backend API ve veritabanı entegrasyonu
- [ ] Kullanıcı girişi ve çoklu kullanıcı desteği
- [ ] Su parametreleri için grafik ve geçmiş takibi
- [ ] Tank bakım ve yemleme geçmişinin raporlanması
