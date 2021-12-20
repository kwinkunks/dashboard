# Maintainer dashboard

This is a status board for repositories in the 'subsurface stack'. It is a fork of the [maintainer.io dashboard](https://github.com/mntnr/dashboard), which was a fork of [ipfs/project-repos](https://github.com/ipfs/project-repos).


## Install

Simply clone this repo.


## Usage

### Local development

Get a GitHub personal access token with `public-repo` permission and create `secret.json` with content like:

    {"token": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"}

To start:

    npm i
    npm run build

To recompile continuously, and start a development server with hot reloading:

    npm run serve-watch

### Enterprise

Add a `rootURL` field to `data.json` with the endpoint needed.


## Deploy

To deploy this, after merging any new PRs, follow these steps:

2. Kill your `npm run dev` script if you happen to have it running.
3. `npm install && npm prune`
4. `npm run publish`. This should open the published page on the gateway.


## Contribute

If you would like to contribute code to this repository, please dive in! Check out [the issues](//github.com/kwinkunks/dashboard/issues).


## License

[MIT](LICENSE)
