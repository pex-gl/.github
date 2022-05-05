# Contribution Guide

Hi, thanks for considering helping!

## Development environment and styleguide for JavaScript projects

Packages are developed using [Snowdev](https://github.com/dmnsgn/snowdev/):

- `npx snowdev init`: Create simple package structure.
- `npx snowdev dev`: Start dev server and install ESM dependencies.
- `npx snowdev build`: Lint and Format sources, run TypeScript, update README API.
- `npx snowdev release`: Bump the version, generate changelog release, create a new commit with git tag.
- `npx snowdev install`: Install ESM dependencies.

They're scaffolded from a [template structure](https://github.com/dmnsgn/snowdev/tree/main/template) and [Snowdev](https://github.com/dmnsgn/snowdev/) enforces some conventions:

- code formatting using [Prettier 2](https://prettier.io/) defaults
- code linting using [ESLint](https://eslint.org/) with a basic configuration for compatibility with [Babel](http://babeljs.io/), [Prettier](https://prettier.io/) and [TypeScript](https://www.typescriptlang.org/). See [snowdev default config](https://github.com/dmnsgn/snowdev/blob/9cf45263b00a8c851c9d635287a7f6549d69b9c8/index.js#L56-L99)
- code comes with type definitions generated using [TypeScript](https://www.typescriptlang.org/) and extrapolated from [JSDoc definitions](https://jsdoc.app/) in JS-only projects
- commit messages follow the [Conventional Commits specification](https://www.conventionalcommits.org/en/v1.0.0/) and the [Angular preset](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines) to generate changelogs and facilitate commit search.

The below comes from [sindresorhus](https://github.com/sindresorhus/.github/blob/main/contributing.md) who sets the best ground rules for contributing.

Be nice and respect the maintainers' time. ❤️

Please read this whole thing. Most of this applies to any repo on GitHub. 🙏

## Contribute

Code is not the only thing you can contribute. I truly appreciate contributions in the form of:

- Fixing typos.
- Improving docs.
- Triaging [issues](https://github.com/search?o=desc&q=user:pex-gl+is:issue+is:open&s=updated&type=Issues).
- Reviewing [pull requests](https://github.com/search?o=desc&q=user:pex-gl+is:pr+is:open&s=updated&type=Issues).
- Sharing your opinion on issues.

## Issues

- Before opening a new issue, look for existing issues (even closed ones).
- [Don't needlessly bump issues.](https://blog.sindresorhus.com/issue-bumping-e3b9740e2a0)
- If you're reporting a bug, include as much information as possible. Ideally, include a test case that reproduces the bug. For example, a [Runkit](https://runkit.com) or [repl.it](https://repl.it) playground. Even better, submit a pull request with a [failing test](https://github.com/avajs/ava/blob/master/docs/01-writing-tests.md#failing-tests).

## Pull requests

### Prerequisite

- If the changes are large or breaking, open an issue discussing it first.
- Don't open a pull request if you don't plan to see it through. Maintainers waste a lot of time giving feedback on pull requests that eventually go stale.
- Don't do unrelated changes.
- Adhere to the existing code style.
- If relevant, add tests, check for typos, and add docs and types.
- Don't add editor-specific metafiles. Those should be added to your own [global gitignore](https://gist.github.com/subfuzion/db7f57fff2fb6998a16c).
- Don't be sloppy. I expect you to do your best.
- Squash your local commits into one commit before submitting the pull request, unless you have important atomic commits.
- Double-check your contribution by going over the diff of your changes before submitting a pull request. It's a good way to catch bugs/typos and find ways to improve the code.
- Do the pull request from a new branch. Never the default branch (`main`/`master`).

### Submission

- Give the pull request a clear title and description. It's up to you to convince the maintainers why your changes should be merged.
- If the pull request fixes an issue, reference it in the pull request description using the syntax `Fixes #123`.
- Make sure the “Allow edits from maintainers” checkbox is checked. That way I can make certain minor changes myself, allowing your pull request to be merged sooner.

### Review

- Push new commits when doing changes to the pull request. Don't squash as it makes it hard to see what changed since the last review. I will squash when merging.
- It's better to present solutions than asking questions.
- Review the pull request diff after each new commit. It's better that you catch mistakes early than the maintainers pointing it out and having to go back and forth.
- Be patient. Maintainers often have a lot of pull requests to review. Feel free to bump the pull request if you haven't received a reply in a couple of weeks.
- And most importantly, have fun! 👌🎉

Thanks, Damien Seguin.
