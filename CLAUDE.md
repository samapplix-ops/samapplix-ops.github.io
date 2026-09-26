# samapplix-ops.github.io

The SamApplix website: the four apps, the privacy policy and the terms. GitHub Pages serves it from
`main` at https://samapplix-ops.github.io/. Plain HTML and CSS - no build step, no framework, and
nothing to install.

It replaced two Google Sites pages on 26 September 2026: `sites.google.com/site/samapplix/`, which
still showed Baby Animal and FB Photo Backup, and `sites.google.com/view/samapplix-privacy-policy/`.

## Two addresses Play depends on

- **`privacy.html` is the privacy policy registered in Play Console for all four apps**, and an app
  for children must have one that answers. Never rename it or move it.
- The site root is the "Website" of the four store listings.

## The privacy policy is the author's legal text

`privacy.html` and `terms.html` are the Google Sites text word for word, only split in two. They
change when an app changes what it does, and two such changes are already known:

- the policy says nothing about advertising, which BabyAnimal and MemoryAnimal still carry, and
  CarSoundKids too until its 3.0 is live;
- FirstWords version 6 is planned to record the family's voice (`RECORD_AUDIO`), which needs a
  paragraph of its own.

A changed policy should say when it changed.

## Kept on purpose

- **Nothing is loaded from anywhere else.** No cookies, no analytics, and the two typefaces -
  Fraunces and Nunito, SIL Open Font License, licences beside them in `fonts/` - are served from
  here rather than from Google Fonts, so no visitor's address goes to a third party.
- **English by default, Italian for a browser set to Italian**, and a button that swaps the two. The
  Italian is the `IT` table at the foot of `index.html`; an element carries `data-t` to be
  translated, an image `data-it-src` and `data-it-alt`. The choice is stored only when it is made by
  hand. The legal pages are English only.
- **The icons are the ones Play shows**, downloaded from Play at 256 px, and the two phones are the
  FirstWords store screenshots `store/screenshots/<lang>/03-learn.jpg` and `04-play.jpg`, scaled to
  540 wide with ffmpeg. A draft made elsewhere used generated pictures for both; that is what this
  page exists to not do, for apps sold on real photographs.
- **Every Play link carries `referrer=utm_source%3Dsamapplix_site%26utm_medium%3Dwebsite`**, so an
  arrival from here shows in Play Console as a third-party referrer, beside the strip in the three
  sister apps.
- **No ratings, no download counts, no ages.** They change, they differ by country, and Play shows
  the real ones one tap away. Each app's line is its Play short description, in English and Italian.
- **Commits use `samapplix@gmail.com`.** This repository is public, and the address a commit carries
  is visible to anyone.
