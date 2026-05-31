# Pavan Sai Tatineni — Portfolio

Dark-themed portfolio with neon accents. Built with HTML, CSS, and JavaScript.

---

## 🚀 Run in VS Code

1. Open the `portfolio/` folder in VS Code
2. Install the **Live Server** extension (if not already)
3. Right-click `index.html` → **Open with Live Server**
4. Opens at `http://localhost:5500` with auto-reload on save

---

## 📤 Deploy to GitHub Pages (free hosting)

```bash
# From inside the portfolio folder:
git init
git add .
git commit -m "Portfolio launch"
git branch -M main
git remote add origin https://github.com/Pavansai0409/portfolio.git
git push -u origin main
```

Then in GitHub:
- Go to your repo → **Settings** → **Pages**
- Source: **main** branch, **/ (root)**
- Click **Save**

Your site will be live at: `https://pavansai0409.github.io/portfolio`

---

## 🌐 Custom Domain: pavansai-portfolio.com

To get `https://pavansai-portfolio.com` to show your portfolio:

### Step 1: Buy the domain
- Buy `pavansai-portfolio.com` from [Namecheap](https://namecheap.com), [GoDaddy](https://godaddy.com), or [Google Domains](https://domains.google)
- Cost: ~₹800–1200/year

### Step 2: Add CNAME file to your repo
Create a file named `CNAME` (no extension) in the root of your portfolio folder containing:
```
pavansai-portfolio.com
```

### Step 3: Configure DNS at your domain registrar
Add these DNS records in your registrar's DNS settings:

**A Records** (point to GitHub's IPs):
```
Type: A  |  Host: @  |  Value: 185.199.108.153
Type: A  |  Host: @  |  Value: 185.199.109.153
Type: A  |  Host: @  |  Value: 185.199.110.153
Type: A  |  Host: @  |  Value: 185.199.111.153
```

**CNAME Record** (for www):
```
Type: CNAME  |  Host: www  |  Value: pavansai0409.github.io
```

### Step 4: Set custom domain in GitHub Pages
- Repo → Settings → Pages → Custom domain → type `pavansai-portfolio.com` → Save
- Tick **Enforce HTTPS** (wait ~5 minutes after DNS propagates)

### DNS propagation
DNS changes take 10 minutes to 24 hours. Check status at [dnschecker.org](https://dnschecker.org).

---

## ✏️ How to update content

| What to change | Where |
|---|---|
| Text, sections, links | `index.html` |
| Colors, fonts, spacing | `style.css` (edit `:root` variables at top) |
| Add a project | Copy a `project-card` div in `index.html` |
| Add a certification | Copy a `cert-card` div in `index.html` |
| Add interactivity | `script.js` |

## 🔄 After making changes

```bash
git add .
git commit -m "Updated portfolio"
git push
```

GitHub Pages auto-updates in ~1 minute.

---

## 🎨 Theme colors

Edit in `style.css`:
```css
:root {
  --neon:  #00ffaa;   /* Main green accent */
  --neon2: #00ccff;   /* Blue accent */
  --neon3: #a855f7;   /* Purple accent */
  --bg:    #0a0a0f;   /* Background */
}
```
