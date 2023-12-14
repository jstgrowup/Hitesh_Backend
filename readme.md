- The common standard for the client to communicate with the server is REST
- REST is has a certain set of rules 
   - Uniform Interface
   - Client-Server
   - Stateless
   - Cachable 
   - Layered System
   - Code On Demand
- An API that follows a REST Standard is called a Restful API
- A REST API is organizes the resources in the form of URIs(Unique resouce indentifiers)
- URI differentiates the 

REST is the most common communication standard  between computers over Internet. What is it? Why  
is it so popular? Let's take a look. API stands  for Application Programming Interface. It is  
a way for two computers to talk to each other.  The common API standard used by most mobile and  
web applications to talk to the servers is called  REST. It stands for REpresentational State Transfer. 
It is a mouthful.
- What does that mean? REST is not  a specification. It is a new set of rules that  

has been the common standard for building web API  since the early 2000s. An API that follows the REST  

standard is called a RESTful API. Some real-life  examples are Twilio, Stripe and Google Maps.  

Let's look at the basics of REST. A RESTful API  organizes resources into a set of unique URIs, or  

Uniform Resource Identifiers. The URIs  differentiate different types of resources  

on a server. Here are some examples. The resources  should be grouped by noun and not verb. An API to  

get all products should be slash products and not  slash getAllProducts. A client interacts with a  

resource by making a request to the endpoint for  the resource over HTTP. The request has a very  

specific format, as shown here. The line contains  the URI for the resource we'd like to access.  

The URI is preceded by an HTTP verb which tells  the server what we want to do with the resource.  

A POST request means we want to create a  new resource. A GET means we want to read  

the data about an existing resource. A PUT is  for updating an existing resource. A DELETE is  

for removing an existing resource. You might have  heard the acronym CRUD. This is what it stands for.  

In the body of these requests, there could be  an optional HTTP request body that contains  

a custom payload of data, usually encoded in  JSON. The server receives a request, processes it,  

and formats the result into a response. The first  line of the response contains the HTTP status code  

to tell the client what happened to the request.  A well-implemented RESTful API returns proper  

HTTP status codes. The 200-level codes mean the  request was successful. The 400-level codes means  

something was wrong with our request. For example  the requests contain incorrect syntax. At the 500- 

level, it means something went wrong at the server  level. For example, the service was unavailable.  

A well-behaved client could choose to retry a  failed request with a 500-level status code. We  

said "could choose to retry" because some actions  are not idempotent, and those require extra care  

when retrying. When an API is idempotent, making  multiple identical requests has the same effect  

as making a single request. This is usually not the  case for a POST request to create a new resource.  

The response body is optional and could contain  the data payload and is usually formatted in JSON.  

There's a critical attribute of  REST that is worth discussing more.  
A REST implementation should be stateless. It  means the two parties don't need to store any  

information about each other, and every request  and response (cycle) is independent from all others.  

This leads to web applications that are easy to  scale and well behaved. There are two final points  

to discuss to round out a well-behaved RESTful API.  If an API endpoint returns a huge amount of data,  

use pagination. A common pagination scheme  uses "limit" and "offset" as parameters. Here is  

an example. If they are not specified, the server  should assume sensible default values. Lastly,  

versioning of an API is very important. Versioning  allows an implementation to provide backward  

compatibility, so that if we introduce breaking  changes from one version to another, consumers  

can get enough time to move to the next version.  There are many ways to version an API. The most  

straightforward is to prefix the version before  the resource on the URI. For instance, like this.

RESTful API is simple and effective when  applied sensibly. It may not be the best  

choice for all companies, but it is simple and  good enough, and that's why it is so widely used.  

There are other popular API options like GraphQL  and gRPC. We'll discuss those and compare them in  

separate videos. If you would like to learn more about system  design, check out our books and weekly newsletter.  

Please subscribe if you learned something new.  Thank you so much, and we'll see you next time.
