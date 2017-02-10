# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
The purpose of a backend is to have the users that are using the same app communicate with eachother. We can also use a backend to store informtaion or the state of a game over time. To give a user the ability to save something their progress in the app and then be able to pick up where they left off later.  For persistance.

```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
A Model
```

Which layer in the MVC pattern communicates with the model?

```md
The Controller.
```

Why don't we use views in our interpretation of the MVC pattern?

```md
I think because the view is the data that gets sent back to the client and that's  built using HTML, js, etc.
```

What does C.R.U.D stand for?

```md
CREATE
READ
UPDATE
DELETE
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
In the Controller
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
:: Index
:: Show
:: Create
:: Update
:: Destroy

```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
- The server receives the GET request then sends it the router to find the right  controller to use.
- The controller parses the request  and talks to the model to execute the request.
- The model talks to the database and based on the request that was made it stores and validates data, and returns it to the model/
- Then the model returns the response/ data to the controller.
- The controller returns the response back to the server.
- The server converts the data and  HTTP response and sends it to the client.
```

What is the command to generate a new rails-api app?

```bash

```

What is the command to start an instance of a rails server?

```bash
bin/rails sever
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash

bin/rake db:migrate
bin/rake db:create
bin/rake db:drop
bin/rake db:seed
bin/rake db:examples
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash

bin/rails generate scaffold pet name:string age:integer

```
