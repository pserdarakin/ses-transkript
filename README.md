# Ses Transkript

Ses dosyalarını Groq Whisper (`whisper-large-v3`) ile metne dönüştüren tek sayfalık araç.

Canlı: https://ses-transkript.vercel.app

- Sunucu yok: tarayıcı ses dosyasını doğrudan Groq API'sine gönderir.
- Her kullanıcı kendi Groq API anahtarını girer ([console.groq.com/keys](https://console.groq.com/keys)); anahtar sadece o tarayıcının `localStorage`'ında saklanır.
- Birden fazla dosya, dil seçimi (Türkçe / English / otomatik), kopyalama ve `.txt` indirme.
- Dosya başına en fazla 25 MB.

## Yerel çalıştırma

```bash
python3 -m http.server 8765
```

Sonra http://localhost:8765 adresini açın.

## Yayınlama

```bash
npx vercel@latest deploy --prod --yes --project ses-transkript
```
