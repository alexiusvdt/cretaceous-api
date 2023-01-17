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
create endpoints for PUT/DEL:
  api/animals/{id} PUT  -> changes existing information (Update)
  api/animals/{id} DEL  -> del it
Add queries
Add Validation:
  [required]
  [stringlength]
  [range]
  etc
    like with the MVC apps add system.componentmodel.dataannotations to access data annotations like validation attrs
    add [tag] to whatever 
    add [errormessage]s as desired
Typically the requirements that we add to our project models, we'll also want applied to our database. However, if you don't want the changes applied to your database, use a ViewModel to separate the database entity model from the ViewModel that you use to handle incoming requests and validate them. 

