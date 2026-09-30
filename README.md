# Kampüs Etkinlikleri

Üniversite etkinliklerini görüntülemek ve yönetmek için hazırlanmış HTML/CSS tabanlı web uygulaması.

## Sprint 2 — CSS ve Responsive Tasarım

Sprint 1 yapısı korunarak `sprint2/` klasörü oluşturuldu ve beş sayfanın tamamına ortak `css/numaran.css` dosyası bağlandı.

### Sprint 2'de yapılanlar

- Beş sayfada ortak başlık, menü ve footer
- Öğrenci numarasından türetilen CSS renk tonu (`--no: 2221031010`, ton: 210)
- Öğrenci numarasının son hanesine göre Arial font
- Etkinlik tablosu yerine `section > article` kart yapısı
- Telefonda tek sütun, geniş ekranda çok sütunlu responsive kartlar
- Detay sayfasında mobilde alt alta, geniş ekranda afiş + künye yan yana
- Form etiketleri alanların üstünde
- Boş/uygunsuz zorunlu alanlarda kırmızı hata görünümü (`:user-invalid`)
- Dokunmatik kullanım için en az 44 px etkileşim alanları
- Telefonda yatay taşmayı engelleyen responsive yapı
- JavaScript kullanılmadı

## Dosya Yapısı

```text
kampusEtkinlik/
├── sprint2/
│   ├── css/
│   │   └── numaran.css
│   ├── afis.jpg
│   ├── afis.jpeg
│   ├── index.html
│   ├── etkinlikler.html
│   ├── etkinlik-detay.html
│   ├── etkinlik-ekle.html
│   └── etkinlik-guncelle.html
├── .gitignore
└── README.md
```

## GitHub'a Gönderme

```bash
git add .
git commit -m "Sprint2 yapıldı"
git tag sprint-02
git push
git push --tags
```

## Vercel

Vercel projesinde **Settings → Root Directory** alanını `sprint1` yerine `sprint2` yapın ve yeniden deploy edin. Framework ayarı **Other**, build komutu yoktur.

## Kontrol Listesi

- `css/numaran.css` beş sayfaya bağlıdır.
- Kartlar telefonda tek sütundur.
- Geniş ekranda tüm etkinlikler üç sütundur.
- Menü mobilde taşmadan alt satıra geçebilir.
- Detay sayfası mobilde alt alta, geniş ekranda iki sütundur.
- Güncelleme formu ekleme formunun dolu halidir.
- Boş form gönderildiğinde tarayıcı doğrulaması ve kırmızı alan görünümü çalışır.
