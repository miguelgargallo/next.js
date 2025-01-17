## Example app using Google Analytics and Google Tag Manager

This example shows how to use Next.js along with Google Tag Manager. [`pages/_document.js`](pages/_document.js) is used to inject [base code](https://developers.google.com/tag-manager/quickstart). [`pages/_app.js`](pages/_app.js) is used to track route changes and send page views to Google Tag Manager, along with [Google Analytics](https://developers.google.com/analytics/devguides/collection/gtagjs/). A custom [\_app](https://nextjs.org/docs/advanced-features/custom-app) is used to inject [tracking snippet](https://developers.google.com/analytics/devguides/collection/gtagjs/) and track [pageviews](https://developers.google.com/analytics/devguides/collection/gtagjs/pages) and [event](https://developers.google.com/analytics/devguides/collection/gtagjs/events).

## Deploy your own

Deploy the example using [Vercel](https://vercel.com?utm_source=github&utm_medium=readme&utm_campaign=next-example):

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/git/external?repository-url=https://github.com/vercel/next.js/tree/canary/examples/with-google-tag-manager&project-name=with-google-tag-manager&repository-name=with-google-tag-manager)

## How to use

Execute [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app) with [npm](https://docs.npmjs.com/cli/init), [Yarn](https://yarnpkg.com/lang/en/docs/cli/create/), or [pnpm](https://pnpm.io) to bootstrap the example:

```bash
npx create-next-app --example with-google-tag-manager with-google-tag-manager-app
```

```bash
yarn create next-app --example with-google-tag-manager with-google-tag-manager-app
```

```bash
pnpm create next-app --example with-google-tag-manager with-google-tag-manager-app
```

Next, copy the `.env.local.example` file in this directory to `.env.local` (which will be ignored by Git):

```bash
cp .env.local.example .env.local
```

Set the `NEXT_PUBLIC_GOOGLE_TAG_MANAGER_ID` variable in `.env.local` to match your Google Tag Manager ID.

Deploy it to the cloud with [Vercel](https://vercel.com/new?utm_source=github&utm_medium=readme&utm_campaign=next-example) ([Documentation](https://nextjs.org/docs/deployment)).
