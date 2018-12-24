# @jagi/jest-transform-graphql

This package allows you to import your GraphQL queries directly from the \*.gql files in Jest.

```js
import USER_QUERY from "./graphql/userQuery.gql";
```

## Usage

In your `package.json` file:

```js
{
  /* ... */
  "jest": {
    "transform": {
      "\\.(gql|graphql)$": "@jagi/jest-transform-graphql"
      /* ... */
    }
  }
}
```

Or in your `jest.config.js` file:

```js
module.exports = {
  transform: {
    "^\\.(gql|graphql)$": "@jagi/jest-transform-graphql"
    /* ... */
  }
  /* ... */
};
```
