# go-graphql
Build simple GraphQL using Golang

# create todo
mutation createTodo {
  createTodo(input: {text: "task 2", userId: "2"}){
    user{
      id
    }
    text
    done
  }
}

# find todos
query findTodos{
  todos{
    text
    done
    user {
      id
      name
    }
  }
}