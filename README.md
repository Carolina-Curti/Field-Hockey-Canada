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

