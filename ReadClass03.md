# class-readings-03-github.io


Why would a developer choose to make data models?

This is a good way of planning in advance how data should be respresented in our codebase, 
and then make the necessary object types to support that plan.


What purpose do CRUD operations serve?

When in the world of data modeling, we want to closely watch and regulate every action that may create or change the data.
CRUD operations make it easier for us.



What kind of database is Postgres? 

SQL database

What kind of database is MongoDB?
noSQL database

What is Mongoose and why do we need it?
Mongoose is a package that acts as a middleman between our application and our database. 
Mongoose is like a JavaScript translator where our application speaks to Mongoose in JavaScript, 
and Mongoose translates that into the terms MongoDB understands. Mongoose also adds a lightweight 
structure and validity checking to our MongoDB, so that we get some of the benefits of an SQL 
database while actually using a NoSQL database.


Define three related pieces of data in a possible application. 
An example for a store application might be Product, Category and Department.
Describe the contraints and rules on each piece of data and how you would relate these pieces to each other. 
For example, each Product has a Category and belongs in a Department.

Each category can have an id and name
const categoryschema = {
      id: { required: true },
      name: { required: true },
    };
    
Each product can have

const productschema = {
      category_id: {type: String, required: true},
      price: { type: Number, required: true },
      department: {type: String,required: true}
    };
