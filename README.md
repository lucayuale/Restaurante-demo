# Alba & Olive — Restaurant Booking Demo

> **A VYB web design concept** · Fictional restaurant · Booking interface preview

**Alba & Olive** is a fictional, Italian-inspired restaurant website designed and developed by **VYB**. This repository demonstrates a warm, editorial web experience for hospitality businesses, with a restaurant menu, photography, and a prepared online-reservation interface.

> **Important:** This is a portfolio demonstration, not a real restaurant. The address, opening hours, menu and prices are illustrative. **Online table reservations are not connected**, and clicking a booking button will not create a reservation.

## Features

- **Seven real pages:** Home, Story, Menu, Experience, Gallery, Booking and Visit.
- **English and Spanish** with a language switcher.
- **Responsive design** for desktop and mobile.
- Sample food menu with four categories and eight bilingual dishes.
- Local restaurant photography stored in `assets/`.
- Gallery with image lightbox and accessible navigation.
- Booking call-to-action components, ready for a future restaurant-owned booking service.
- Static hosting: no backend, database or installation needed to view the demo.

## Technology

Plain **HTML, CSS and JavaScript**. Google Fonts are loaded over the internet; the restaurant photographs are included in this repository. The demo works as a static website and is compatible with GitHub Pages.

## Folder structure

```text
index.html              Homepage
story.html              Brand story
services.html           Food and drinks menu
experience.html         Restaurant atmosphere
gallery.html            Photo gallery
booking.html            Booking preview
visit.html              Location and illustrative hours
config.js               Content, translations and site configuration
app.js                  Page behavior, language switch, navigation
styles.css              Responsive styles
assets/                 Local images and favicon
.nojekyll               GitHub Pages static-site setting
README.md               This guide
COMO_PUBLICAR.txt       Spanish publishing instructions
```

**Do not upload only `index.html`:** upload every HTML page, JavaScript, CSS and the entire `assets/` directory. The files are already arranged for deployment at the root of a GitHub repository.

## Run locally

Download or clone the repository, then start a local web server in its root:

```bash
python -m http.server 8080
```

Open `http://localhost:8080`. If Python is installed as `py` on Windows, use `py -m http.server 8080` instead.

## Publish with GitHub Pages

1. Create a GitHub repository that you own or can administer.
2. Upload **the contents of this folder** to the repository root. Keep `assets/` as a folder.
3. Open **Settings → Pages**.
4. Set **Source: Deploy from a branch**, **Branch: main**, **Folder: /(root)**. Save.
5. In **Actions**, wait for the Pages deployment to complete successfully.
6. Use the **Visit site** link shown in Settings → Pages to check the site.

All paths are relative, so the pages and images work under a GitHub Pages project URL such as `username.github.io/repository-name/`. No URL is assumed or hardcoded in this repository.

## Booking integration

The demo keeps the **Booking** design and related calls to action, but intentionally has no active booking URL:

```js
// config.js
"booking": {
  "mode": "modal",
  "url": ""
}
```

With a blank URL, clicking a booking button displays a clear notice instead of sending anyone to another demo's calendar. **No Obsidian Setmore account is used.**

For a real client, set up a booking platform owned and configured by that restaurant. Then add its HTTPS booking URL after validating the integration, reservation confirmation, available capacity and cancellation behavior. An appointment calendar alone does not necessarily manage table availability, party sizes or restaurant capacity.

## Content and privacy

- This is a demonstration of design and structure, **not a live business**.
- Displayed menu, prices, opening hours and location details are examples.
- No real customer contact or booking information is stored by this static demo.
- Do not add private credentials, booking API secrets, customer records or unpublished business information to a public repository.
- Before reuse for a real restaurant, replace illustrative content and confirm image licenses/usage permissions.

## Español

Esta es una **demo de restaurante ficticio creada por VYB**, con **siete páginas independientes**, menú bilingüe, galería, diseño adaptable y presentación de reservas. Las reservas **no están conectadas**: los botones no generan turnos ni reservas de mesas. Para publicarla, subí todos los archivos y la carpeta `assets` a la raíz del repositorio, y activá **Settings → Pages → Deploy from a branch → main → /(root)**. La guía paso a paso está en `COMO_PUBLICAR.txt`.

---

**VYB — Website Design & Development** · Portfolio demonstration
