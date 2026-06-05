# Keshav Singla — Portfolio Setup

Your portfolio is in `index.html` (single file, zero build tools).

---

## ⭐ TWO QUICK TO-DOS (do these now)

### A. Activate the contact form (1 click)
You already received an email from **FormSubmit** titled
"Action Required: Activate FormSubmit…". Open it and click **ACTIVATE FORM**.
After that, every contact-form submission lands in your inbox automatically.
(Until then the form falls back to opening the visitor's mail app.)

### B. Turn on analytics (2 min, free, privacy-friendly)
The site already includes the GoatCounter snippet — you just need a code:
1. Go to **https://www.goatcounter.com** → "Sign up" (free).
2. Pick a site code, e.g. **keshavsingla** → you get `keshavsingla.goatcounter.com`.
3. In `index.html`, search for **`YOURCODE`** and replace it with your code:
   ```html
   data-goatcounter="https://keshavsingla.goatcounter.com/count"
   ```
4. Commit & push. Visit your dashboard at `https://keshavsingla.goatcounter.com`
   to see visitors — no cookies, no personal data collected.

(If you skip this, nothing breaks — the snippet just won't count anything.)

---

## 1. Add your résumé  ⚠️ (button is already live)

Drop your résumé into this folder named **exactly**:

```
Keshav_Singla_Resume.pdf
```

The "↓ RÉSUMÉ" button in the nav bar and hero will then download it.
Until you add it, the button will 404.

---

## 2. Add your photo (optional but recommended)

Drop a square-ish photo into this folder named **exactly**:

```
profile.jpg
```

It auto-fills the hexagon frame in the hero.
If no `profile.jpg` exists, it gracefully falls back to the glowing "KS" initials —
so nothing breaks either way.

Tip: a 600×600px headshot looks best.

---

## 3. Make the contact form land in your inbox (silent — no mail client popup)

Right now the form uses a **mailto fallback** (opens the visitor's email app).
To receive messages silently in your inbox:

1. Go to **https://formspree.io** → sign up (free, 50 submissions/month)
2. Create a new form → connect `keshavsingla940@gmail.com`
3. Copy your form ID (looks like `xeqyabcd`)
4. In `index.html`, find this line (search for `FORM_ID`):

   ```html
   <form id="contactForm" ... action="https://formspree.io/f/FORM_ID" ...>
   ```

5. Replace `FORM_ID` with your real ID:

   ```html
   action="https://formspree.io/f/xeqyabcd"
   ```

Done. Messages now arrive in your inbox without opening anyone's mail client.
(If you skip this, the form still works via the mailto fallback.)

---

## Deploy

- **Vercel:**  `vercel`  in this folder, or import the repo at vercel.com
- **Netlify:**  drag this folder onto netlify.com/drop
- **GitHub Pages:**  push to a repo → Settings → Pages → deploy from main

All three host this as-is with zero config.

---

## TODO reminder
When your GitHub handle migration finishes, search `index.html` for
`keshavhacker1609` and replace with `keshavsingla`.
