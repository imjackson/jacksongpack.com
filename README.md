# jacksongpack.com

My personal website / online CV.

## About

This site is built with plain HTML and CSS. Node is used during development for Prettier and pre-commit hooks.

A lot of consideration was taken to make this site as fast and as energy efficient as possible. [Fonts](#fonts) are served locally and preloaded. The fonts used are also subsetted into base Latin characters. Images and markup are kept to a minimum.

## Running Locally

-   Clone the repository: `git clone https://github.com/imjackson/jacksongpack.com.git` or `git clone git@github.com:imjackson/jacksongpack.git` (if using ssh).
-   Install development dependencies with npm: `npm install`
-   Run the site using your preffered live-server app.

Husky and Pretty-Quick are used to run prettier as a pre-commit hook. You can run prettier manually with `npx prettier --write .`.

## Building Site

The `build` script is a simple bash script that copies necessary public files into the `dist/` directory. This avoids serving development files when using a host like Netlify. If a `dist/` folder is already found in the root directory, it is deleted before building. The following files or directories are copied into the `dist/` directory:

-   assets/
-   css/
-   \*.html
-   LICENSE
-   robots.txt

Run the script with: `./build`, or direct your host to run `./build` before deploying and ensure that the public directory is set to `dist/`.

## Development Dependencies

-   Prettier
-   Husky
-   Pretty-Quick

## Fonts

Fonts are served locally from [assets/fonts](./assets/fonts/).

Fonts used:

-   Lato
-   Roboto
-   IBM Plex Sans

## License

This repository is maintained with the [GNU General Public License v3.0](./LICENSE). However the following files or directories are Copyright Jackson Pack, and may not be used without permission:

-   assets/images/
