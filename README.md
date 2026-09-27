# Cafe Mehfil — Website

A single static page (`index.html`) for Cafe Mehfil, Malvan. No build step —
open it directly in a browser, or host it for free on GitHub Pages / Netlify / Vercel.

## Connecting the live Instagram feed

The exact Instagram handle wasn't provided, so `PUT_HANDLE_HERE` appears twice
in `index.html` as a placeholder (in the Instagram section's link and label).
Once you have it:

1. Go to https://snapwidget.com (or https://elfsight.com / https://lightwidget.com)
   and create a free "Instagram Feed" widget.
2. Enter the Cafe Mehfil Instagram username (account must be public, or
   Business/Creator).
3. Copy the `<iframe>` embed code it gives you.
4. Open `index.html`, find the section commented `AUTO-SYNC INSTAGRAM FEED`,
   and paste the iframe code inside `<div id="insta-live">`, replacing the
   placeholder emoji grid. Also replace both `PUT_HANDLE_HERE` occurrences
   with the real handle.

New posts will then appear on the site automatically — the widget service
polls Instagram on your behalf, nothing else to maintain.

## Editing

- Colors, fonts, and spacing: all in the `<style>` block at the top of `index.html`
  (same palette as the Cheezy Bites site — toast-brown, cheese-gold, brick accent).
- Menu items, reviews, and contact info: plain HTML further down the file —
  search for the matching section (`Menu`, `Reviews`, `Find Us`, etc.).
- Hours aren't on the Google listing yet — if they get added, put them in the
  "Good to Know" list in the Location section.

## Hosting for free

- **GitHub Pages**: create a repo, upload `index.html`, enable Pages in repo settings.
- **Netlify**: drag-and-drop the folder at app.netlify.com/drop.
