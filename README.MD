<div align="center">

<img src="https://capsule-render.vercel.app/api?type=slice&color=0:000000,100:00ff41&height=160&section=header&text=GitHub%20Control%20Panel&fontSize=38&fontColor=00ff41&fontAlignY=45&animation=twinkling" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=20&pause=1000&color=00FF41&background=000000&center=true&vCenter=true&width=750&lines=root%40github-control%3A~%24+connect;%3E+single-file+HTML+%2B+CSS+%2B+JS;%3E+no+backend%2C+no+build+step;%3E+direct+GitHub+REST+API+access" alt="Typing SVG" />

</div>

<br/>

```bash
$ cat about.log
------------------------------------------------------------
[INFO]  Type       : Single-file HTML/CSS/JS tool
[INFO]  Backend    : none (100% client-side)
[INFO]  API        : GitHub REST API (api.github.com)
[INFO]  Auth       : Personal Access Token (in-memory only)
[INFO]  Theme      : terminal / hacker style
------------------------------------------------------------
```

## `> what_it_does`

Brauzerda ochiladigan bitta HTML fayl orqali GitHub akkauntingizni boshqarish uchun panel. Hech qanday server, hech qanday build jarayoni kerak emas — faylni ochasiz, tokeningizni kiritasiz va ishlaysiz.

## `> features`

```
[x] repo va branch tanlash / almashtirish
[x] fayl va papkalarni ko'zib chiqish (breadcrumb navigatsiya)
[x] fayl yaratish / tahrirlash / o'chirish
[x] butun papkani (subfolder'lari bilan) bitta commit orqali yuklash
[x] tashqi papka nomisiz, faqat ichidagi fayllarni yuklash rejimi
[x] commit tarixini ko'rish
[x] yangi repo yaratish / mavjud repo'ni o'chirish
[x] branch yaratish / o'chirish
[x] repo sozlamalari: nom, ko'rinish (public/private), tavsif
```

## `> quick_start`

1. `github-control-panel.html` faylini brauzerda oching (double-click yetarli)
2. GitHub'da token yarating: **Settings → Developer settings → Personal access tokens**
   - Classic token: `repo` va `delete_repo` scope'larini belgilang
   - Fine-grained token: `Contents`, `Administration`, `Metadata` — Read and write
3. Tokenni panelga kiriting → `connect`
4. Repo va branch tanlang, kerakli tab (`files` / `upload folder` / `commits` / `repos`) orqali ishlang

## `> security_notes`

```diff
+ Token faqat brauzer xotirasida (RAM) saqlanadi
+ Har bir so'rov to'g'ridan-to'g'ri api.github.com ga ketadi
+ Hech qanday uchinchi tomon serveriga ma'lumot yuborilmaydi
- Sahifani yopsangiz yoki yangilasangiz, token yo'qoladi (qayta kiritish kerak)
- Tokenni hech qachon boshqalar bilan (jumladan skrinshot/chatlarda) baham ko'rmang
```

## `> tech_stack`

```
HTML5, vanilla CSS (custom properties), vanilla JavaScript (fetch API)
GitHub REST API v3 (git/blobs, git/trees, git/commits, git/refs, contents)
```

## `> access token olish`

```
1.Github accountizga kirasiz
2.Profil=>Settings=>Developer Settings
3.Personal access token=>Tokens(classic)=>Generate new tokens(classic)
4.Nom va hamma joyiga ruxsat berasiz
5.ghp_m3xxxxxxxxxxxxxxxxxxxx shuni nushalisiz
```

## `> limitations`

GitHub'ning o'zi qo'ygan huquq va rate limit'lari (soatiga ~5000 so'rov) baribir amal qiladi — bu vosita ularni chetlab o'tolmaydi, faqat mavjud API imkoniyatlarini qulay GUI orqali taqdim etadi.

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=slice&color=0:00ff41,100:000000&height=90&section=footer" width="100%"/>
</div>
</div>
