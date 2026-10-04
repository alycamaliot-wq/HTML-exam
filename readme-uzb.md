# Ko'p sahifali shaxsiy veb-sayt: HTML imtihoni / topshirig'i

**sof HTML** o'rgatish uchun amaliy topshiriq: semantik tuzilma, navigatsiya, formalar va havolalar. O'quvchilar **hech qanday CSS ishlatmasdan** kichik ko'p sahifali shaxsiy veb-sayt yaratadilar. Tayyor saytni keyinchalik **CSS imtihoni** uchun boshlang'ich loyiha sifatida ishlatish mumkin.

---

## 1. Umumiy ma'lumot

| | |
|---|---|
| **Fan** | HTML asoslari |
| **Daraja** | Boshlang'ich |
| **Davomiyligi** | 60-90 daqiqa (imtihon) yoki 1-2 dars (topshiriq) |
| **Vositalar** | Istalgan kod muharriri + brauzer |
| **Ruxsat etilgan** | Faqat HTML. CSS, JavaScript va freymvorklar yo'q |
| **Umumiy ball** | 100 ball |
| **O'tish bali** | 60 ball |

---

## 2. Topshiriq nimalarni qamrab oladi

Topshiriqni bajarish orqali o'quvchilar quyidagilarni ko'rsatadilar:

- Umumiy `<div>` teglari o'rniga **semantik HTML elementlaridan** foydalanish
- To'g'ri **sarlavhalar ierarxiyasi** bilan kontentni tuzish (`h1` dan `h3` gacha)
- Sahifalar orasida ham, sahifa ichida ham (anchor havolalar) **navigatsiya** qurish
- Noyob **`id` atributlari** bilan bo'limlarni ajratish
- To'g'ri label va input turlari bilan foydalanuvchi ma'lumotlarini oladigan **forma** yaratish
- **Tashqi havolalar** (ijtimoiy tarmoqlar) va aloqa havolalari (`mailto:`, `tel:`) qo'shish
- Loyihani **bir nechta o'zaro bog'langan fayllarga** ajratish

---

## 3. Topshiriq tavsifi (o'quvchilarga bering)

**4 ta HTML sahifadan** iborat shaxsiy veb-sayt yarating:

| Sahifa | Fayl | Mazmuni |
|---|---|---|
| 1 | `index.html` | O'zingiz haqingizda (1-qism): tanishtiruv, ta'lim, qiziqishlar |
| 2 | `about2.html` | O'zingiz haqingizda (2-qism): kelib chiqish, tajriba, maqsadlar |
| 3 | `skills.html` | Nima qila olasiz: ko'nikmalar, xizmatlar, loyihalar |
| 4 | `contact.html` | Aloqa formasi + ijtimoiy tarmoq havolalari |

Har bir sahifada bir xil navigatsiya va footer bo'lishi kerak, hamda har bir sahifadan boshqa barcha sahifalarga o'tish mumkin bo'lishi shart.

