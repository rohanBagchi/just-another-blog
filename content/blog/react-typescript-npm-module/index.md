---
title: React + Typescript NPM module. An Introduction
date: "2020-07-26"
description: This is an introduction to our journey into building a React + TypeScript + Storybook NPM Module. We will cover building a vanilla JavaScript function and making it ready for publishing, then we will add react + storybook and publish a v2. Finally bring in Typescript.
published: false
---

Welcome to the series.

We will start with a problem statement, followed by a plan on how we aim to solve it.

#### So the problem statement

We want to create a reusable React component with Typescript and be able to publish it to NPM.

#### Our solution plan

1. Create a simple multiplier function in JavaScript. Let's call it `AwesomeMultiplier.js`
2. Add a simple jest test to verify it works
3. Convert it to TypeScript. Add dependencies, `tsconfig.json` & rename `AwesomeMultiplier.js` -> `AwesomeMultiplier.ts`
4. Prepare for build and release to an NPM registry
5. Install [Verdaccio](https://verdaccio.org/). This is done so that you can test your releases locally without ever publishing to npmjs. Once you are confident, it is only a matter of switching to `npmjs` as a registry.
6. Publish to Verdaccio
7. Create a test node project and install the `AwesomeMultiplier` npm package from our local Verdaccio instance and verify it works.
8. Add React to the `tsconfig.json` and create our React component. Let's call it `Multiplier.tsx`. It's job is to accept two numbers as props and show their product.
9. Add [storybook](https://storybook.js.org/) to behave as a demo / kitchensink for our component library.
10. Add a story for `Multiplier.tsx` component
11. Add `npm scripts` for the following:
    1. Running storybook locally
    2. Creating a releasable static build of the storybook
    3. Creating a releasable build for `Multiplier.tsx`
12. Build and publish our storybook to Netlify
13. Build and publish our `Multiplier.tsx` to Verdaccio
14. Create a simple react app, install from Verdaccio and verify it all works as expected
15. Publish to `npmjs` under your name under your namespace.

#### Tentative tutorial split

1. `Part 1`: will cover step 1 to step 7.
2. `Part 2`: will cover from step 7 to step 11.
3. `Part 3`: will cover from step 12 to step 15.
