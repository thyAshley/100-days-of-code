# 100 Days Of Learning Code - Log

This is my progress log for my 100 days of learning code challenge.  I will update my goals as i progress through learning web development.

**==== GOALS ====** 
<table>
<thead>
    <th>Topic</th>
    <th>Status</th>
    <th>Link</th>
</thead>
<tbody>
    <tr>
        <td>NodeJS</td>
        <td>In Progress</td>
    </tr>
    <tr>
        <td>ReactJS</td>
        <td>Not Started</td>
    </tr>
</tbody>
</table>

**Link(s) to work**
1. [NodeJS Tutorial](https://www.youtube.com/channel/UCW5YeuERMmlnqo4oq8vwUpg) [Completed]
2. [NodeJS Express MongoDB & More: The Complete Bootcamp 2020](https://www.udemy.com/course/nodejs-express-mongodb-bootcamp/) [In-Progress]


# Day 1: May 21, 2020
##### Started the 100 days of code challenge 

## Today's Progress: 
* Introduction to NodeJS and REPL 
* NodeJS standard libraries (fs, event, util)
* Learn About Buffer and Streams
* Read Stream, Write Stream and Piping.
* Routing with vanilla NodeJS`
* NPM, package.json

**Link(s) to work**
1. [NodeJS Tutorial](https://www.youtube.com/channel/UCW5YeuERMmlnqo4oq8vwUpg) 

# Day 2: May 22, 2020

## Today's Progress:
* Introduction to Express
* Route Parameters
* Introduction to Templating Engines with EJS 
    * View Engine
    * Rendering 
    * Passing of data
    * Partial Templates
* Middleware and static files
* Query Strings
* No SQL Database - MongoDB
* dotenv library to store secret keys
* Finish a ToDo-list application using nodejs
* Finish the NodeJS Tutorial

## Notes
* Express default views directory should be views. To use another directory instead of the default use express.set('views', __dirname + '/directory name').

* to use a static file location, app.use('route', express.static('folder_name'))
with this, we can apply css to our html files. By convention, this folder will be called "Public"

* body-parser middleware is now built into express

* When pushing information to git, make sure all sensitive information such as password are in .gitignore file.

## Challenges

* Unable to call a delete method from a form, but found a way to use a get request to perform delete operations [not sure if this is the right way]

**Link(s) to work**
1. [NodeJS Tutorial](https://www.youtube.com/channel/UCW5YeuERMmlnqo4oq8vwUpg) 

# Day 3: May 23, 2020
#### Started on Udemy Express Bootcamp by Jonas Schmedtmann [Link 2]

**Today's Progress**: 
* Recap Synchronous and Asynchonous Blocking
* Customise HTML Template how how html template works
* Introduction to Slugify library to replace html params links.
* Understanding HTTP/HTTPS requests.
* Using Vanilla checklist to create a inventory list
    * Routing
    * Custom Template with replace and regex
    * url parsing

### Notes

### Challenges

* A lot of regex involved, to include regex and javascript in this 100 days challenge

**Link(s) to work**
1. [NodeJS Express MongoDB & More: The Complete Bootcamp 2020](https://www.udemy.com/course/nodejs-express-mongodb-bootcamp/) 

# Day 4: May 24, 2020

**Today's Progress**: 
* Learning about NodeJS Stream
* Asynchronous, Callback, Promises
* Async function and Awaits
* API Testing with Postman
* RESTful API architecture, creating RESTFul with express
* Created a GET and POST API to get tour list and add new tour into the list
* Reading parameters from url
* Learning about route for refactoring http methods.

### Notes
* we can create a promise by using ES6 new Promise((resolve, reject)), we can call resolve() and reject() to indicate if the promise is successful or not.

### Challenges
* confuse when to use async function and when to use promises or if they are interswappable. To research on this more.
* was using status code 204 which stands for no-content and try to send a json response back to the user when the user call the API. Notice there was no response and tried fixing the issue, found out eventually that http status 204 will not include ny message body. 

**Link(s) to work**
1. [NodeJS Express MongoDB & More: The Complete Bootcamp 2020](https://www.udemy.com/course/nodejs-express-mongodb-bootcamp/) 

# Day 5: May 25, 2020

**Today's Progress**: 
* Request Response Cycle and Middleware
* Mounting Routers
* Separation of Concerns
* Param middleware
* Middleware chaining
* Environment variables
* MongoDB and Mongoose
    * Creating MongoDB Schema
    * Creating MongoDB Model
* Created CRUD API request using express and mongoDB. 
* Working with process.argv
* API query string
* Implemnting filters on query string

### Notes
* To look more into MVC setup

### Challenges

**Link(s) to work**
1. [NodeJS Express MongoDB & More: The Complete Bootcamp 2020](https://www.udemy.com/course/nodejs-express-mongodb-bootcamp/) 

# Day 6: May 26, 2020

**Today's Progress**: 
* Advance Filtering on query string
    * GTE/LTE/LT/GE using regex and replace
    * Sorting [query = ?sort=name or sort=-name, ascending and descending]
    * Field Limiting fields[query= ?fields=name,price,e.g.]
    * Pagination [query = ?page=10&limit=5 e.g.]
    * Aliasing using middleware to pre-fill query string
    * MongoDB Aggregation pipeline and unwinding data
    * Virtual Property

### Notes
* We are unable to mix inclusion and exclusion fields during field limiting
* Certain fields can be excluded in the schema, e.g. sensitive data
* Aggregation pipeline has multiple layers, the first layer is usually what data is to be extracted, next we can use $group to group all this data together and use aggregation function such as sum, avg, min, max to aggregate our data.
* Virtual property cannot be used in a query.

### Challenges
* Having issue understanding regex syntax and wrapping around the idea of advance filtering.
* Careless mistake in creating API using comma instead of ampersand cause unwanted debugging effort
* Order of routing matters, we should not place any route below a params route :id otherwise node will treat it as a params route.

**Link(s) to work**
1. [NodeJS Express MongoDB & More: The Complete Bootcamp 2020](https://www.udemy.com/course/nodejs-express-mongodb-bootcamp/) 