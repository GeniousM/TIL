# Before Start Project Setting

Client setting options

- react, react-apollo, react-apollo-boost
- GraphQL, GraphQL-tag
- typeScript
- ESlint - TSlint
- Prettier

Serveer setting option

-
- babel

## Client All in One

1. create react app project

```
npx create-react-app projectName --typescript
or
yarn create react-app projectName --typescript
```

1. install settings
   - graphql
   - apollo
   - ant design

```
npm i --save react-router-dom apollo-boost react-apollo react-apollo-hooks graphql-tag graphql
or
yarn add react-router-dom apollo-boost react-apollo react-apollo-hooks graphql-tag graphql

yarn add -D @graphql-codegen/cli

yarn add antd
```

1. set tslint

```
yarn add --dev tslint-config-airbnb
```

1. only Prettier
   1. install Prettier
   ```
   - npm install --save-dev eslint-plugin-prettier
   - npm install --save-dev --save-exact prettier
   ```
   1. Configuration

1) React + typeScript + TSLint
   1. create react-app and typescript project
   ```
   npx create-react-app typescript-react-app --scripts-version=react-scripts-ts
   ```
   1. set tslint at project
   ```
   yarn add --dev tslint-config-airbnb
   ```
