# Gatsby Pages

![GitHub repo size](https://img.shields.io/github/repo-size/maxsonyang/gatsby-pages?color=%2300a6ff)

Pre-configured Gatsby project that's ready to deploy to gh-pages because I've had to do this too many times already.

## Comes with

* gh-pages
* Sass
* ESLint configured with AirBnB and Prettier configuration [credits](https://medium.com/@joshuacrass/javascript-linting-and-formatting-with-eslint-prettier-and-airbnb-30eb746db862)
* some random media queries


## Usage

These commands are are all run from the project root:

### Install Node Packages

```shell
npm i
```

### Start the development server

```shell
npm start
```

### Deployment

#### package.json configuration

You'll want to change some of the metadata in the package.json, namely:
- name
- description
- author

#### Deploying to a subdomain

Specifically, this is if you're deploying to a url that follows the pattern:
`your-gh-username.github.io/*`.

If this is the case, you'll need to specify the subdomain by updating the `pathPrefix`
in `gatsby-config.js`.

#### Publishing to Github Pages

To deploy, you can run the following command:
```shell
npm run deploy
```

_note: you'll need to have a branch already set up if you're not deploying to your gh-pages branch_

[Gatsby Docs Here](https://www.gatsbyjs.com/docs/how-to/previews-deploys-hosting/how-gatsby-works-with-github-pages/)