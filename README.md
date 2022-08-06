# [jacksongpack.com](https://jacksongpack.com)

My personal website / online CV.
([Site Status](https://stats.uptimerobot.com/nXRK6cXKKP))

## About

This site is built with plain HTML and CSS, and is hosted on
[Netlify](https://netlify.com). Node is used during development to run Prettier
as a pre-commit hook.

Consideration was taken to make this site as fast and as
[energy efficient](https://websitecarbon.com) as possible. [Fonts](#fonts) are
served locally and preloaded. The fonts used are subsetted into base Latin
characters. Images and markup are kept to a minimum.

## Running Locally

- Clone the repository:

```bash
git clone https://github.com/imjackson/jacksongpack.com.git
```

or

```bash
git clone git@github.com:imjackson/jacksongpack.com.git # if using ssh
```

- Install development dependencies with npm: `npm install`
- Run the site using your preferred live-server app.

Husky and Pretty-Quick are used to run Prettier as a pre-commit hook; meaning
your code will be formatted each time you make a commit. You can run prettier
manually with `npm run lint:write`.

## Building Site

The `build` script is a simple bash script that copies necessary public files
into the `dist/` directory. This avoids serving development files when using a
host like Netlify. If a `dist/` folder is already found in the root directory,
it is deleted before building. The following files or directories are copied
into the `dist/` directory:

- `assets/`
- `css/`
- `\*.html`
- `LICENSE`
- `robots.txt`

The `build` script will also inject a line into the `robots.txt` file which
points to the sitemap location (`/sitemap.xml`). A sitemap is not included in
this repo, as it is created at build time with
[netlify-plugin-sitemap](https://github.com/netlify-labs/netlify-plugin-sitemap).

Run the script with: `npm run build`, or direct your host to run `npm run build`
before deploying and ensure that the public directory is set to `dist/`.

## Development Dependencies

- [Prettier](https://github.com/prettier/prettier)
- [Husky](https://github.com/typicode/husky)
- [Pretty-Quick](https://github.com/azz/pretty-quick)

## Fonts

Fonts are served locally from [assets/fonts](./assets/fonts/).

Fonts used:

- [Lato](https://www.latofonts.com/)
- [Roboto](https://fonts.google.com/specimen/Roboto?preview.text_type=custom#about)
- [IBM Plex Sans](https://www.ibm.com/plex/)

## License

This repository is maintained with the
[GNU General Public License v3.0](./LICENSE) (where applicable). However the
following files or directories are Copyright Jackson Pack, and may not be used
without permission:

- assets/images/
