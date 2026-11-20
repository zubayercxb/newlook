# Newlook

Node.js project. Environment variables are loaded with [dotenv](https://github.com/motdotla/dotenv).

## Requirements

- Node.js 12 or newer (`dotenv` requires `node >= 12`)
- npm

## Setup

```bash
npm install
```

Put local configuration in a `.env` file at the project root. Do not commit that file.

The package uses CommonJS (`"type": "commonjs"`). `package.json` points `"main"` at `index.js`. That file is not in the repo yet.

## Scripts

```bash
npm test
```

`npm test` is still the npm placeholder and exits with an error until tests are added.

## License

ISC
