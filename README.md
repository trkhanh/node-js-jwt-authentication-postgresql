# node-js-jwt-authentication-postgresql


Token Based Authentication
Overview of Node.js JWT Authentication with PostgreSQL example
Flow for Signup & Login with JWT Authentication
Node.js Express Architecture with Authentication & Authorization
Technology
Project Structure
Create Node.js App
Setup Express web server
Configure PostgreSQL database & Sequelize
Define the Sequelize Model
Initialize Sequelize
Configure Auth Key
Create Middleware functions
Create Controllers
Controller for Authentication
Controller for testing Authorization
Define Routes
Run & Test with Results
Conclusion
Source Code
Further Reading

# Token Based Authentication
Comparing with Session-based Authentication that need to store Session on Cookie, the big advantage of Token-based Authentication is that we store the JSON Web Token (JWT) on Client side: Local Storage for Browser, Keychain for IOS and SharedPreferences for Android… So we don’t need to build another backend project that supports Native Apps or an additional Authentication module for Native App users.

There are three important parts of a JWT: Header, Payload, Signature. Together they are combined to a standard structure: header.payload.signature.
The Client typically attaches JWT in Authorization header with Bearer prefix:

`Authorization: Bearer [header].[payload].[signature]`

Or only in x-access-token header:

`x-access-token: [header].[payload].[signature]`
