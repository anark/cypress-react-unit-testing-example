This is a app generated using @rails/webpacker with react and typescript defaults

It is an attempt to get it working with https://github.com/bahmutov/cypress-react-unit-test so I have added a very basic component test and the loadWebpack config

Currently there are two issue that seem to be blocking this from working.  You see these errors when trying to run the component test `Hello.spec.tsx`

- When you run cypress open you get the following error due to code-coverage not being correctly enabled.
  `Cannot find module '/Users/andrewnarkewicz/Development/example_app/node_modules/get-package-type/index'`

- If you disable code-coverage(setting env.coverage to false in cypress.json and commenting out line 9 of node_modules/cypress-react-unit-test/plugins/load-webpack/index.js) you get the following error when trying to run the spec
  `TypeError: (0 , _schemaUtils.validate) is not a function`

Install dependencies and open cypress with

```
yarn install
yarn cypress open` and selecting
```
