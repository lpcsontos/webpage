# csontoslp.hu

Source of my portfolio site, served by GitHub Pages at [csontoslp.hu](https://csontoslp.hu).

Plain HTML and CSS, with no build step and no JavaScript. The windows on the page are drawn the way my operating system, [Odin OS](https://github.com/lpcsontos/odin_based_os), draws them.

## Structure

```
index.html             the whole page
assets/css/style.css   styles: desktop layout from 960px up, mobile layout below that
assets/img/            photo, Odin OS screenshots, window close icon
assets/fonts/          self-hosted Press Start 2P, IBM Plex Sans and IBM Plex Mono (SIL Open Font License, see the license files)
CNAME                  custom domain for GitHub Pages
.nojekyll              tells GitHub Pages to serve the files as they are, without Jekyll
```

## Preview locally

```
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Adding the tank photo

Save the photo as `assets/img/tank.jpg`. In the "Arduino tank" window in `index.html`, remove the `<!--` and `-->` around the `<img class="tank-photo">` line and set its `width` and `height` attributes to the photo's size in pixels.
