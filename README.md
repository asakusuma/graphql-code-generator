A fork of [https://github.com/dotansimha/graphql-code-generator](https://github.com/dotansimha/graphql-code-generator) to create a custom version of the typescript operations plugin:

https://github.com/asa-graphql-codegen/graphql-code-generator/tree/master/packages/plugins/typescript/operations

The fork adds a new option `referenceFragmentSpreads`, which directs the codegen to apply fragment spreads as types, rather than inlining. It also directs the codegen to just assume all fragment types are available, which relies on importing any fragment types that are externally defined.
