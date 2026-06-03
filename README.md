# DRAPE — Fashion Store

A complete, no-backend clothing shop website. Customers browse and order freely; you manage stock from a hidden admin panel.

---

## 🚀 Deploy to GitHub Pages (Free Hosting)

### Step 1 — Create a GitHub repository
1. Go to [github.com](https://github.com) and sign in (or create a free account).
2. Click **New** → give it a name like `drape-store`.
3. Make it **Public**, leave everything else default, click **Create repository**.

### Step 2 — Upload your files
**Option A — Drag & Drop (easiest):**
1. Open your new repository on GitHub.
2. Click **uploading an existing file**.
3. Drag ALL the files and folders (`index.html`, `admin.html`, `css/`, `js/`) into the upload area.
4. Click **Commit changes**.

**Option B — Using Git (if you have it installed):**
```bash
git init
git add .
git commit -m "Initial store launch"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/drape-store.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages
1. In your repository, go to **Settings** → **Pages**.
2. Under **Source**, select `Deploy from a branch`.
3. Choose **main** branch, **/ (root)** folder.
4. Click **Save**.
5. Wait 1–2 minutes. Your site will be live at:
   `https://YOUR_USERNAME.github.io/drape-store/`

---

## 🔐 Admin Panel

**URL:** `https://your-site-url/admin.html`

**Default password:** `drape2025`

> ⚠️ **Change your password before going live!**
> Open `js/admin.js` and change the value on this line:
> ```js
> const ADMIN_PASSWORD = 'drape2025';
> ```
> Replace `drape2025` with your own secure password, then save and re-upload the file.

**What you can do in admin:**
- ➕ Add new clothing items with photos, price, stock, sizes
- ✏️ Edit existing products
- 🗑️ Delete products
- 📋 View all customer orders (name, phone, items ordered)

---

## 🛍️ How it works for customers

1. Browse the store at your main URL.
2. Click any product to see a quick view.
3. Add items to cart.
4. Click the cart icon → **Proceed to Checkout**.
5. Enter their **name** and **phone number** (no account needed).
6. Place order — you see it instantly in the admin panel.

---

## 📁 File Structure

```
drape-store/
├── index.html          ← Customer store
├── admin.html          ← Admin panel (password protected)
├── css/
│   ├── style.css       ← Store styles
│   └── admin.css       ← Admin styles
└── js/
    ├── data.js         ← localStorage data layer
    ├── store.js        ← Store logic
    └── admin.js        ← Admin logic (change password here)
```

---

## 💡 Tips

- **Product images:** Upload real photos of your clothes when adding products in admin. Supported formats: JPG, PNG, WEBP (max 5MB each).
- **Data storage:** All products, orders and cart data are stored in the visitor's browser (`localStorage`). This means each device has its own data. For a shared database, you'd need a backend service.
- **Orders:** Orders are saved in the browser where the admin session runs. Keep an eye on the admin Orders tab regularly.
- **Customise the name:** Replace "DRAPE" with your store name by doing Find & Replace across `index.html`, `admin.html`, and `css/style.css`.

---

Made with ❤️ — Pure HTML, CSS & JavaScript. No server required.
