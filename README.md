# Arrow Architect Website
**Ajeesh | Rajajinagar, Bangalore**

A professional architecture portfolio website with booking calendar, WhatsApp integration, Google Analytics, and a CMS for content updates.

---

## 📁 Folder Structure

```
arrow-architect/
├── index.html          ← Main website (homepage)
├── netlify.toml        ← Netlify configuration
├── css/
│   └── style.css       ← All styling
├── js/
│   └── main.js         ← All interactivity, calendar, WhatsApp
├── admin/
│   ├── index.html      ← CMS login panel
│   └── config.yml      ← CMS fields configuration
├── images/             ← Upload your project photos here
│   └── (your photos)
└── projects/           ← CMS-managed project data
```

---

## 🚀 Going Live (Step by Step)

### Step 1 — Upload to GitHub
1. Go to github.com → Sign up / Log in
2. Click **New Repository** → name it `arrow-architect`
3. Set to **Public** → Create Repository
4. Click **"uploading an existing file"** → drag your entire folder in
5. Click **Commit changes**

### Step 2 — Deploy on Netlify
1. Go to netlify.com → Sign up with GitHub
2. Click **"Add new site" → "Import an existing project"**
3. Choose GitHub → select `arrow-architect`
4. Click **Deploy Site** — live in 2 minutes ✅

### Step 3 — Enable Contact Form Emails
1. In Netlify → **Site Settings → Forms**
2. Click your `contact` form → **Form Notifications**
3. Add your email → save
4. Every enquiry now arrives in your inbox ✅

### Step 4 — Enable CMS (Content Manager)
1. In Netlify → **Site Settings → Identity → Enable Identity**
2. Then → **Git Gateway → Enable Git Gateway**
3. Visit `yoursite.netlify.app/admin` → Invite yourself
4. You can now add/edit projects, services, and contact info from a dashboard ✅

---

## ✏️ Things To Personalise

Open `js/main.js` and update:
```javascript
const WHATSAPP_NUMBER = "919XXXXXXXXX"; // Your number e.g. "919845001234"
```

Open `index.html` and update:
```html
<!-- Line 14 & 18 -->
gtag('config', 'G-XXXXXXXXXX'); // Your Google Analytics ID
```

Also in `index.html`, search for `<!-- REPLACE` comments — they guide you to update:
- Your phone number
- Your email address
- Your photo (in the About section)
- Your project images (in the Portfolio section)
- Your social media links

---

## 📸 Adding Your Photos

1. Put your photos in the `images/` folder
2. In `index.html`, find the portfolio section and replace:
```html
<div class="portfolio-item-bg">Upload Project Image</div>
```
with:
```html
<img src="images/your-photo.jpg" style="position:absolute;inset:0;width:100%;height:100%;object-fit:cover;">
```

---

## 📅 Managing Booking Availability

Open `js/main.js` and find `BOOKED_SLOTS`:
```javascript
const BOOKED_SLOTS = {
  "2025-04-15": ["10:00 AM", "11:00 AM"],  // These times are blocked on this date
  "2025-04-18": ["2:00 PM", "4:00 PM"],
};
```
Add dates and times you're NOT available to block them out.

---

## 🌐 Custom Domain Setup

1. Buy `arrowarchitect.in` from GoDaddy or Namecheap (~₹1000/year)
2. In Netlify → **Domain Settings → Add custom domain**
3. Copy the DNS records Netlify gives you
4. Paste them into your domain registrar's DNS settings
5. Wait 24–48 hours → your site is live at arrowarchitect.in ✅

---

*Built for Arrow Architect by Claude · 2025*
