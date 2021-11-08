# GraphQL Quiz

?: What is GraphQL?

( )It is an algorithm in graph theory.
( )GraphQL is the technology for building APIs.
( )GraphQL is a communication protocol.
( )GraphQL is a cognitive architecture.

?: What does SDL stand for in GraphQL?

( )Structured Data Language
( )Syntactic Definition Language
( )Schema Definition Language
( )Syntactic Data Language

?: What operations can we execute on the GraphQL server?

( )Queries, aliases and directives
( )Only queries and mutations
( )Directives and fragments
( )Queries, mutations and subscriptions

?: What is underfetching?

( )When you fetch too much data that are not even used.
( )When we do not have enough data in the first request, so we need to call additional requests to obtain all needed data.
( )When we use the special library called "unfetch".
( )An optimization technique for GraphQL mutations.

?: Is GraphQL only for React developers?

( )Yes
( )No

?: What does a `!` indicate in GraphQL's SDL?

( )A value will be updated
( )A value is optional
( )A value can be deleted
( )A value is required

?: Select all the Scalar types native to GraphQL:

[ ]ID
[ ]Float
[ ]Date
[ ]Boolean
[ ]String
[ ]Post

?: What GraphQL feature improves the structure and reusability of your code?

( )Aliases
( )Fragments
( )Refactoring
( )Queries

?: Given this schema:

```graphql
type Animal {
  id: ID!
  age: Float
  alive: Boolean
  breed: String
  zoo: Zoo
}
type Location {
  id: ID!
  address: String!
  city: String!
  state: String!
  zoos: [Zoo]!
}
type Zoo {
  id: ID!
  animals: [Animal]
  location: Location!
  name: String
}
```

Select all that are true:

[ ]Zoos have many animals
[ ]Location's address field is a Scalar type
[ ]A zoo belongs to a Location
[ ]Animal's age field is not required

?: Given the schema above, select the fields below that are required:

[ ]Zoo name
[ ]Zoo location
[ ]Location ID
[ ]Animal age
[ ]Location state

?: Let's say we want to query for 2 specific Animals, like so:

```graphql
{
  Animal(id: 8) {
    age
    breed
  }
  Animal(id: 14) {
    age
    breed
  }
}
```

This would be invalid because GraphQL cannot resolve two identically named queries. What feature could we use to solve this issue?

( )Fragments
( )Arguments
( )Aliases

?: What major problems do aliases handle?

( )Aliases reduce overfetching.
( )Aliases reduce underfetching.
( )Aliases allow us to call the same query with different variables in a single GraphQL request.
( )Aliases are special type of custom scalars which name fields differently based on received data.

?: In GraphQL type definitions, each field can take zero or more arguments.

( )True
( )False

?: In GraphQL, there is no such concept of default arguments.

( )True
( )False

?: What is a resolver function?

( )A function that a GraphQL client uses to resolve a query on the frontend
( )A function on a GraphQL server that's responsible for fetching the data for a single field
( )A function that solves all your problems
( )It's a synonym for serverless functions
