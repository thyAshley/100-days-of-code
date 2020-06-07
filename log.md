# 100 Days Of Learning Code - Log

This is my progress log for my 100 days of learning code challenge. I will update my goals as i progress through learning web development.

**=== Major Projects===**

<table>
    <tr>
        <th>Application</th>
        <th>Username</th>
        <th>Password</th>
    </tr>
    <tr>
        <td>
            <a href="https://natoursbooking.herokuapp.com/">Tour Booking Application</a>
        </td>
        <td>leo@example.com</td>
        <td>test1234</td>
    </tr>
</table>

**==== GOALS ====**

To learn about fullstack development over and beyond this 100 days

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
        <td rowspan="1">Completed (to re-do)</td>
        <td rowspan="1">Tour Booking</td>
    </tr>
        <tr>
        <td rowspan="1">Not Started</td>
        <td rowspan="1">PassportJS</td>
    </tr>
    <tr>
        <td>ReactJS</td>
        <td>In Progress</td>
    </tr>
    <tr>
        <td>Dot Net C#</td>
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

- Introduction to NodeJS and REPL
- NodeJS standard libraries (fs, event, util)
- Learn About Buffer and Streams
- Read Stream, Write Stream and Piping.
- Routing with vanilla NodeJS`
- NPM, package.json

# Day 2: May 22, 2020

## Today's Progress:

- Introduction to Express
- Route Parameters
- Introduction to Templating Engines with EJS
  - View Engine
  - Rendering
  - Passing of data
  - Partial Templates
- Middleware and static files
- Query Strings
- No SQL Database - MongoDB
- dotenv library to store secret keys
- Finish a ToDo-list application using nodejs
- Finish the NodeJS Tutorial

## Notes

- Express default views directory should be views. To use another directory instead of the default use express.set('views', \_\_dirname + '/directory name').

- to use a static file location, app.use('route', express.static('folder_name'))
  with this, we can apply css to our html files. By convention, this folder will be called "Public"

- body-parser middleware is now built into express

- When pushing information to git, make sure all sensitive information such as password are in .gitignore file.

## Challenges

- Unable to call a delete method from a form, but found a way to use a get request to perform delete operations [not sure if this is the right way]

# Day 3: May 23, 2020

#### Started on Udemy Express Bootcamp

**Today's Progress**:

- Recap Synchronous and Asynchonous Blocking
- Customise HTML Template how how html template works
- Introduction to Slugify library to replace html params links.
- Understanding HTTP/HTTPS requests.
- Using Vanilla checklist to create a inventory list
  - Routing
  - Custom Template with replace and regex
  - url parsing

### Challenges

- A lot of regex involved, to include regex and javascript in this 100 days challenge

# Day 4: May 24, 2020

**Today's Progress**:

- Learning about NodeJS Stream
- Asynchronous, Callback, Promises
- Async function and Awaits
- API Testing with Postman
- RESTful API architecture, creating RESTFul with express
- Created a GET and POST API to get tour list and add new tour into the list
- Reading parameters from url
- Learning about route for refactoring http methods.

### Notes

- we can create a promise by using ES6 new Promise((resolve, reject)), we can call resolve() and reject() to indicate if the promise is successful or not.

### Challenges

- confuse when to use async function and when to use promises or if they are interswappable. To research on this more.
- was using status code 204 which stands for no-content and try to send a json response back to the user when the user call the API. Notice there was no response and tried fixing the issue, found out eventually that http status 204 will not include ny message body.

# Day 5: May 25, 2020

**Today's Progress**:

- Request Response Cycle and Middleware
- Mounting Routers
- Separation of Concerns
- Param middleware
- Middleware chaining
- Environment variables
- MongoDB and Mongoose
  - Creating MongoDB Schema
  - Creating MongoDB Model
- Created CRUD API request using express and mongoDB.
- Working with process.argv
- API query string
- Implemnting filters on query string

### Notes

- To look more into MVC setup

# Day 6: May 26, 2020

**Today's Progress**:

- Advance Filtering on query string
  - GTE/LTE/LT/GE using regex and replace
  - Sorting [query = ?sort=name or sort=-name, ascending and descending]
  - Field Limiting fields[query= ?fields=name,price,e.g.]
  - Pagination [query = ?page=10&limit=5 e.g.]
  - Aliasing using middleware to pre-fill query string
  - MongoDB Aggregation pipeline and unwinding data
  - Virtual Property

### Notes

- We are unable to mix inclusion and exclusion fields during field limiting
- Certain fields can be excluded in the schema, e.g. sensitive data
- Aggregation pipeline has multiple layers, the first layer is usually what data is to be extracted, next we can use \$group to group all this data together and use aggregation function such as sum, avg, min, max to aggregate our data.
- Virtual property cannot be used in a query.

### Challenges

- Having issue understanding regex syntax and wrapping around the idea of advance filtering.
- Careless mistake in creating API using comma instead of ampersand cause unwanted debugging effort
- Order of routing matters, we should not place any route below a params route :id otherwise node will treat it as a params route.

# Day 7: May 27, 2020

**Today's Progress**:

- Learning about Mongoose Middleware (Pre and Post)
  - Document Middleware
  - Query Middleware
  - Aggregation Middleware
- Built in validators and custom validators in Mongoose
- Node Debugging with ndb
- unhandled route handling
  - Error handling middleware

### Notes

- Query middleware can be use to hide documents or perform pre-filtering
- There is a differences between find and findOne event
- When creating a middleware with 4 parameter, express will know it is a error-handling middleware

# Day 8: May 28, 2020

**Today's Progress**:

- Exception handling, Uncaught Exception
- creating user models
- using bcrypt to hash user password.
- Json Web Tokens and Protected Route
- Postman for API and environment setup

### Notes

- Exception handling should be at top of code, otherwise it may not run for code running before exception.
- Password and private fields should be set to select: false by default, this way unless specified, user will have no access to such information
- to get hidden fields, we need to explicitly set select('fields') to get the field
- Token are usually stored in headers and the key value pair is as such: { authorization: Bearer Token_name }

# Day 9: May 30, 2020

skipped May 29 due to work but it's the weekend again, so time to catch up on learning.

**Today's Progress**:

- account roles
- Reset Password and NodeMailer
- Capture email using mailtrap during development
- Allow user to update their own password.
- Security and rate-limiter
- sending JWT in cookies
- Implementing helmetjs for http header
- Data Modelling, 1 : few, 1 : Many, 1 : Ton, Many: Many
- GeoJSON Data which work using lat and lon to identify locations

### Notes

- To pass argument into middleware function, we can use a wrapper which take in a argument and returns a middleware function
- When reseting password, sometime token is created earlier than data being saved, so token may not be valid, we can insert a buffer time to prevent this.
- If database timing is different from backend, how will it work?
- findByIdAndUpdate() will not work for fields like password as their default select value is false, and pre-"save" middleware will not run on update.
- Parameter Pollution, express will convert 2 element of the same name into a array.

### Challenges

- Spend too long debugging on issue where bcrypt return Error: Illegal arguments: undefined, number
- This is due to calling a pre - save middleware which run bcrypt on password change and new password being keyed for the user.
- Using (!document.isModified('password')) allows me to skip this encrypting of password.
- Found out about nosql injection where vulnerability can be exploited by sending a query instead of given text

# Day 10: May 31, 2020

1/10th of this challenge is completed and i still have so much to learn, i never thought that i would learn so much in these 10 days. I have also added a list of useful middlewares that i am working with for my first course.

**Today's Progress**:

- Learn about referencing datatype and populating in mongoose
- Virtual Populate
- Nested Route, mergeParams.
- Factory Function
- indexes when filtering

### Notes

- when using referencing, the ref should have the same <b>name</b> as the model mongoose.model(<b>name</b>, schema="xxSchema")
- Using virtual populate we can make a parent/child reference without having it being persistent
- nested route can be implemented but in order to pass parameters we need to use the option mergeParams: true in express.Router()
- middleware run in sequence, we can implement authentication and authorization using middleware on all function by running middleware before running those function.
- when selecting use <code>.select(+fields)</code> instead of <code>.select(fields)</code> as without the plus sign, it will only extract that single field
- By default, mongoDB will search all query based on id, we can set our own indexes to make this search faster. all unique field will have a index. There is also a compound index where multiple field can be use as index
- Post middleware does not have access to next()
- Query middleware have no access to "this", in this case, this refers to the query. We can execute the query to get the document
- this refers to the query in pre but not in post
- /^findOneAnd/ refers to findbyIdAndUpdate and findByIdAndDelete

### Challenges

- Performed a lot of simple mistake and typo, spend hours only to find out i been using the wrong wrong findBy function.
- Still don't understand how is findOneAnd regex linked to findByIdAndUpdate and findByIdAndDelete
- Need to learn more on constructor function as it is confusing using a pre and post middleware with constructor to access the Class

# Day 11: June 1, 2020

**Today's Progress**:

- Unique Entry using indexes.
- setting function in mongoose
- GeoWithin and Geolocation
- Geoaggregation \$geoNear
- Creating documents using PostMan
- PUG templating

### Notes

- we can create unique input by using indexes
- we can use split to destruct array <code>[ el1, el2 ] = array.split(',');</code>
- index for geospatial type is 2d or 2dSphere
- very unfamiliar with using geo datapoint, to practice on this more.

### Challenges

- always look at routing url and router.route url, spend too much trying to fix routing issue

# Day 12: June 2, 2020

**Today's Progress**:

- Working with Pug file to render website
  - Mixin
  - each loop,
  - conditional
- Mapbox API for frontend integration with Maps
- Axios for logging in application on frontend
- pass variables from backend to front using res.locals
- Module Bundler

# Day 13: June 3, 2020

**Today's Progress**:

- Logging out user by sending new cookie without token
- Error handling page, 404
- using form post method and AXIOS for making call to backend
- Express urlencoded to parse form data and data coming by url.

# Day 14: June 4, 2019

**Today's Progress**:

- Working with Multer library for file uploading
  - single file uploading
  - multi file uploading
  - enctype multipart/form-data
  - Working with SendGrid

### Notes

- use multer.single for single file upload, multer.array for multiple same file upload and multer.fields for multiple different file upload
- using map return a array of promises which we can apply promise.all() for.

# Day 15: June 5, 2019

**Today's Progress**:

- Working with Stripe API
- Deployed Website on Heroku, finish baseline project for making a tour booking application using nodejs
- heroku sigterm and allowing cross origin resource sharing of APIs
- webhooks

### Notes

- May be a bug with parcel bundle, but stripe need to be on all pages.
- Nodemon only for development
- heroku dyno restart every 24h use a process.on('sigterm') to handle this from shutting down abrutly
- have to set a trust proxy as heroku does not have req.secure
- Web hooks require non-json body, apply this before express.json(). <code>Use express.raw({type: 'application/json'} instead</code>

### Remarks

- Finally done with my first huge course on nodejs, i have learnt a great deal in this 2 weeks on this course. The course is really well detailed but skip some parts like html and css which i would have to go back and review. From this, i found that i prefer to work with ejs as compared to pug as it is more similiar to HTML. At the end of this 100 day challenge, i would like to rebuilt this application again without following the tutorials to see how much i have learn. This application is also only partially completed as the creator left some of the parts as challenges for the us.

# Day 17: June 7, 2019

Started on React Course

**Today's Progress**:

- Updating webhooks to redirect
- JSX - Javascript XML and Babel
- React
  - Class Components and Function Based Components
  - Javascript embedding
  - JSX Conditioning
  - Props
  - Default Props
  - inline-css and adding className.
  - Passing component as props <code>{props.children}</code>
  - React setstates and states
  - Hooks, Functional Components and Context

### Notes

- react has re-usable components concept which make up the entire webpage like lego blocks.
- Before React-Hooks, State and lifecycle is for class based component, so better to just use class based component.
- defaultProps must be called that otherwise it will not work.
- keyword in javascript are replaced in react, e.g. class->className, for->htmlFor
- setState is asynchronous function

<code>
This is a collection of middleware that i think is useful for every project.

- nodemon - Must have application for development for auto restarting of servers
- helmet - Inclusion of HTTP-headers for security purpose
- bcryptjs - Salting and hashing of password
- dotenv - allow the use of custom environmental variables
- express - Make life Easier for creating backend services
- express-rate-limit - prevent dos/ddos and high volume access to server
- nodemailer - use to send out email
- validator - library for validating and sanitizes strings. Can be use with mongoose model validate.
- morgan - for logging purpose
- mongoose - ODM for mongoDB and nodeJS
- jsonwebtoken - JWT provide a way of authorization for users
- express-mongo-sanitize - prevent query attack for mongoDB by removing all dots and dollar sign.
- xss-clean - sanitization for input by cleaning malicious code from inputs
- hpp - http parameter pollution prevention middleware, the result will be using the last parameter. takes in a whitelist array
- cookie-parser - read cookie
- multer - file uploading
- sharp - image resizing
- html-to-text - strip all html and converting to text
- compression - compress all response and text to client
- cors - allow cross origin resource sharing
- faker - populating with fake data

</code>
