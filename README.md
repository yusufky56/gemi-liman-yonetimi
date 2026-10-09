# Gemi ve Liman Yönetim Sistemi

Gemileri, seferleri, limanları, kaptanları ve mürettebatı SQLite veritabanında tutan, PyQt5 arayüzlü masaüstü uygulaması. Ders ödevi olarak hazırlandı.

## Özellikler

- Tabloları açılır listeden seçip içeriğini görüntüleme
- Arayüzden satır ekleme, silme ve güncelleme
- Kalıtımla modellenmiş gemi türleri: yolcu, petrol tankeri, konteyner gemisi
- Yabancı anahtarlarla bağlı tablolar

## Veritabanı tabloları

| Tablo | İçerik |
|---|---|
| `SHIPS` | Seri no, ad, ağırlık, yapım yılı, tür |
| `CRUISE_SHIP` / `OIL_SHIP` / `CONTAINER_SHIP` | Gemi türüne özel kapasite bilgileri |
| `VOYAGES` | Sefer tarihleri, kalkış limanı, gemi |
| `HARBORS` | Liman, ülke, nüfus, pasaport ve ücret bilgisi |
| `VISITED_HARBOURS` | Seferlerde uğranan limanlar |
| `CAPTAINS` / `CREW_MEMBERS` | Kaptan ve mürettebat bilgileri |

## Çalıştırma

```bash
pip install -r requirements.txt
python main.py
```

Uygulama ilk çalıştığında `Odev2.db` dosyasını ve tabloları kendisi oluşturur.

## Ekip

- Talha Tuna
- Muhammed Yusuf Kaya

Proje raporu: [`docs/proje-raporu.pdf`](docs/proje-raporu.pdf)

## License

[MIT](LICENSE)
