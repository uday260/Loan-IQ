# 🏠 LoanIQ — Deployment & Monetization Guide

## STEP 1 — Test locally
Open `index.html` in your browser. Everything works offline (no internet needed for the calculator).

---

## STEP 2 — Host on GitHub Pages (Free, 10 min)

### 2a. Create GitHub account
1. Go to https://github.com and sign up (free)
2. Verify your email

### 2b. Create repository
1. Click **"New repository"** (green button)
2. Name it: `loaniq` (or any name you like)
3. Set to **Public** (required for free GitHub Pages)
4. Click **"Create repository"**

### 2c. Upload your files
1. Click **"uploading an existing file"** link
2. Drag and drop `index.html` into the upload area
3. Click **"Commit changes"**

### 2d. Enable GitHub Pages
1. Go to your repository → **Settings** tab
2. Scroll to **"Pages"** in the left sidebar
3. Under **Source**, select **"Deploy from a branch"**
4. Branch: **main**, Folder: **/ (root)**
5. Click **Save**
6. Wait 2-3 minutes → your site is live at:
   `https://YOUR-USERNAME.github.io/loaniq/`

### 2e. Share the link!
Your testing URL: `https://YOUR-USERNAME.github.io/loaniq/`
Share this with friends to test.

---

## STEP 3 — Get a Custom Domain (Optional, ₹800/year)

A custom domain (loaniq.in) makes it look professional and helps SEO.

1. Buy domain at **GoDaddy.in** or **Namecheap.com**
   - Suggested: `loaniq.in` or `emicalculator.co.in`
   - Cost: ₹600–900/year

2. In GitHub Pages settings, enter your custom domain
3. At your domain registrar, add DNS records:
   ```
   A record: 185.199.108.153
   A record: 185.199.109.153
   A record: 185.199.110.153
   A record: 185.199.111.153
   CNAME: www → YOUR-USERNAME.github.io
   ```
4. Check "Enforce HTTPS" in GitHub Pages settings

---

## STEP 4 — Google Analytics (Track visitors)

1. Go to https://analytics.google.com
2. Create account → Create Property → Web
3. Enter your site URL
4. Copy your **Measurement ID** (format: G-XXXXXXXXXX)
5. In `index.html`, find this comment and replace:
   ```html
   <!-- <script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script> -->
   ```
   Uncomment and replace `G-XXXXXXXXXX` with your real ID.

---

## STEP 5 — Google AdSense (Earn from ads)

### Requirements before applying:
- Your site must be live for at least 2-4 weeks
- Must have real content (not just a calculator — add a blog!)
- Need 20-30 genuine visitors per day

### How to apply:
1. Go to https://adsense.google.com
2. Sign in with your Google account
3. Enter your website URL
4. Add the AdSense verification code to your `<head>`
5. Wait 2-4 weeks for approval

### After approval, replace ad slots:
In `index.html`, find all `[Ad Slot — ...]` placeholders.
Replace with your actual AdSense code:
```html
<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-XXXXXXXXXXXXXXXX"
     data-ad-slot="XXXXXXXXXX"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>
<script>(adsbygoogle = window.adsbygoogle || []).push({});</script>
```

### Expected earnings:
- Financial niche CPC: ₹8–40 per click (very high!)
- 1000 visitors/day → ₹500–2000/day from ads alone
- 10,000 visitors/day → ₹5,000–15,000/day

---

## STEP 6 — Affiliate Marketing (Biggest income potential)

### BankBazaar Affiliate Program
- URL: https://www.bankbazaar.com/affiliate.html
- Commission: ₹500–2000 per approved loan application
- Replace `href="#"` in affiliate cards with your tracking link

### PaisaBazaar Affiliate Program
- URL: https://www.paisabazaar.com/affiliate/
- Commission: ₹300–1500 per lead

### Direct Bank Programs
- SBI: Contact your nearest SBI branch for DSA empanelment
- HDFC: https://www.hdfc.com/dsa-registration
- Commission: ₹3,000–10,000 per sanctioned loan

### How to replace affiliate links:
In `index.html`, search for `href="#"` in affiliate cards.
Replace with your actual affiliate tracking links.

---

## STEP 7 — SEO & Traffic (Most important!)

### Update these meta tags in index.html:
```html
<link rel="canonical" href="https://YOUR-DOMAIN.in/">
<meta property="og:url" content="https://YOUR-DOMAIN.in/">
```

### Add blog posts (create new HTML files):
- `how-to-reduce-home-loan-interest.html`
- `should-i-prepay-home-loan-or-invest.html`
- `best-home-loan-rates-india-2025.html`

Each article → more Google traffic → more ad clicks + affiliate conversions.

### Target keywords (high traffic, low competition):
1. "home loan prepayment calculator" — 22,000 searches/month
2. "EMI calculator India" — 180,000 searches/month
3. "should I prepay home loan" — 8,000 searches/month
4. "home loan interest calculator 2025" — 15,000 searches/month

### Share on communities:
- Reddit: r/IndiaInvestments, r/personalfinanceindia
- Quora: Answer home loan questions, link your calculator
- WhatsApp groups: Personal finance groups
- LinkedIn: Post a screenshot with savings example

---

## STEP 8 — Monetization Timeline

| Month | Action | Expected Income |
|-------|--------|-----------------|
| 1 | Launch, share with 50 friends | ₹0 (testing) |
| 2-3 | Submit to Google, build SEO | ₹0 (building) |
| 4-6 | AdSense approved, 500 visitors/day | ₹3,000–8,000/month |
| 7-12 | 2000 visitors/day, affiliate links active | ₹15,000–40,000/month |
| Year 2 | 10,000+ visitors/day | ₹60,000–2,00,000/month |

---

## TODO Checklist

- [ ] Create GitHub account
- [ ] Upload index.html to GitHub
- [ ] Enable GitHub Pages
- [ ] Test on mobile
- [ ] Share link with 10 friends for feedback
- [ ] Buy custom domain (optional)
- [ ] Set up Google Analytics
- [ ] Apply for AdSense (after 2-3 weeks of traffic)
- [ ] Sign up for BankBazaar/PaisaBazaar affiliate
- [ ] Replace affiliate `href="#"` with real links
- [ ] Replace `TODO` items in index.html (canonical URL, OG image)
- [ ] Write first blog article

---

## Support
Questions? The key files to edit:
- `index.html` — everything is in one file
- Search for `TODO` to find all items needing your attention
- Search for `XXXXXXXX` to find all placeholder IDs

