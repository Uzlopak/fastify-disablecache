# Contributing

Contributions are welcome and any help that can be offered is greatly appreciated.
Please take a moment to read the entire contributing guide.

This repository uses the [Feature Branch Workflow](https://atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow),
meaning that development should take place in `feat/` branches, with the `main` branch kept in a stable state.
When you submit pull requests, please make sure to fork from and submit back to `main`.

Other processes and specifications that are in use in this repository are:

-   [Semantic versioning](https://semver.org/)
-   [Conventional commits](https://conventionalcommits.org/en/v1.0.0/) following the @commitlint/config-conventional config
-   [Prettier](https://prettier.io/) style guide

## Getting started

This repository requires that you have [Node.js](https://nodejs.org) >=14.0.0 installed.

With that in place, you can fork the repository, clone it, and then run `npm i` to install all dependencies.

### Development workflow

After cloning the repository and installing all the dependencies, there are several commands available for local development:

-   `npm run lint` - Lints everything in src directory
-   `npm run jest` - Runs Jest over all tests in src directory
-   `npm test` - Runs `npm run lint` and `npm run jest` together

## Documentation style

Documentation (both in markdown files and inline comments) should be written in **British English** where possible.

Titles and headings should use sentence-style capitalisation, where only the first letter of a sentence and proper nouns are capitalised.

## Pull request checklist

Before submitting a pull request back to the main repository, please make sure you have completed the following steps:

1. Pull request base branch is set to `main`. All pull requests should be forked from and merged back to `main`
2. Run `npm test` to check the code adheres to the defined ESLint style and that it passes the Jest tests
3. Run `npm run lint:prettier` to run the Prettier code formatter over the code
4. Run `npm run lint:licenses` if adding or updating production dependencies to check they use permissive licenses

Steps 2. and 4. are automatically run by a pre-commit hook added by [Husky](https://typicode.github.io/husky/#/).

Step 2. is automatically run by a pre-commit hook added by [Husky](https://typicode.github.io/husky/#/).

## Issues

Please file your issues [here](https://github.com/Fdawgs/fastify-disablecache/issues) and try to provide as much information in the template as possible/relevant.
