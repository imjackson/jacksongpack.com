# jacksongpack.com

My personal website / online CV.

## About

This site is built with plain HTML and CSS. Node is used during development for Prettier and pre-commit hooks.

A lot of consideration was taken to make this site as fast and as energy efficient as possible. Fonts are served locally and preloaded. The fonts used are also subsetted into base Latin characters. Images and markup are kept to a minimum.

## Running Locally

-   Clone the repository: `git clone https://github.com/imjackson/jacksongpack.com.git`
-   Install development dependencies with npm: `npm install`
-   Run the site using your preffered live-server app.

Husky and Pretty-Quick are used to run prettier as a pre-commit hook. You can run prettier manually with `npx prettier --write`.

## Development Dependencies

-   Prettier
-   Husky
-   Pretty-Quick

## License

This repository is maintained with the [GNU General Public License v3.0](./LICENSE). However the following files or directories are Copyright Jackson Pack, and may not be used without permission:

-   assets/images/
