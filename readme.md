# 🌞 Maharaja Solar — GitHub Pages Deployment Guide

## Files आपको मिले हैं:
- `index.html` — Complete website

---

## 🚀 GitHub Pages पर Deploy करने के Steps:

### Step 1 — GitHub Account बनाएं (अगर नहीं है)
👉 https://github.com/signup पर जाएं और free account बनाएं।

### Step 2 — New Repository बनाएं
1. GitHub पर login करें
2. ऊपर right में `+` → **New Repository** click करें
3. Repository name: `maharaja-solar` (या कोई भी नाम)
4. **Public** select करें (GitHub Pages free में Public repo पर काम करती है)
5. **Create repository** click करें

### Step 3 — index.html Upload करें
1. Repository page पर **"uploading an existing file"** link click करें
2. `index.html` drag & drop करें
3. नीचे **Commit changes** click करें

### Step 4 — GitHub Pages Enable करें
1. Repository में **Settings** tab click करें
2. Left sidebar में **Pages** click करें
3. **Source** के नीचे: Branch → `main`, Folder → `/ (root)` select करें
4. **Save** click करें

### Step 5 — Your Website is LIVE! 🎉
कुछ minutes में आपकी website इस URL पर live होगी:
```
https://YOUR-USERNAME.github.io/maharaja-solar/
```
(YOUR-USERNAME = आपका GitHub username)

---

## 📝 Form Submission के लिए (Optional upgrade):
अभी form submit होने पर success message दिखता है।
Real email notifications के लिए **Formspree** use करें (free):

1. https://formspree.io पर signup करें
2. New form बनाएं, अपना email add करें
3. Form का endpoint मिलेगा जैसे: `https://formspree.io/f/XXXXXXXX`
4. `index.html` में `submitForm()` function में यह line add करें:

```javascript
await fetch('https://formspree.io/f/YOUR_ID', {
  method: 'POST',
  headers: {'Content-Type': 'application/json'},
  body: JSON.stringify({ name, mobile, district })
});
```

---

## 📱 Custom Domain (Optional):
अगर आप `maharajasolar.com` जैसा domain चाहते हैं:
1. Godaddy/Namecheap से domain खरीदें (~₹500-800/year)
2. GitHub Pages Settings → Custom Domain में add करें
3. Domain provider के DNS में CNAME record add करें

---

## ✅ Website Features Summary:
- ☀ Hero section with animated sun & stars
- 📊 Subsidy table (1kW → 3kW with amounts)
- ⚡ kW comparison cards (1/2/3/5 kW guide)
- ⚙️ On-Grid / Off-Grid / Hybrid explained
- 📋 5-step process guide
- 📁 Required documents section (Aadhaar, Bill, Passbook)
- ❓ FAQ accordion (6 questions)
- 📝 Application form with file upload
- 📞 Contact section
- 📱 Mobile responsive
- 🏛️ Official portal link (pmsuryaghar.gov.in)
