
## Natural Cycles JS Platform

Natural Cycles JS Platform is an opinionated stack of tools that work well together.

## Highlights

- [Architecture choices](#architecture-choices)
- [NPM packages](#npm-packages)
- [CI](#ci)
- [Blessed packages](#blessed-packages)

## Architecture choices

- TypeScript
- prettier
- Jest
- yarn
- CircleCI
- Express.js
- NoSQL

## NPM packages

###### Kick-start a new package

- [generator-nodejs-lib](https://github.com/NaturalCycles/generator-nodejs-lib)
- [generator-backend-service](https://github.com/NaturalCycles/generator-backend-service)

###### devDependencies

- [dev-lib](https://github.com/NaturalCycles/dev-lib)
- [cli](https://github.com/NaturalCycles/cli)
- [semantic-release](https://github.com/NaturalCycles/semantic-release)

###### Universal (Node.js + Browser)

- [js-lib](https://github.com/NaturalCycles/js-lib)
- [time-lib](https://github.com/NaturalCycles/time-lib)

###### Node.js

- [nodejs-lib](https://github.com/NaturalCycles/nodejs-lib)
- [db-lib](https://github.com/NaturalCycles/nodejs-lib)
  - [mongo-lib](https://github.com/NaturalCycles/mongo-lib)
  - [firestore-lib](https://github.com/NaturalCycles/firestore-lib)
  - [datastore-lib](https://github.com/NaturalCycles/datastore-lib)
  - [mysql-lib](https://github.com/NaturalCycles/mysql-lib)
  - [redis-lib](https://github.com/NaturalCycles/redis-lib)
  - [airtable-lib](https://github.com/NaturalCycles/airtable-lib)
  - [spreadsheet-lib](https://github.com/NaturalCycles/spreadsheet-lib)
  - [github-db](https://github.com/NaturalCycles/github-db)
  - sqlite-lib (in progress)
- [fs-lib](https://github.com/NaturalCycles/fs-lib)
- [scrubber-lib](https://github.com/NaturalCycles/scrubber-lib)

###### Frontend

- [frontend-lib](https://github.com/NaturalCycles/nodejs-lib)

###### Backend

- [backend-lib](https://github.com/NaturalCycles/nodejs-lib)

### Experimental

Packages that haven't yet proven their usefullness. API may change without notice.

- [junit-lib](https://github.com/NaturalCycles/junit-lib)
- [json2html](https://github.com/NaturalCycles/json2html)
- [puppeteer-lib](https://github.com/NaturalCycles/yeoman-lib)
- [grafana-lib](https://github.com/NaturalCycles/yeoman-lib)
- [yeoman-lib](https://github.com/NaturalCycles/yeoman-lib)
- [bench-lib](https://github.com/NaturalCycles/bench-lib)
- e2e-lib (todo)

# CI

All packages follow [SemVer](https://semver.org/) (as opposed to [Sentimental versioning](http://sentimentalversioning.org/)) and [Conventional commits](https://www.conventionalcommits.org).

Versions are bumped and released automatically by using [semantic-release](https://github.com/semantic-release/semantic-release).

Current CI of choice is CircleCI, but may be switched to Github Actions in future.

Common CI configuration is abstracted via [orbs](https://github.com/NaturalCycles/orbs).

## Blessed packages

### Already included in libs

- linting / formatting
  - prettier
  - tslint (to be replaced by ESLint)
  - husky
  - lint-staged
- testing
  - jest
  - test-cafe
- cli / tools
  - yargs (alternatives: commander)
  - inquirer (alternatives: enquirer)
  - fs-extra
  - execa
  - globby
  - chalk (alternatives: ansi-colors)
  - dotenv
  - semver
  - lru-cache
  - cheerio
- typescript
  - ts-node
  - tsconfig-paths
- process management
  - nodemon
- validation
  - Joi
- date/time
  - dayjs
  - timekeeper
- data / parsers
  - marked
  - yamljs
  - json5
- http
  - got
  - getGot
  - ky

### Not included in libs

- templating
  - ejs (alternative: nunjucks)
  - bcryptjs
  - node-schedule
  
