# prettier-config

[![npm version](https://badge.fury.io/js/%40calblueprint%2Fprettier-config.svg)](https://badge.fury.io/js/%40calblueprint%2Fprettier-config)

This package provides a shared Prettier configuration.

## Usage

1. Install this package as a development dependency:

   ```sh
   # with npm
   npm install --save-dev @calblueprint/prettier-config

   # with yarn
   yarn add --dev @calblueprint/prettier-config
   ```

2. Install peer dependencies:

   ```sh
   # with npm or yarn
   npx install-peerdeps --dev @calblueprint/prettier-config
   ```

3. Use the shared Prettier config in your project's `.prettierrc.js`:

   ```js
   module.exports = {
     ...require('@calblueprint/prettier-config'),
     // Add any overrides here
   };
   ```
   
   Note: you may need to remove or merge any other existing prettier config files.

4. Test that the config is working by running `npx prettier --check .` in your project's root directory.