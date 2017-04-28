# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
So that users can interact with each other and use the app more dynamically. It
also allows data to be stored and persist over time (e.g. save a game and come
back to it later).
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
Because we generate our own view.
```

What does C.R.U.D stand for?

```md
Create, Read, Update, Delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
Controller
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
create, index, show, update, destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md

- The server receives the GET request
- The server uses the router to figure out which controller to use.
- We then need a Controller, which communicates with the model in order to respond to the request
- The model gets information from the database and returns a response to the Controller
- The controller then communicates that response to the server
```

What is the command to generate a new rails-api app?

```bash
rails-api new
```

What is the command to start an instance of a rails server?

```bash
bundle exec rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
bundle exec db:drop
bundle exec db:create
bundle exec db:migrate
bundle exec db:seed
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
rails generate scaffold Pet name:string age:integer
```
