# NLP Soru Bankası

Doğal Dil İşleme (Raymond Lee — *NLP: A Textbook with Python Implementation*) dersi final soru havuzu.
589 soru, 10 bölüm. Her sorunun cevabında **Gemini 3.5 Flash** ve **Opus 4.8** versiyonları yan yana gösterilir.
Opus cevapları kitap temel alınarak verilmiştir; Gemini anahtarının hatalı olduğu sorular ⚠️ rozetiyle işaretlidir.

## Özellikler
- Bölüm + soru tipi (Doğru/Yanlış, Boşluk, Çoktan Seçmeli, Kısa Cevap) filtreleri
- Metin içinde arama
- ⭐ Yıldızlı (önemli) sorular kategorisi
- ⚠️ Gemini ≠ Opus çelişkileri kategorisi (Gemini anahtarının yanlış olduğu sorular)
- Açık / koyu tema

## Vercel'e Yükleme

### Yöntem 1 — Sürükle-bırak (en kolay)
1. https://vercel.com adresine giriş yap.
2. **Add New → Project → Deploy** kısmında bu klasörü (`nlp-soru-bankasi`) sürükle-bırak,
   ya da içindeki `index.html` dosyasını yükle.
3. Build ayarı sorulursa: framework **Other**, build komutu **boş**, output dizini **boş** bırak.

### Yöntem 2 — Vercel CLI
```bash
npm i -g vercel
cd nlp-soru-bankasi
vercel        # önizleme
vercel --prod # yayına alma
```

Tek dosyalık statik site olduğu için ek bir derleme adımı gerekmez.
