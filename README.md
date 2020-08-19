# botch-lambda

This is an optional tool that helps with building or locally developing [Netlify Functions](https://www.netlify.com/docs/functions/?utm_source=github&utm_medium=swyx-netlify-lambda&utm_campaign=devex) with a simple webpack/babel build step. For function folders, there is also a small utility to install function folder dependencies.

The goal is to make it easy to write Lambda's with transpiled JS/TypeScript features and imported modules.

<details>
  <summary><b>Multiple ways to deploy functions on Netlify</b></summary>

as of [CLI v2.7](https://www.netlify.com/docs/cli/#unbundled-javascript-function-deploys?utm_source=github&utm_medium=swyx-netlify-lambda&utm_campaign=devex), a non-bundled, non-zipped, folder of files.

`Netlify-Lambda` uses webpack to bundle up your functions and their dependencies for you, suiting the first approach. However, if you have native node modules (or other dependencies that don't expect to be bundled like [the Firebase SDK](https://github.com/netlify/netlify-lambda/issues/112)) then you may want to try the other approaches. In particular, try [`Netlify Dev`](https://www.netlify.com/docs/cli/?utm_source=github&utm_medium=swyx-jamstack&utm_campaign=devex#netlify-dev-beta).

If this sounds confusing, support is available through [our regular channels](https://www.netlify.com/support/?utm_source=github&utm_medium=swyx-netlify-lambda&utm_campaign=devex).

</details>

## Installation

**recommend installing locally** rather than globally:

```bash
npm install netlify-lambda
```
