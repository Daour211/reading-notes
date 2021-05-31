## Status Codes Based On REST Methods

**HTTP Status CodesPermalink**

A status code is a number higher than 100 and smaller than 600 that is part of a HTTP response. The first digit defines the class of the status.
A status code comes with a reason phrase. The code is for programmatic recognition the phrase is for humans to understand what happened.

Q1) In your own words, describe what each group of status code represents:

100’s = they are informational status codes; which tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client.

200’s = They are success codes which tell the client that the resource they are requesting isn’t available at the expected location anymore.

300’s = They are the client error codes, which tell the client that the resource they are requesting isn’t available at the expected location anymore.

400’s = They are the client error codes, which are all about invalid requests a client sent to a server.

500’s = They are the server error codes. They indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server.

Q2) What is a status code 202?<br>

For “create”: 
This code tells the client that the request was valid, but its processing will finish sometime in the future.

For “update”:
If the update is done asynchronous, this code can be used. It should include an URL to access the updated resource or an URL to check if the update has been succeeded. 


Q3) What is a status code 308?<br>

This is the right code if the resource will now be available at a new URL and the client should directly access it via the new URL in the future.

Q4) What code would you use if an update didn’t return data to a client?<br>

Code 204 No Content

Q5) What code would you use if a resource used to exist but no longer does?<br>

Code 410 Gone

Q6) What is the ‘Forbidden’ status code?<br>

403: The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.


## Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes

Q1) Why do we need to pull our MongoDB database string out of our server and put it into our .env?<br>
Because when we deploy our app we want to use something that is not local host.

Q2) What is middleware?<br>
It is a code that runs once the server get request before it get passed. (A software that lies between an operating system and the applications running on it) 


Q3) What does app.use(express.json()) do?<br>
It lets the server to accept as body inside a post element or get element 


Q4) What does the /:id mean in a route?<br>
To access whatever comes after the “/” to 

Q5) What is the difference beween PUT and PATCH?<br>
Patch used to update based on what the user is passing 

Put creates a resource or updates an existing resource.

Q6) How do you make a default value in a schema?<br>
By typing ‘default” as property of a value we create. 

Q7) What does a 500 error status code mean?<br>
It means that there is an error in the server 

Q8) What is the difference between a status 200 and a status 201?<br>
200: It means that everything was successful 

201: It means successfully created in object (it specifies what was successful that I created something)
<br>
<br>


**Resources:**
 - [Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

- [Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

