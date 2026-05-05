# My Website — Owner's Guide

A simple one-page website hosted **for free** on GitHub Pages.
You only need to edit **one file** (`index.html`) to update your website. No coding knowledge required!

---

## 🌐 Your Live Website

Your site is live at: **https://www.smmthes.gr**

*(Until the custom domain is set up, you can also use: `https://eyagfrag.github.io/dtc_geoquest/github-pages-template/`)*

---

## 📁 What's in This Repository

| File/Folder | What it does |
|---|---|
| `index.html` | **This is your website.** Edit this file to change all text and content. |
| `style.css` | Controls colors, fonts and layout. You probably won't need to touch this. |
| `images/` | Contains all your pictures. Replace them here. |
| `README.md` | This guide you're reading now. |

### Images folder

| Filename | Where it appears | Recommended size |
|---|---|---|
| `hero.jpg` | The big banner at the top of the page | 1920 × 800 pixels |
| `photo1.jpg` | "About Us" two-column section | 800 × 600 pixels |
| `photo2.jpg` | "Our Services" two-column section | 800 × 600 pixels |
| `photo3.jpg` | "More Information" two-column section | 800 × 600 pixels |
| `photo4.jpg` | Carousel slide 1 | 800 × 600 pixels |
| `photo5.jpg` | Carousel slide 2 | 800 × 600 pixels |
| `photo6.jpg` | Carousel slide 3 | 800 × 600 pixels |
| `photo7.jpg` | Carousel slide 4 | 800 × 600 pixels |
| `photo8.jpg` | Carousel slide 5 | 800 × 600 pixels |
| `photo9.jpg` | Carousel slide 6 | 800 × 600 pixels |

---

## ✏️ How to Update Your Website Text

### Step-by-step:

