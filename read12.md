# Class 301 Reading12

## Status Codes Based On REST Methods

1. In your own words, describe what each group of status code represents:

**100’s** = Usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client. 
**200’**s = They tell the client that its request was accepted.
**300’s** =  They tell the client that the resource they are requesting isn’t available at the expected location anymore.
**400’s** = They are all about invalid requests a client sent to a server. There are several causes to this, timeouts, wrong URI, missing authentication, etc.
**500’s** =Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server.

2. What is a status code 202?
    - 202 Accepted - Often used for asynchronous processing.

3. What is a status code 308?
    - 308 Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore.

4. What code would you use if an update didn’t return data to a client?
    - 204 No Content

5. What code would you use if a resource used to exist but no longer does?
    - 410 Gone - This is like 404 but we know that the resource existed in the past, but it got deleted or somehow moved, and we don’t know where.


6. What is the ‘Forbidden’ status code?
    - 403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

## Build A REST API With Node.js, Express, & MongoDB

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?
    - Because the database string holds our password.

2. What is middleware?
    - Middleware is software that lies between an operating system and the applications running on it, enabling communication and data management.

3. What does app.use(express.json()) do?
    - a. express.json() is a method inbuilt in express to recognize the incoming Request Object as a JSON Object.

4. What does the /:id mean in a route?
    - The “:id” portion of that route specifies that whatever you put into that position will be passed as the id in the params map.

5. What is the difference between PUT and PATCH?
    - PUT is a method of modifying resource where the client sends data that updates the entire resource . PATCH is a method of modifying resources where the client sends partial data that is to be updated without modifying the entire data.

6. How do you make a default value in a schema?
    - You can specify a default value for an item using the default keyword. When a data doesn't have a corresponding value, the value of this keyword will be used instead to do the validation checks.

7. What does a 500 error status code mean?
    - The HyperText Transfer Protocol (HTTP) 500 Internal Server Error server error response code indicates that the server encountered an unexpected condition that prevented it from fulfilling the request. 

8. What is the difference between a status 200 and a status 201?
    - 200 simply means that the request was received, understood, and is being processed, whereas the 201 status code indicates that a request was successful and a resource was created as a result.

## Things I Want To Know More About

- More react, react, react!!!!

## Sources

- https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/

- https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw
