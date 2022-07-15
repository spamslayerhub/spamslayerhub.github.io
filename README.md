# SpamSlayerHub

The source code of the [SpamSlayerHub.github.io](https://SpamSlayerHub.github.io) website.

## Developing

| Requirements | Version |
| ------------ | ------- |
| Node.js      | >= 14   |
| NPM          | >= 8    |
| Git          | >= 2    |

Clone the repository

```sh
git clone https://github.com/spamslayerhub/spamslayerhub.github.io
```

CD into it

```sh
cd SpamSlayerHub.github.io
```

Checkout `development`

```sh
git checkout development
```

Install the necessary dependencies

```sh
npm i
```

Check to see if everything worked

```sh
npm run dev
```

## Building

Build the project

```sh
npm run build
```

Serve the project (requires [serve](https://www.npmjs.com/package/serve) / `npm i -g serve`)

```sh
serve build
```
