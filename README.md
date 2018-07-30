# cli-guides-app

This repository is part of a Work-In-Progress project to refresh the CLI guides content that currently lives at [https://ember-cli.com](ember-cli.com). The CLI Guides App is the structure for the [cli-guides-source](https://github.com/ember-learn/cli-guides-source) markdown files.

As this project is pre-1.0, no content should be taken as the final word. Additional review is still pending.

Do you know a thing or two about the CLI or addons? We'd love to have your help with writing! Do you _wish_ you knew a thing or do? You could help us review to make sure that content is helpful to all knowledge levels. Please drop by the #-team-learning channel on the [Ember Community Slack](https://ember-community-slackin.herokuapp.com/) and `@` one of the [main contributors](https://github.com/ember-learn/cli-guides-app/graphs/contributors) to get more information.

## Prerequisites

You will need the following things properly installed on your computer.

* [Git](https://git-scm.com/)
* [Node.js](https://nodejs.org/) (with npm)
* [Ember CLI](https://ember-cli.com/)
* [Google Chrome](https://google.com/chrome/)

## Installation

* `git clone <repository-url>` this repository
* `cd cli-guides-app`
* `npm install`

This will display the content of the deployed Guides markdown

## Local Development

To see what a local copy of the Guides markdown looks like:

* Clone the [Ember CLI Guides](https://github.com/ember-learn/cli-guides-source) Source repository
* link the `ember-cli-guides-source` repository by running `npm link` inside that repo, then `npm link @ember-learn/cli-guides`
* `ember serve`
* Visit your app at [http://localhost:4200](http://localhost:4200).
* Visit your tests at [http://localhost:4200/tests](http://localhost:4200/tests).

### Adding more things to the table of contents

See `pages.yaml` in the cli-guides-source. Whatever has a url of index will be what is shown for the top level path, like `/tutorial/`. There must be an `index.md` under each topic. 

### Running Tests

* `ember test`
* `ember test --server`

### Linting

* `npm run lint:js`
* `npm run lint:js -- --fix`

### Building

* `ember build` (development)
* `ember build --environment production` (production)

### Deploying

- Clone the [cli-guides-source](https://github.com/ember-learn/cli-guides-source) to your computer
- From within the guides-source repo, do `np` or `npm run release`. You must have valid npm credentials to do this. Choose a `patch` release.
- From within this cli-guides-app repository, do `npm install @ember-learn/cli-guides@latest`
- `git diff` to see that the package number has been updated to whatever `np` produced.
- commit the changes and push to `master` of the cli-guides-app respository


## Further Reading / Useful Links

* [ember.js](https://emberjs.com/)
* [ember-cli](https://ember-cli.com/)
* Development Browser Extensions
  * [ember inspector for chrome](https://chrome.google.com/webstore/detail/ember-inspector/bmdblncegkenkacieihfhpjfppoconhi)
  * [ember inspector for firefox](https://addons.mozilla.org/en-US/firefox/addon/ember-inspector/)
