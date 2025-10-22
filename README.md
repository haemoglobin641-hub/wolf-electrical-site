# Wolf Electrical Bournemouth — Static Website

This is a simple, zero-cost website suitable for **GitHub Pages** or **Netlify** hosting.

## Structure
```
wolf-electrical-site/
├── index.html
├── css/
│   └── styles.css
├── assets/
│   └── logo.png
└── js/
```
> Add more pages later by creating new `.html` files and linking them in the header nav.

## Edit Text
Open `index.html` and change the copy inside each `<section>`:
- **Hero** (business name, services, buttons)
- **About** (company summary, bullet points)
- **Services** (cards you can add/remove)
- **Certifications** (NICEIC etc.)
- **Contact** (service area, phone, email, WhatsApp)

## Update Services
Duplicate a service `<article class="card">` block in the **Services** section.
Change the `<h3>` and `<p>` to suit.

## Colours & Style
Colours are defined in `css/styles.css` under the `:root{}` CSS variables:
```css
:root{
  --brand:#10a3f0; /* primary blue */
  --accent:#0ea5e9;
  --text:#0f172a;
}
```
Adjust these values to change the theme. Typography uses system fonts for speed and zero cost.

## Logo
Replace `assets/logo.png` with your preferred logo file using the same name.
For a favicon, reuse the same file or add a dedicated `favicon.ico` and update the `<link rel="icon">` in `index.html`.

## Contact Buttons
- **Call:** change the `href="tel:..."`
- **Email:** change `mailto:...`
- **WhatsApp:** update to `https://wa.me/<countrycode+number>`

## Free Hosting

### Option A — GitHub Pages (recommended, fast)
1. Create a new repository on GitHub called `wolf-electrical-site`.
2. Upload the contents of this folder (or drag‑and‑drop the ZIP).
3. Go to **Settings → Pages**.
4. Under *Build and deployment*, set **Source** = *Deploy from a branch*.
5. Choose **Branch** = `main` and **Folder** = `/ (root)`. Save.
6. After a minute, your site will be live at `https://<your-username>.github.io/wolf-electrical-site/`.

### Option B — Netlify (drag‑and‑drop)
1. Create a free Netlify account.
2. Drag the **`wolf-electrical-site`** folder (or ZIP) onto the Netlify dashboard.
3. Netlify gives you a live URL immediately; rename it in **Site settings → Domain management**.

## Mobile & Performance
- Mobile menu appears at small widths (☰ button).
- Layout is responsive using CSS Grid & fluid type.
- No external libraries: fast, free, and simple.

## Custom Domain (optional, still free to host)
- Buy a domain from a registrar.
- Point the domain to GitHub Pages or Netlify following their docs (uses DNS CNAME/A records).

---

Need more sections (gallery, FAQs, testimonials), or a second page (e.g., pricing)? Create another HTML file and copy the header/footer.
