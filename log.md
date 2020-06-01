# 100 Days Of Learning Code - Log

This is my progress log for my 100 days of learning code challenge.  I will update my goals as i progress through learning web development.


**==== GOALS ====** 
<table>
<thead>
    <th>Topic</th>
    <th>Status</th>
    <th>Topics</th>
</thead>
<tbody>
    <tr>
        <td rowspan="3">NodeJS</td>
        <td rowspan="1">Completed</td>
        <td rowspan="1">To Do List</td>
    </tr>
    <tr>
        <td rowspan="1">In Progress</td>
        <td rowspan="1">Tour Booking</td>
    </tr>
        <tr>
        <td rowspan="1">Not Started</td>
        <td rowspan="1">PassportJS</td>
    </tr>
    <tr>
        <td>ReactJS</td>
        <td>Not Started</td>
    </tr>
    <tr>
        <td>React Native</td>
        <td>Not Started</td>
    </tr>
    </td>
    <tr>
        <td rowspan="2">Javascript</td>
        <td rowspan="1">Not Started</td>
        <td rowspan="1">Async and Promises</td>
    </tr>
    <tr>
        <td rowspan="1">Not Started</td>
        <td rowspan="1">Regex</td>
    </tr>
</tbody>
</table>

# Day 1: May 21, 2020
##### Started the 100 days of code challenge 

## Today's Progress: 
* Introduction to NodeJS and REPL 
* NodeJS standard libraries (fs, event, util)
* Learn About Buffer and Streams
* Read Stream, Write Stream and Piping.
* Routing with vanilla NodeJS`
* NPM, package.json

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

# Day 3: May 23, 2020
#### Started on Udemy Express Bootcamp

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

# Day 7: May 27, 2020

**Today's Progress**: 
* Learning about Mongoose Middleware (Pre and Post)
    * Document Middleware
    * Query Middleware
    * Aggregation Middleware
* Built in validators and custom validators in Mongoose
* Node Debugging with ndb
* unhandled route handling
    * Error handling middleware

### Notes
* Query middleware can be use to hide documents or perform pre-filtering
* There is a differences between find and findOne event
* When creating a middleware with 4 parameter, express will know it is a error-handling middleware

### Challenges

# Day 8: May 28, 2020

**Today's Progress**: 
* Exception handling, Uncaught Exception
* creating user models
* using bcrypt to hash user password.
* Json Web Tokens and Protected Route
* Postman for API and environment setup

### Notes
* Exception handling should be at top of code, otherwise it may not run for code running before exception.
* Password and private fields should be set to select: false by default, this way unless specified, user will have no access to such information
* to get hidden fields, we need to explicitly set select('fields') to get the field
* Token are usually stored in headers and the key value pair is as such: { authorization: Bearer Token_name }

### Challenges


# Day 9: May 30, 2020
skipped May 29 due to work but it's the weekend again, so time to catch up on learning.

**Today's Progress**: 
* account roles
* Reset Password and NodeMailer
* Capture email using mailtrap during development
* Allow user to update their own password.
* Security and rate-limiter
* sending JWT in cookies
* Implementing helmetjs for http header
* Data Modelling, 1 : few, 1 : Many, 1 : Ton, Many: Many
* GeoJSON Data which work using lat and lon to identify locations

### Notes
* To pass argument into middleware function, we can use a wrapper which take in a argument and returns a middleware function
* When reseting password, sometime token is created earlier than data being saved, so token may not be valid, we can insert a buffer time to prevent this.
* If database timing is different from backend, how will it work? 
* findByIdAndUpdate() will not work for fields like password as their default select value is false, and pre-"save" middleware will not run on update.
* Parameter Pollution, express will convert 2 element of the same name into a array.


### Challenges
* Spend too long debugging on issue where bcrypt return Error: Illegal arguments: undefined, number
* This is due to calling a pre - save middleware which run bcrypt on password change and new password being keyed for the user.
* Using (!document.isModified('password')) allows me to skip this encrypting of password.
* Found out about nosql injection where vulnerability can be exploited by sending a query instead of given text

# Day 10: May 31, 2020
1/10th of this challenge is completed and i still have so much to learn, i never thought that i would learn so much in these 10 days. I have also added a list of useful middlewares that i am working with for my first course. 

**Today's Progress**: 
* Learn about referencing datatype and populating in mongoose
* Virtual Populate
* Nested Route, mergeParams. 
* Factory Function
* indexes when filtering

### Notes
* when using referencing, the ref should have the same <b>name</b> as the model mongoose.model(<b>name</b>, schema="xxSchema")
* Using virtual populate we can make a parent/child reference without having it being persistent
* nested route can be implemented but in order to pass parameters we need to use the option mergeParams: true in express.Router()
* middleware run in sequence, we can implement authentication and authorization using middleware on all function by running middleware before running those function.
* when selecting use <code>.select(+fields)</code> instead of <code>.select(fields)</code> as without the plus sign, it will only extract that single field
* By default, mongoDB will search all query based on id, we can set our own indexes to make this search faster. all unique field will have a index. There is also a compound index where multiple field can be use as index
* Post middleware does not have access to next()
* Query middleware have no access to "this", in this case, this refers to the query. We can execute the query to get the document
* this refers to the query in pre but not in post
* /^findOneAnd/ refers to findbyIdAndUpdate and findByIdAndDelete

### Challenges

## Useful Middlewares (Externals)

<code>
This is a collection of middleware that i think is useful for every project.

* helmet - Inclusion of HTTP-headers for security purpose
* bcryptjs - Salting and hashing of password
* dotenv - allow the use of custom environmental variables
* express - Make life Easier for creating backend services
* express-rate-limit - prevent dos/ddos and high volume access to server
* nodemailer - use to send out email
* validator - library for validating and sanitizes strings. Can be use with mongoose model validate.
* morgan - for logging purpose
* mongoose - ODM for mongoDB and nodeJS
* jsonwebtoken - JWT provide a way of authorization for users
* express-mongo-sanitize - prevent query attack for mongoDB by removing all dots and dollar sign.
* xss-clean - sanitization for input by cleaning malicious code from inputs
* hpp - http parameter pollution prevention middleware, the result will be using the last parameter. takes in a whitelist array
</code>