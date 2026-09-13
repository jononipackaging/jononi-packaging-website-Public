# Jononi Packaging — Website

A single-page site (`index.html` + an `images` folder) with sections: Home, Products, Gallery, Why Us, Process, About, Contact.
Off-white + sky-blue theme, your logo in the header, a photo gallery of your product line with a soft scroll-reveal animation on the cards, a working contact form (Netlify Forms), and a floating WhatsApp button.

## Folder contents

```
jononi-site/
  index.html
  images/
    logo.jpg                       — header & footer logo
    bag-ldpe-handle-folding.jpg
    bag-nonwoven-dcut.jpg
    bag-nonwoven-swing-food.jpg
    bag-ldpe-dcut-folding.jpg
    bag-nonwoven-swing-box.jpg
    bag-nonwoven-loop-handle.jpg
```
Keep `index.html` and the `images` folder together — the page loads images using relative paths like `images/logo.jpg`.

## Deploy to Netlify (no domain needed)

**Fastest way — drag and drop:**
1. Go to https://app.netlify.com/drop
2. Drag the whole `jononi-site` folder onto the page.
3. Netlify gives you a free address like `random-name-123.netlify.app` immediately.
4. In **Site settings → Change site name**, rename it to something like `jononi-packaging.netlify.app`.

**Recommended way — connect GitHub (auto-redeploys on every change):**
1. Push this folder to a new GitHub repository.
2. In Netlify: **Add new site → Import an existing project → GitHub** → select the repo.
3. Leave the build command empty and set the publish directory to `/` (root).
4. Deploy — every future push updates the live site automatically.

## What's already filled in

- **Contact**: phone/WhatsApp `+880 1830-593672`, email `jononipackaging@gmail.com`
- **Address & map**: pulled from the Google Maps link you shared (Hwk Place, Madani City Rd, Kalibandor 3100) — double-check the embedded map pin looks right once it's live, since it was matched from the link's place name.
- **Office hours**: Sat–Thu, 9:00 AM – 6:00 PM
- **Gallery**: your six product photos, in a card grid that fades in as visitors scroll to it

## What's still a placeholder — update before going live

In the **About** section of `index.html`, replace these two lines with your real content:
- `[Add your company's founding story, facility details and capacity figures here.]`
- `[Add certifications, major clients or export markets here, if applicable.]`

## The contact form

`data-netlify="true"` and the hidden `form-name` field are already in place, so Netlify auto-detects the form once the site is deployed — no backend needed. Submissions appear under **Site → Forms** in your Netlify dashboard, where you can also turn on email notifications.

## Adding a custom domain later

You can add one anytime from **Site settings → Domain management → Add a custom domain** — no need to redeploy the site first.
