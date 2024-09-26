A fork of https://github.com/dotansimha/graphql-code-generator to create a custom version of the typescript operations plugin, i.e. forking the [@graphql-codegen/typescript-operations](https://www.npmjs.com/package/@graphql-codegen/typescript-operations) package.

The fork adds a new option referenceFragmentSpreads, which directs the codegen to apply fragment spreads as types, rather than inlining. It also directs the codegen to just assume all fragment types are available, which relies on importing any fragment types that are externally defined. This importing must be handled by https://github.com/asa-graphql-codegen/asa-graphql-ts-typed-document. In other words, `referenceFragmentSpreads` assumes `asa-graphql-ts-typed-document` is being used.

### Running Tests

```
yarn test --testNamePattern="TypeScript Operations Plugin"
```
