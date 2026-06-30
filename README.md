# SaaS Guide 🌟

> **Complete guide to launching your SaaS in 2025** — From idea to first paying users.

**🌍 Live sites:**
- GitHub Pages: [https://ucfzem.github.io/saas-guide](https://ucfzem.github.io/saas-guide)
- Vercel: [https://saas-guide-ten.vercel.app](https://saas-guide-ten.vercel.app)
- GitHub Repo: [https://github.com/ucfzem/saas-guide](https://github.com/ucfzem/saas-guide)

---

## Features

- 🎨 **Theme** — Dark mode default (brown `#1a1412` bg, gold/yellow accents, white text)  
  ↳ Toggle to light mode (beige `#fcf9f5` bg, brown/gold accents, dark brown text)
- 🌐 **4 Languages** — Français (FR 🇫🇷), English (EN 🇬🇧), Español (ES 🇪🇸), العربية (AR 🇲🇦)
- 📱 **Fully responsive** — built with Tailwind CSS, scrollable lang bar on mobile
- 📊 **Interactive MRR calculator** — sliders for users & price
- ✅ **Validation checklist** — interactive checkboxes
- ❓ **FAQ accordion** — click to expand answers
- ⚡ **Dark/Light mode toggle** — persists on switch
- 🏗️ **Build in Public section** — example tweets
- 📈 **SaaS metrics bars** — Churn, MRR Growth, LTV:CAC, Activation, NPS
- 💰 **Pricing examples** — Starter/Pro/Enterprise with popularity metrics

## Files

| File | Description |
|------|-------------|
| `index.html` | Main HTML file (all-in-one, no build step) |
| `vercel.json` | Vercel static deployment config |
| `README.md` | This documentation |

## Color Palette

**Dark mode (default):**
- Background: `#1a1412` (deep brown)
- Cards: `rgba(74,44,26,0.6)` with blur
- Accents: Gold (`#d97706`, `#f59e0b`), Yellow (`#fbbf24`, `#facc15`)
- Text: `#f5f0e6` (warm white)
- Code blocks: `#2d1f1a`

**Light mode (toggle):**
- Background: `#fcf9f5` (warm beige)
- Cards: `rgba(248,240,230,0.85)`
- Accents: Brown (`#8b5e3c`, `#a67b56`), Gold
- Text: `#4d3521` (dark brown)
- Code blocks: `#f5f0e6`

## Languages

4 languages implemented via `data-i18n` attributes + JavaScript translations object:
- **FR** — Default, full French content
- **EN** — Full English translation
- **ES** — Full Spanish translation
- **AR** — Full Arabic translation, RTL direction, Moroccan flag 🇲🇦

Language switcher in nav bar with scrollable container on mobile.

## Deployment

- **GitHub Pages:** Auto-deploy on push to `main` branch
- **Vercel:** Static deployment via `vercel.json`

### Update deployed sites

```bash
# Push to GitHub (auto-deploys Pages)
git push origin main

# Deploy to Vercel
vercel --prod --yes
```

## Author

Made by [**ucfzem**](https://ucfzem.github.io/works) — Check out [SaaS projects](https://ucfzem.github.io/works) and [Blog](https://ucfzem.github.io/ucfzem-blog/)
