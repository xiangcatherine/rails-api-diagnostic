# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
* receive incoming requests from a front-end
* execute specific behaviors in response to those requests
* create, read, update, or destroy data records through some kind of data storage system
* share information back to the browser
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
Model
```

Which layer in the MVC pattern communicates with the model?

```md
Controller
```

Why don't we use views in our interpretation of the MVC pattern?

```md
// your response here
```

What does C.R.U.D stand for?

```md
Create, Read, Update, Delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
// your response here
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
create, index, update, destroy, show
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
1. There needs to be a GET request route, e.g.:
   - resources :books, only: [:index, :show]
2. There needs to be a Controller (e.g. BooksController)
   - The Controller gets from the model
3. The index method needs be defined
4. There needs to be a model, we can do this using the command line, e.g.:
   - $ bin/rails generate model Book title:string author:string
4. Generates output, which alters the view.
```

What is the command to generate a new rails-api app?

```bash
rails new
```

What is the command to start an instance of a rails server?

```bash
rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
db:drop
db:create
db:migrate
db:seed
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
rails generate scaffold Pet name:string age:integer
```
