## GraphQL 특징

1. benefit - problems can be solved

- over-fetching
  receiving more data than what i wanted
- under-fetching
  some reqs want more data befor what i want some data
  = a task what i wanted require other tasks before the task complete
- resolver
  해결사, what will do with the received data?
- 'Query' is only used to get data
- 'Mutation' is used to change data

1. there is no URL idea concept

1. define schema - data that we send or get

1. easy to check APIs made before

1. when sand many data ->

```
type Query {
    people: [person]!
}
```
