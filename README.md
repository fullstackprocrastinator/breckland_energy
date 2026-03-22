# Breckland Energy

**EPC Assessments & Retrofit Services Built on Construction Expertise | Attleborough, Norfolk**

The website for Breckland Energy — a domestic energy assessment and PAS 2035 retrofit assessment service based in Attleborough, Norfolk NR17.

## Live Site

🌐 [https://yourusername.github.io/breckland-energy](https://yourusername.github.io/breckland-energy)

> Replace `yourusername` with your GitHub username once deployed.

## Pages

| File | Description |
|------|-------------|
| `index.html` | Main single-page website (home, about, services, coverage, process, contact) |
| `privacy.html` | Privacy Policy |
| `terms.html` | Terms & Conditions |

## Deploying to GitHub Pages

### 1. Create the repository

- Go to [github.com/new](https://github.com/new)
- Repository name: `breckland-energy` (or your preferred name)
- Set to **Public**
- Click **Create repository**

### 2. Upload the files

- Click **"uploading an existing file"** on the repository page
- Drag and drop all three HTML files (`index.html`, `privacy.html`, `terms.html`)
- Write a commit message (e.g. "Initial site upload")
- Click **Commit changes**

### 3. Enable GitHub Pages

- Go to **Settings** → **Pages** (in the left sidebar)
- Under **Source**, select **Deploy from a branch**
- Branch: **main**, folder: **/ (root)**
- Click **Save**
- Your site will be live within a minute or two at `https://yourusername.github.io/breckland-energy`

### 4. Custom domain (optional)

If you've registered `brecklandenergy.co.uk`, you can point it to GitHub Pages:

1. In your repository, go to **Settings** → **Pages**
2. Under **Custom domain**, enter `www.brecklandenergy.co.uk` and click **Save**
3. With your domain registrar, add these DNS records:

| Type | Name | Value |
|------|------|-------|
| CNAME | www | `yourusername.github.io` |
| A | @ | `185.199.108.153` |
| A | @ | `185.199.109.153` |
| A | @ | `185.199.110.153` |
| A | @ | `185.199.111.153` |

4. Tick **Enforce HTTPS** once the certificate is provisioned (usually takes a few minutes)

## Tech Stack

- Pure HTML, CSS, and vanilla JavaScript — no build tools, no frameworks, no dependencies
- Google Fonts (DM Serif Display, Outfit)
- Fully responsive (mobile, tablet, desktop)
- All logos embedded as inline SVGs (zero external image dependencies)

## Making Changes

All files are plain HTML. To update content:

1. Edit the file directly on GitHub (click the file → pencil icon → edit → commit)
2. Or clone the repo locally, edit, and push

Changes go live automatically within a minute of committing to the `main` branch.

### Common edits

- **Phone number:** Search for `[Your Phone Number]` or `01onal 000 0000` across all files and replace with your actual number
- **Email address:** Currently set to `info@brecklandenergy.co.uk` — update if different
- **Pricing:** Search for `£75`, `£95`, `£120` in `index.html` to adjust service prices
- **Contact form:** The form is currently static HTML. To make it functional, integrate with [Formspree](https://formspree.io) (free tier), [Netlify Forms](https://www.netlify.com/products/forms/), or [Web3Forms](https://web3forms.com)

## Contact Form Setup

The contact form needs a backend to actually send submissions. The simplest free option:

1. Sign up at [formspree.io](https://formspree.io) (free for up to 50 submissions/month)
2. Create a new form and copy your form endpoint (e.g. `https://formspree.io/f/abcd1234`)
3. In `index.html`, find the `<div class="contact-form">` section
4. Wrap the form fields in a `<form>` tag:

```html
<form action="https://formspree.io/f/YOUR_ID" method="POST" class="contact-form">
```

5. Add `name` attributes to each input field (e.g. `name="name"`, `name="email"`, `name="phone"`, `name="postcode"`, `name="service"`, `name="message"`)
6. Change the submit button to `<button type="submit">`

## Folder Structure

```
breckland-energy/
├── index.html        ← Main website
├── privacy.html      ← Privacy Policy
├── terms.html        ← Terms & Conditions
└── README.md         ← This file
```

## License

© 2026 Breckland Energy. All rights reserved.
