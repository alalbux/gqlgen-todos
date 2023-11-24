# gqlgen-todos

This is a GraphQL project in Go for managing a list of tasks (todos) using gqlgen.

## Prerequisites

Make sure you have Go installed on your machine. You can download it at [https://golang.org/dl/](https://golang.org/dl/).

### Installation

1. Clone this repository:
```
git clone https://github.com/your-username/gqlgen-todos.git
```

2. Navigate to the project directory:
```
cd gqlgen-todos
```

3. Install dependencies:
```
go mod download
```

### Configuration
Copy the .env.example file to a new file named .env:

```
cp .env.example .env
```
Edit the .env file as needed, configuring variables such as ports and database settings, if applicable.

### Running the Server
Run the following command to start the server:
```
go run server/main.go
```

The GraphQL server will be available at http://localhost:8080.

### Example GraphQL Query
You can use tools like Insomnia or Postman to make GraphQL queries.

Example query to get all todos:

```graphql
query {
  todos {
    id
    title
    completed
  }
}
```

Feel free to adjust this README as needed based on the specific details of your project. Make sure to provide enough information so that other developers can easily set up and run the project on their own machines.
