<<<<<<< HEAD
# Field Hockey Canada Masters – Mini Site

A tiny, static React site (no build step) you can deploy on Netlify.

It supports:

- Announcements (create/delete in Admin mode)
- Photo gallery (add via image URLs)
- Event links for PACC and WMH World Cup (edit in Admin mode)
- Settings for title/subtitle/socials (saved locally)

## Deploy to Netlify

1. Create a new site on Netlify and connect this GitHub repo.
2. **Build command:** (leave empty)
3. **Publish directory:** `.` (dot = repo root)

## Admin Mode

- Toggle **Admin: ON** (top-right) to add announcements/photos or edit event links.
- Data saves to your browser’s localStorage.
- Click **Reset** to restore defaults.

## Official Links

- PACC Info: https://fieldhockey.ca/masters-pan-american-championship-expression-of-interest/
- PACC Registration (Ramp): http://fhcmast.rampregistrations.com/
- World Cup Info: https://worldmastershockey.org/wmhevents/category/wc/
- World Cup Registration (FHC EOI hub): https://fieldhockey.ca/program/canadian-masters-hockey/
=======
# Field Hockey Canada Masters – Public Mini Site

This repository hosts the static site for **Field Hockey Canada Masters**.  
It provides announcements, photo highlights, and event registration links for the Pan American Championships (PACC) and WMH World Cup.

👉 Live site: [https://fhcmasters.netlify.app](https://fhcmasters.netlify.app)

---

## 🔒 Read-Only Version
- No **Admin toggle**, **Settings**, or **Reset** features.  
- The site is **read-only** for the public.  
- All content is stored in the code (`index.html`) and updated by editing the repository.  
- Visitors cannot add or edit announcements/photos directly.

---

## 📌 Content Structure
All content is inside `index.html` → `<script type="text/babel">` block in the `DEFAULT_DATA` object:

- **Site Info**:  
  - Title, subtitle, logo text  
  - Contact emails (supports multiple addresses)  
  - Social links (Instagram, Facebook, FHC Masters site)  

- **Announcements**:  
  - Stored in `DEFAULT_DATA.announcements` as an array of objects with `id`, `date`, `title`, `body`, `ctaText`, `ctaUrl`, and `tag`.

- **Photos**:  
  - Stored in `DEFAULT_DATA.photos` as objects with `id`, `url`, `caption`, and `credit`.

- **Events & Registration**:  
  - Links for PACC info, PACC registration, World Cup info, World Cup registration, and policies.

---

## 🛠 How to Update Content
1. Open `index.html` in this repository.
2. Scroll to the `DEFAULT_DATA` section:
   ```js
   const DEFAULT_DATA = {
     site: { ... },
     links: { ... },
     announcements: [ ... ],
     photos: [ ... ]
   };

>>>>>>> 8d24a52143696bdad8e0beda56ed044c1b0fe963
