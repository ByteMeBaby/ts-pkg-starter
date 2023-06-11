Hey there 👋. I created this simple template for my own projects. Decided to make it public thinking this would be helpful for others too. Feel free to use it.

## How to use this template

1. Install dependencies by running `pnpm install` (Or you can use yarn or npm. Make sure to delete pnpm-lock.yaml file if you are not using pnpm).
2. Open package.json change name, version, homepage, author, keywords, description, repository, bugs, homepage, license, etc.
3. Change readme file.
4. Delete CHANGELOG.md
5. Change LICENSE file and license fild in package.json file.
6. This file uses changesets for versioning. If you don't want to use it, delete `version` script from package.json file and delete `.changeset` folder. More info can be found [here.](https://github.com/changesets/changesets/tree/main)
7. Rename github folder to .github
8. Update .github/workflows/publish.yml and .github/workflows/tests.yml file with your own details.
9. Delete .changeset folder.
10. delete CHANGELOG.md file.

## Steps to publish

**Note**: Please make sure you have granted required permissions for the github actions to create PR and publish the package to NPM.

1. Make changes.
2. Commit your changes
3. Run `pnpm changeset` and follow the instructions.
4. Commit changeset file.
5. Push your changes to github.
6. Github actions will run and create a PR to publish your package.
7. Merge the PR and your package will be published to npm.

## Scripts

- `lint`: Run typescript as a linter.
- `build`: Build and bundle the project to ./dist using tsup.
- `test`: Run tests using vitest in watch mode.
- `test:ci`: Run tests using vitest in CI mode.
- `build:ci`: Build and bundle the project to ./dist using tsup in CI mode.
- `release:ci`: Release a new version using changesets in CI mode.

## Note

I have published a demo package using this template. You can find it [here](https://www.npmjs.com/package/@bytemebaby/demo-ts-pkg-starter)
