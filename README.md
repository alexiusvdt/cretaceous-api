filler text filler text

needed packages:
$ dotnet add package Microsoft.EntityFrameworkCore -v 6.0.0
$ dotnet add package Pomelo.EntityFrameworkCore.MySql -v 6.0.0
$ dotnet add package Microsoft.EntityFrameworkCore.Design -v 6.0.0

Steps:
add models
add necessary context model
update program.cs to use mysql and the apicontext
add seed data (updating migrations)
create endpoints for GET/POST:
  api/animals GET       -> return all objects
  api/animals/{id} GET  -> return one object based on ID
  api/animals POST      -> add new to db, requiring object literal of an animal