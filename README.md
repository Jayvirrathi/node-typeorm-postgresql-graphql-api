# Graphql API with Node.js, PostgreSQL with TypeORM

> A Basic Node.js project

## Build Setup

```bash
# install dependencies
npm install

# serve at http://localhost:3000/graphql

npm start
```

## Prerequisites

-   Nodejs
-   Postgresql

**Request:**

```gql
mutation {
    createProduct(variables: { name: "IPhone 11 Max", quantity: 25 }) {
        quantity
        name
        id
    }
}

mutation {
    updateProduct(fields: { name: "IPhone 11 Max", quantity: 45 }, id: 1)
}

query {
    products {
        id
        name
    }
}

query {
    products {
        id
        name
        quantity
    }
}

mutation {
    deleteProduct(id: 1)
}
```
