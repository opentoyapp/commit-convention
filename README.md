# Commit Convention Auto-Install Toolkit

I got tired of manually installing `husky`, `commitlint`, `commitizen`, etc. with `npm i -D blah blah ...` every time I set up a new project, so I created this module.

## Usage

You can use it as follows:

```bash
npx create-commit-convention   # npm
yarn create commit-convention  # yarn
pnpm create commit-convention  # pnpm
```

When you run the above command, the following files will be created in your project:

- `.cz-config.js`
- `commitlint.config.js`
- `.husky` directory
- `commit-msg` and `prepare-commit-msg` files under the `.husky` directory

Additionally, a `prepare` script will be added to the `scripts` section of your `package.json`, and commitizen-related configurations will be added to the `config` field.

If there is no `.git` directory in your project, it will automatically run `git init`.
