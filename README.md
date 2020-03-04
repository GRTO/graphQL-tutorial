# How to run the project
- Run in terminal `npm run json:server` to run DB.
- Run `npm run serve` to run the express project with the graphQL layer.
- Open http://localhost:3300/graphql to see graphiQL.

## Examples
- Query:

```
{
  company(id: "2") {
    id
    name
    description
    users{
      id
      firstName
      age
    }
  }
}
```

- Mutation:

```
mutation {
  addUser(firstName: "Gerson", age: 24) {
    id
    firstName
    age
  }
}
```