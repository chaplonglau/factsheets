# HTTP | REST | CRUD 

# HTTP methods 
HTTP stands for Hypertext Transfer Protocol. It is a protocol for communciations between a client and a server. HTTP methods are ways within the protocol to obtain/receive information. 

Rails commonly uses these five HTTP methods 

GET - Request data 
POST - Creating a new resource 
PUT - Update a pre-existing resource with a complete replacement 
PATCH - Update only specified fields of a pre-existing resource 
DELETE - Delete a resource 

(PUT is for replacing everything, and PATCH is for updating a portion.  )

# REST 
REST stands for Representational State Transfer. It is a structural design pattern that most web apps use to communicate with other web apps. There are seven RESTful routes. 

## resource :corgis @ routes.rb will generate the following 7 routes 

| HTTP verb     | route          | action  | meaning                         |
| ------------- |----------------| --------| --------------------------------|
| GET           | /corgis        | index   | list of all corgis              | 
| GET           | /corigs/new    | new     | FORM for new corgi              |
| POST          | /corgis        | create  | create a new corgi              |
| GET           | /corgis/       | show    | display corgi with id of 1      |  
| GET           | /corgis/1/edit | edit    | FORM to edit corgi with id of 1 |
| PATCH         | /corgis/1      | update  | update corgi with id of 1       | 
| DELETE        | /corgis/1      | destroy | delete corgi with id of 1       |

# CRUD 
CRUD stands for Create, Read, Update, and Delete. These operations are essential to any persistent database storage. 

# Tie-it-all-together 

RESTful routes map HTTP verbs to a controller's CRUD actions