**Cheklovlar:** CSS ishlatmang (`<style>` yo'q, `style=""` yo'q, `.css` fayl yo'q) va JavaScript ishlatmang.

---

## 4. 20 ta talab (baholash mezoni)

Har bir talab **5 ball**. Jami: **100**. O'tish: **60 va undan yuqori** (12 ta talab).

### A. Tuzilma va semantika (25 ball)

| # | Talab | Ball |
|---|---|---|
| 1 | Har bir sahifada to'g'ri skelet bor: `<!DOCTYPE html>`, `<html lang>`, `<head>`, `<meta charset>`, `<title>`, `<body>` | 5 |
| 2 | Har bir sahifada **noyob va mazmunli `<title>`** bor | 5 |
| 3 | Har bir sahifada semantik elementlar ishlatilgan: `<header>`, `<nav>`, `<main>`, `<footer>` | 5 |
| 4 | Kontent kerakli joyda `<section>` va `<article>` bilan guruhlangan (hamma joyda `<div>` emas) | 5 |
| 5 | Har bir sahifada aniq **bitta `<h1>`** bor | 5 |

### B. Sarlavhalar va kontent (20 ball)

| # | Talab | Ball |
|---|---|---|
| 6 | Sarlavhalar to'g'ri ierarxiyada (`h1` > `h2` > `h3`), darajalar tashlab ketilmagan | 5 |
| 7 | 1 va 2-sahifalarda o'quvchi haqida haqiqiy ma'lumot bor (ism, ta'lim, kelib chiqish, maqsadlar) | 5 |
| 8 | 3-sahifada o'quvchi nima qila olishi tasvirlangan (ko'nikmalar, xizmatlar yoki loyihalar) | 5 |
| 9 | Kamida **bitta ro'yxat** (`<ul>` yoki `<ol>`) va `<thead>` / `<tbody>` bilan **bitta jadval** ishlatilgan | 5 |

### C. Navigatsiya va ID lar (25 ball)

| # | Talab | Ball |
|---|---|---|
| 10 | Har bir sahifada **asosiy navigatsiya** (havolalar ro'yxati bilan `<nav>`) bor | 5 |
| 11 | Asosiy navigatsiya havolalari barcha 4 sahifa orasida ishlaydi (buzilgan havola yo'q) | 5 |
| 12 | Har bir `<section>` mazmunini ifodalovchi **noyob `id`** ga ega | 5 |
| 13 | Kamida **bitta sahifa ichidagi navigatsiya** anchor havolalar (`href="#id"`) bilan shu id larga o'tadi | 5 |
| 14 | Sahifadan sahifaga o'tish uchun **Keyingi / Oldingi** havolalar va "Tepaga qaytish" havolasi bor | 5 |

### D. Forma (20 ball)

| # | Talab | Ball |
|---|---|---|
| 15 | `contact.html` da `action` va `method` atributlari bilan `<form>` bor | 5 |
| 16 | Har bir input mos `<label for="...">` va `name` atributiga ega | 5 |
| 17 | Kamida **4 xil input turi** ishlatilgan (masalan `text`, `email`, `tel`, `number`, `date`, `radio`, `checkbox`) | 5 |
| 18 | `<select>` yoki `<textarea>`, **yuborish tugmasi** va kamida bitta `required` maydon bor | 5 |

### E. Havolalar va aloqa (10 ball)

| # | Talab | Ball |
|---|---|---|
| 19 | Kamida **3 ta platforma** (Instagram, Telegram, WhatsApp va h.k.) uchun ijtimoiy tarmoq havolalari yangi oynada ochiladi (`target="_blank"`) | 5 |
| 20 | Aloqa ma'lumotlarida `mailto:` va `tel:` havolalari ishlatilgan; har bir sahifada footer bor | 5 |

---

## 5. Ballarni talqin qilish

| Ball | Natija |
|---|---|
| 90-100 | A'lo |
| 75-89 | Yaxshi |
| 60-74 | O'tdi |
| 0-59 | O'tmadi: qayta topshirishi kerak |

**Tavsiya etiladigan ball ayirish:**

- CSS yoki JavaScript ishlatilgan bo'lsa: **-10 ball**
- Sahifalar orasidagi buzilgan havolalar: #11 talab bo'yicha hisoblanadi
- Ko'chirilgan ish: **0 ball**

---

## 6. Namunaviy yechim tuzilmasi

```
my-website/
├── index.html      → Men haqimda (1): #intro, #education, #hobbies
├── about2.html     → Men haqimda (2): #background, #experience, #goals
├── skills.html     → Nima qila olaman: #skills, #services, #projects
└── contact.html    → #contact-form, #socials
```

### Minimal sahifa shabloni

```html
<!DOCTYPE html>
<html lang="uz">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Men haqimda - 1-sahifa</title>
</head>
<body id="page-about-1">

  <header id="site-header">
    <h1>O'quvchi ismi</h1>

    <nav id="main-nav" aria-label="Asosiy navigatsiya">
      <ul>
        <li><a href="index.html">Men haqimda (1)</a></li>
        <li><a href="about2.html">Men haqimda (2)</a></li>
        <li><a href="skills.html">Nima qila olaman</a></li>
        <li><a href="contact.html">Aloqa</a></li>
      </ul>
    </nav>
  </header>

  <main id="main-content">
    <section id="intro">
      <h2>Tanishtiruv</h2>
      <p>...</p>
    </section>
  </main>

  <footer id="site-footer">
    <p>&copy; 2026 O'quvchi ismi</p>
  </footer>

</body>
</html>
```

### Minimal forma namunasi

```html
<form action="#" method="post" id="form-contact">
  <p>
    <label for="fullname">To'liq ism:</label>
    <input type="text" id="fullname" name="fullname" required>
  </p>
  <p>
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>
  </p>
  <p>
    <label for="message">Xabar:</label>
    <textarea id="message" name="message" rows="5"></textarea>
  </p>
  <button type="submit">Yuborish</button>
</form>
```

---

## 7. O'qituvchilar buni qanday ishlatishi mumkin

1. **Imtihon sifatida:** 3-bo'limni (topshiriq) o'quvchilarga bering, 4-bo'limni (mezon) baholash uchun o'zingizda saqlang.
2. **Dars namunasi sifatida:** namunaviy yechimni ko'rsating va har bir talabni birma-bir tushuntiring.
3. **O'z-o'zini tekshirish uchun:** o'quvchilarga mezonni bering, ular topshirishdan oldin ishlarini o'zlari baholasin.
4. **CSS imtihoni uchun asos sifatida:** o'quvchilarning HTML ini saqlab qo'ying va uni bezashni so'rang. Har bir bo'lim noyob `id` ga ega bo'lgani uchun ular `#id` selektorlari, `header` / `nav` / `main` / `footer` maketi, forma, jadval va ro'yxatlarni bezash kabilarni mashq qilishlari mumkin.

### Tezkor tekshiruv ro'yxati

- [ ] Barcha 4 fayl mavjud va brauzerda ochiladi
- [ ] CSS / JS ishlatilmagan
- [ ] Har bir sahifada bir xil nav va footer bor
- [ ] Bo'lim id lari noyob va anchor havolalar ishlaydi
- [ ] Formada label, turli input turlari va yuborish tugmasi bor
- [ ] Ijtimoiy tarmoq havolalari yangi oynada ochiladi

---

## 8. O'quvchilarning odatiy xatolari

| Xato | Nima uchun muhim |
|---|---|
| Hamma joyda `<div>` ishlatish | Semantik HTML ma'nosini yo'qotadi |
| Bir sahifada bir nechta `<h1>` | Sarlavhalar ierarxiyasini buzadi |
| Sarlavha darajasini o'lchamiga qarab tanlash | Sarlavhalar tuzilmani bildiradi, ko'rinishni emas |
| Takrorlanuvchi `id` qiymatlari | Id lar sahifada noyob bo'lishi kerak |
| `<label>` siz inputlar | Foydalanish qulayligi (accessibility) yomonlashadi |
| Noto'g'ri nisbiy yo'llar | Fayllar bir papkada bo'lishi kerak |
| Qoldirilgan namuna matn (`[Ismingiz]`) | Kontent to'liq emas |

---

## 9. Qo'shimcha g'oyalar (ixtiyoriy)

- Xuddi shu sayt ustiga CSS imtihoni qo'shish (ranglar, maket, navigatsiya paneli, forma dizayni)
- To'g'ri `alt` atributi bilan rasm qo'shish
- `<video>` yoki `<audio>` elementi qo'shish
- Favicon va meta description qo'shish

---

*Bu topshiriqni o'z darslaringiz uchun erkin nusxalashingiz, tarjima qilishingiz va moslashtirishingiz mumkin.*