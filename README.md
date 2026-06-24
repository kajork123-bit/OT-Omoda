# 💰 OT Tracker – Omoda-Jecoo

Personal OT and salary tracking app for Omoda-Jecoo staff. Runs entirely in the browser — no server, no sign-up.

## ✨ Features

- 🔐 **PIN lock** with brute-force protection (lockout after 5 failed attempts)
- ⏱ **OT logging** — daily OT×1 / OT×1.5 / OT×3 with auto-calculated baht amounts
- 💵 **Income summary** — base salary + OT + Saturday bonus + daily allowances
- 💸 **Expense tracker** — per-period expenses with paid/unpaid status
- 📈 **Statistics** — cumulative totals, monthly comparison charts, income forecast
- 🎨 **4 color themes** — Cyan / Purple / Green / Warm
- 🌙 **Dark / Light mode** toggle
- 📅 **Thai public holidays** highlighted in the OT table (2025–2026)
- 👆 **Swipe gestures** to switch tabs on mobile
- 📳 **Haptic feedback** on mobile devices
- 💾 **Auto-save** to localStorage — data persists across sessions
- 📤 **JSON export/import** for backup

## 🚀 Usage

Open **[index.html](index.html)** directly in a browser, or visit the GitHub Pages URL.

Default PIN: `1234` — change it immediately in Settings ⚙️

## 🗂 Project Structure

```
index.html    — single-file app (HTML + CSS + JS, no build step)
README.md     — this file
.nojekyll     — tells GitHub Pages not to use Jekyll
```

## 🌐 Deploy to GitHub Pages

1. Push this folder to a GitHub repository
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch → main → / (root)**
4. Your app will be live at `https://<username>.github.io/<repo-name>/`

## 📱 Mobile

Works as a PWA-style web app. On iOS: Safari → Share → Add to Home Screen.  
On Android: Chrome → Menu → Add to Home Screen.

## ⚙️ Customization

All constants are at the top of the `<script>` section in `index.html`:

| Constant | Default | Description |
|---|---|---|
| `SAT_BONUS` | 300 | Saturday OT bonus (฿) |
| `RENT_AMT` | 1,200 | Monthly rent allowance (฿) |
| `DILIGENCE_AMT` | 1,000 | Diligence bonus (฿) |
| `TRAVEL_RATE` | 50 | Daily travel allowance (฿) |
| `LUNCH_RATE` | 50 | Daily lunch allowance (฿) |
| `FOOD_OT_RATE` | 50 | OT meal allowance (฿) |
| `SHIFT_RATE` | 100 | Daily shift allowance (฿) |
| `MAX_OT_HOURS` | 16 | Max OT hours per day |

---

> Data is stored locally in your browser (`localStorage`). Use **Export JSON** to back up your data.
