# Frontend-Project-Tips

List some tips that how to make a good frontend project according to my experiences in the past few years.

## Structure

### UI

- basic styles (contains fonts, element styles, color styles...)
- basic UI components (images, buttons, texts, panels, swipers, loadings, indicators, table-cells...)

### Folders

Just for your reference, you can always get benefits from splitting the whole business into several modules.

```
└── src
    ├── components
    ├── moduleA
    │   ├── components
    │   ├── pages
    │   ├── services
    │   └── ...
    ├── moduleB
    │   ├── components
    │   ├── pages
    │   ├── services
    │   └── ...
    ├── pages
    ├── services
    └── ...
```

### Logics

- use custom hooks to wrap some of the logics to make the logics clear and clean.
- distinguish the common logics from the business ones, and make the common logics testable.
- handle business logics with functions which has definite inputs and outputs so that they can be covered by tests and unlikely to become unexpected.

## Tools

###  Environment

- cross-env
- dotenv / dotenv-flow (for multiple env files, e.g .env.development, .env.development.local, .env.production)

### CSS

- CSS-Modules
- CSS-in-JS

### Statement Management

- Redux
- Redux-Toolkit (highly recommended if you are using Redux)
- Mobx

### Request

- axios
- React-Query
- Redux-Toolkit-Query (aka rtk-query)
- Apollo-GraphQL

### Code Style Check

- eslint
  - eslint-plugin-unicorn
  - eslint-plugin-promise
  - eslint-plugin-sonarjs
- stylelint
- prettier
- commitlint

### Code Quality Check

- sonarQube
- sonarLint

### Unit & E2E Test

- jest
- testing-library
- cypress

### Hooks

- husky
- lint-staged

### CI/CD

- Docker
- TravisCI
- CircleCI 
- Jenkins
- Github Actions / GitLab CI
- Bamboo
- aws-cli 

### Chore

- npm version (automatically update package.json version and add git tags)
- standard-version / conventional-changelog-cli (automatically generate changelogs)
