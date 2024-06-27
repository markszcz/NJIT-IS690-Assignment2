## API Design and Implementation

14. **What are REST APIs, and how do they function in your project? Provide an example of a REST endpoint from your user management system.**

REST APIs are a way of creating a standard in order to expose application logic that can be triggered from an external source. Unlike webpages, REST is stateless where all the information necessary in order to execute a command is contained in the request, but similarly to websites, the way you interact with REST APIs is through a URL address. Since the request communicates over stanard HTTP methods, there are standard methods that can be used to trigger a REST API, such as a GET, POST, PUT or even a DELETE request. The data can be transmitted in any format, depending on the application of the backend service, but typically the standard way of sending and recieving data is either in JSON or SML format.

All the "router.get" request for example in the user_routes.py file are REST APIs. The ".get" for /users/ (line 142) is responsible for retrieving a list of users, but the ".post" for /users/ (line 108) is responsible for creating the user.

- user_routes.py [user_routes](../app/routers/user_routes.py)