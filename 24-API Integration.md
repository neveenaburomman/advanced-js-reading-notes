## Dynamic API Server
An Express/Node.js based server designed to be a “model agnostic” REST API server, which can perform CRUD operations on any data model

### The API Server must operate as follows:
Support all REST/HTTP methods
- GET: Retrieve record(s) from a data source
All
One (by id)
Some (by filtering)
- POST: Create a new record in a data source
- PUT: Update a single full record in a data source
- PATCH: Update part of a single record in a data source
- DELETE: Delete a record in a data source

### Development Process, Milestones
- Phase 1: API Basics
     Use JSON Server (non-express) to mock the routes for testing purposes
- Phase 2: Basic API
     Create CRUD/ReST endpoints for categories and products
     Separate route modules for each data model type
     Store user created data in memory (no persistence)
     Integrates with an online CI framework
- Phase 3: Persistence
    Replace the in-memory data store with mongo
    Use Mongo Collections for each data model type
- Phase 4: Dynamic Models
    Create a single model class that all data models can inherit from to keep the interface simple
    Use middleware to load models based on param
     i.e. Replace app.get('/api/v1/categories') and app.get('/api/v1/products') with app.get('/api/v1/:model')
     API is Fully Documented
     API is deployed and running live
     
## Authentication Server / Module
An Express/Node.js based server using a custom “authentication” module that is designed to handle user registration and sign in using Basic, Bearer,
or OAuth along with a custom “authorization” module that will grant/deny users access to the server based on their role or permissions level.

## The system to be built will have the following core features:
- Users can create an account, associated with a “role”
User Roles will be pre-defined and will each have a list of allowed capabilities
- admin can read, create, update, delete
- editor can read, create, update
- writer can read, create
user can read
Users can then login with a valid username and password
Alternatively, users can login using an OAuth provider such as Google or GitHub
In this case, users should be automatically assigned the role of user
Once logged in, Users can then access any route on the server, so long as they are permitted by the capabilities that match their role.
