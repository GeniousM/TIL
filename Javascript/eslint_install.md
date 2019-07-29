# Install ESLint

yarn add -D eslint prettier @typescript-eslint/{eslint-plugin,parser} eslint-config-{airbnb,prettier} eslint-plugin-{import,jest,jsx-a11y,prettier,react,react-hooks}

1. Local Install

   - begin install start

   ```javascript
      $ npm install eslint --save-dev
   ```

   - setting after install

   ```javascript
      $ ./node_modules/.bin/eslint --init
   ```

   - run eslint at root directory

   ```javascript
     $ ./node_modules/.bin/eslint yourfile.js
   ```

   - also can be run with 'npx'

   ```javascript
     $ npx
   ```

1. Global Install

   - start install

   ```javascript
   $ npm install -g eslint
   ```

   - setting after install

   ```javascript
   $ eslint --init
   ```

   - available to run eslint at dir

   ```javascript
   $ eslint yourfile.js
   ```
