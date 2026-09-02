# To'y taklifnomasi — qo'llanma

## 1. Nimalarni to'ldirish kerak

`index.html` faylini istalgan matn muharriri (masalan, VS Code yoki hatto GitHub'ning o'zidagi "Edit" tugmasi) bilan oching va quyidagi joylardagi `[...]` ichidagi matnlarni o'zingizniki bilan almashtiring:

- `[KUYOV ISMI]`, `[KELIN ISMI]` — ismlar (bir necha joyda takrorlanadi)
- `[KUN]`, `[OY]`, `[YIL]`, `[SANA]`, `[KUN HAFTA]` — sana ma'lumotlari
- `[TO'YXONA NOMI]`, `[VILOYAT]`, `[TUMAN]`, `[KO'CHA MANZILI]` — manzil
- `[VAQT]` — boshlanish vaqti
- Rus tilidagi bloklardagi mos `[...]` joylarni ham to'ldiring (har bir UZ matn ostida RU varianti bor)

## 2. Sana va countdown

`index.html` faylining pastida, `<script>` ichida:

```js
const weddingDate = new Date('2026-12-31T18:00:00');
```

Bu qatordagi sana va vaqtni haqiqiy to'y kuningizga o'zgartiring (format: YIL-OY-KUNTVAQT).

## 3. Xarita manzili

`Xaritada ko'rish` tugmasidagi havolani (`href="https://maps.google.com/?q=41.311081,69.240562"`) to'yxonangizning haqiqiy koordinatalari bilan almashtiring. Google Maps'da manzilni oching, "Share" > "Copy link" orqali olishingiz mumkin.

## 4. Musiqa qo'shish

`assets` papkasiga o'zingiz xohlagan musiqa faylini `music.mp3` nomi bilan joylang (fayl nomi shu bo'lishi shart, yoki `index.html` ichidagi `<source src="assets/music.mp3">` qatorini o'zgartiring). Mualliflik huquqi himoyalangan qo'shiqlar o'rniga tinch instrumental yoki ruxsat etilgan musiqadan foydalanishni tavsiya qilamiz.

## 5. GitHub Pages orqali joylashtirish

1. GitHub'da yangi repository yarating (masalan, `wedding-invitation`)
2. Ushbu papkadagi barcha fayllarni (`index.html`, `assets/` papkasi) repository'ga yuklang
3. Repository sozlamalarida: **Settings → Pages → Source** bo'limidan `main` branch'ni tanlang va saqlang
4. Bir necha daqiqadan so'ng saytingiz shu manzilda ishga tushadi:
   `https://SIZNING-USERNAME.github.io/wedding-invitation/`
5. Shu havolani mehmonlaringizga WhatsApp yoki Telegram orqali yuborishingiz mumkin

## 6. Ixtiyoriy o'zgartirishlar

- Ranglar `index.html` faylining boshidagi `:root { ... }` qismida (`--gold`, `--rose`, `--paper` va h.k.) — o'zingizga yoqqan ranglarga almashtirishingiz mumkin
- Agar kerak bo'lsa, menga qayta murojaat qilib qo'shimcha bo'lim (masalan, mehmonlar ro'yxati, sovg'a hisob raqami, RSVP formasi) qo'shishimni so'rashingiz mumkin
