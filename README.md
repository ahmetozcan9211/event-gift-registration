# Kongre Stant Hediye Kayıt Sistemi

Tıbbi kongrelerde firma standını ziyaret eden katılımcıların mobil formla kaydolduğu, SMS ile doğrulama kodu aldığı ve standda kodla hediyesini teslim aldığı web uygulaması. İki farklı ulusal kongrede, ayrı kurulumlarla kullanıldı.

> Bu depo bir proje vitrinidir. Kaynak kod paylaşılmamaktadır.

## Akış

```
Stanttaki QR afiş → Mobil kayıt formu + KVKK onayı
       → SMS ile tek kullanımlık kod (NetGSM)
       → Stant görevlisi panelde kodu sorgular → "ürün verildi"
```

## Özellikler

- Mobil uyumlu katılımcı formu ve KVKK aydınlatma metni
- NetGSM entegrasyonu ile SMS gönderimi
- Stant paneli: kod sorgulama, teslim işaretleme, katılımcı listesi, CSV dışa aktarma
- Mükerrer kayıt ve kötüye kullanım koruması
- QR kodlu afişleri otomatik üreten Python betiği
- **Paylaşımlı hostingde çalışır:** cPanel, PHP 7.4+ ve MySQL yeterli, ek kütüphane gerekmez
- Tüm renkler ve ayarlar tek yerden değiştirilir. Aynı sistem başka bir etkinlik için kopyalanıp dakikalar içinde yeniden kurulabilir.

## Teknolojiler

`PHP` · `MySQL` · `NetGSM SMS API` · `HTML/CSS` · `Python (QR afiş)` · `cPanel`
