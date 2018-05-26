# Figuring out `send-introspection-query`

## diff on introspection for [graphql/ppx](https://github.com/mhallin/graphql_ppx/blob/master/sendIntrospectionQuery.js) and [graphql/utilities] from [aws-appsync-codegen](https://github.com/awslabs/aws-appsync-codegen/blob/master/package.json) which uses the introspection query package from [graphql-js](https://github.com/graphql/graphql-js/blob/master/src/utilities/introspectionQuery.js)

## Purpose

Trying to figure out if this is causing errors in graphql/ppx.
see issue here: https://github.com/apollographql/reason-apollo/issues/98#issuecomment-392239469

Looks like this is not the source of the error as the diff for the actual query is the same except for where graphq-js passes a variable for `definition`.