1. Go to your repository on [github.com](https://github.com)
2. Click on the file `index.html`
3. Click the **pencil icon** ✏️ (top right of the file) to edit
4. Make your changes (see the guides below)
5. Scroll down and click the green **"Commit changes"** button
6. Wait ~1 minute — your website will update automatically!

---

## 📝 What Can I Change and Where?

The `index.html` file is organized in **sections**. Each section is marked with a comment
that looks like `<!-- SECTION NAME -->`. You only need to change the text **between the tags**.

### Quick HTML crash course

HTML uses **tags** — they look like this:

```
<p>This is a paragraph of text.</p>
<h2>This is a heading.</h2>
```

- Tags come in pairs: an opening tag `<p>` and a closing tag `</p>`
- You only change the **text between the tags**
- **Don't delete the tags themselves!**

---

### 🖼️ 1. Hero Banner (the big image at the top)

Look for this section:
```html
<!-- HERO BANNER -->
<h1>Your Website Title</h1>
<p>A short tagline or description goes here</p>
```

- Change `Your Website Title` → to your actual website title
- Change `A short tagline or description goes here` → to your tagline

**To change the banner image:** replace the file `images/hero.jpg` with your own image (keep the same filename).

---

### 📖 2. Welcome / Intro Text

Look for this section:
```html
<!-- INTRO TEXT - full width pure text section -->
<h2>Welcome</h2>
<p>
    Add your introductory text here...
</p>
```

- Change `Welcome` → to any heading you want
- Replace the text between `<p>` and `</p>` with your own text
- **To add another paragraph**, copy and paste this block and write your text:
```html
<p>
    Your new paragraph goes here.
</p>
```

---

### 🏢 3. Two-Column Sections (text + image side by side)

There are **3 two-column sections**. Each one looks like this:
```html
<h2>About Us</h2>
<p>
    Write your main content here...
</p>
```
and
```html
<img src="images/photo1.jpg" alt="About us image">
```

- Change the heading (e.g. `About Us`, `Our Services`, `More Information`) to whatever you want
- Change the paragraph text between `<p>` and `</p>`
- The image changes when you replace the file in the `images/` folder

---

### 🎠 4. Photo Carousel (slideshow)

Look for this section:
```html
<!-- PHOTO CAROUSEL -->
<h2>Gallery</h2>
```

The carousel has **6 slides** using images `photo4.jpg` through `photo9.jpg`.
Each slide looks like this:
```html
<div class="carousel-slide">
    <img src="images/photo4.jpg" alt="Photo 4">
    <p>Caption for photo 4</p>
</div>
```

- Change `Caption for photo 4` → to your own caption
- Change `alt="Photo 4"` → to a short description of the image
- The images update when you replace files `photo4.jpg` to `photo9.jpg` in the `images/` folder

**To add a 7th slide**, copy one of the slide blocks above, paste it after the last one, and change the image to `images/photo10.jpg`. Then also add a new dot:
```html
<span class="dot" onclick="goToSlide(6)"></span>
```
*(The number starts at 0, so the 7th slide = `6`)*

---

### 📞 5. Footer (contact details)

Look for this section:
```html
<!-- FOOTER -->
<p>Email: <a href="mailto:your.email@example.com">your.email@example.com</a></p>
<p>Phone: +1 234 567 890</p>
<p>Address: 123 Street Name, City, Country</p>
```

- Replace `your.email@example.com` in **both places** (the `mailto:` AND the visible text)
- Replace the phone number and address
- Update the LinkedIn/Twitter links with your own URLs
- Change `Your Name` in the copyright line

---

## ��️ How to Replace Images

1. Go to the `images/` folder in your repository
2. Click **"Add file"** → **"Upload files"**
3. Upload your new image with the **exact same filename** (e.g. `hero.jpg`)
4. Click **"Commit changes"**
5. The website updates automatically in ~1 minute

> **💡 Tips for images:**
> - Use `.jpg` or `.png` format
> - Keep file sizes under 1MB for fast loading
> - Use the recommended sizes listed above for best results
> - Free image resizer: [iloveimg.com/resize-image](https://www.iloveimg.com/resize-image)

---

## 🎨 How to Change Colors (optional, advanced)

Open `style.css` and look for color codes like `#1a1a2e`.

| Color code | Where it's used |
|---|---|
| `#1a1a2e` | Headings and footer background (dark navy) |
| `#555` | Body text (grey) |
| `#7ec8e3` | Links in the footer (light blue) |

Pick new colors at [htmlcolorcodes.com](https://htmlcolorcodes.com/).

---

## 🚀 Initial Setup (one-time only)

1. Create a new repository on [github.com](https://github.com) → click **"New"**
2. Upload all the files from this folder to the repository
3. Go to **Settings** → **Pages** (in the left sidebar)
4. Under **"Source"**, select **"Deploy from a branch"**
5. Choose **`main`** branch and **`/ (root)`** folder
6. Click **Save**
7. Your site will be live in a few minutes! 🎉

---

## 🌍 Custom Domain Setup (www.smmthes.gr)

Your website uses a custom domain: **www.smmthes.gr**

The `CNAME` file in this repository is already configured. But for the domain to work,
you need to set up **DNS records** at your domain provider (e.g. Papaki, TopHost, or wherever you registered `smmthes.gr`).

### What to do at your domain provider:

Log in to your domain provider's control panel and go to **DNS Settings** (or "DNS Zone", "Manage DNS").
Add the following records:

#### For `www.smmthes.gr` — add a CNAME record:

| Type | Name | Value |
|------|------|-------|
| CNAME | www | `eyagfrag.github.io` |

#### For `smmthes.gr` (without www) — add these 4 A records:

| Type | Name | Value |
|------|------|-------|
| A | @ | `185.199.108.153` |
| A | @ | `185.199.109.153` |
| A | @ | `185.199.110.153` |
| A | @ | `185.199.111.153` |

### After adding DNS records:

1. Wait **1 to 24 hours** for the DNS changes to take effect (this is normal)
2. Go to **https://github.com/eyagfrag/dtc_geoquest/settings/pages**
3. In the **"Custom domain"** field, type `www.smmthes.gr` and click **Save**
4. Once GitHub verifies the domain, check the **"Enforce HTTPS"** checkbox for security
5. Your site will be live at **https://www.smmthes.gr** 🎉

### How to check if DNS is ready:

Visit [dnschecker.org](https://dnschecker.org/) and search for `www.smmthes.gr`.
If it shows `eyagfrag.github.io` as the result, the DNS is ready!

---

## ⚠️ Important Rules

- **Don't delete anything inside `< >`** — those are HTML tags and the site will break
- **Only change the text between tags**, not the tags themselves
- **Keep image filenames simple** — no spaces, no special characters
- **Test after each change** — wait 1 min, then refresh your website
- If something breaks, use the **History** button to revert (see below)

---

## 🆘 Something Went Wrong?

1. Go to your repository on GitHub
2. Click on `index.html`
3. Click **"History"** (top right)
4. Find the last version that worked
5. Click on it, then click **"..."** → **"Revert changes"**

This will restore your website to the previous working version. Don't panic! 😊
