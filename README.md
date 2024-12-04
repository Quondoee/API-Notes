# REST API Notes




## 1. What is an API?

An **API** (Application Programming Interface) is a set of rules that allows different software applications to communicate with each other. It defines the methods and data formats that applications use to request and exchange information. APIs are crucial for enabling integration between different systems.



## 2. What is HTTP?

**HTTP** (HyperText Transfer Protocol) is the foundation of data communication on the web. It is a protocol used for transmitting data over the internet, primarily between web browsers and servers. HTTP operates through a request-response cycle, where a client sends a request to the server, and the server responds with the requested data.



## 3. Different Types of HTTP Headers

HTTP headers carry metadata that is sent with requests and responses. Some important types include:
- **Request Headers**: Used by the client to provide information like authentication tokens, user agent, and language preferences.
- **Response Headers**: Sent by the server to provide information about the server itself, content type, and caching.
- **General Headers**: Include data relevant to the entire request or response, such as connection management.



## 4. Different Types of HTTP Methods

HTTP methods define the action the client wants to perform on a resource. Common methods include:
- **GET**: Retrieve data from the server.
- **POST**: Submit data to the server to create a new resource.
- **PUT**: Update an existing resource on the server.
- **DELETE**: Remove a resource from the server.
- **PATCH**: Apply partial modifications to a resource.



## 5. What is a REST API?

A **REST API** (Representational State Transfer) is a web service API that adheres to the principles and constraints of REST architecture. It allows for efficient, stateless communication and uses standard HTTP methods to perform CRUD operations on resources (data).



## 6. Key Features of REST APIs

Key features of REST APIs include:
- **Stateless**: Each request from a client must contain all the information necessary to understand and process the request.
- **Client-Server Architecture**: The client and server are separate entities, each with distinct roles.
- **Cacheable**: Responses must explicitly define whether they can be cached to improve performance.
- **Uniform Interface**: A standardized way of interacting with resources through HTTP methods and URIs.
- **Layered System**: REST allows for a layered architecture, promoting scalability and modularity.



## 7. Principles of REST API

RESTful services must follow these core principles:
1. **Statelessness**: Each request is independent, and the server does not store any session state.
2. **Client-Server Separation**: Client and server operate independently, with a clear interface between them.
3. **Cacheability**: Responses must be explicitly labeled as cacheable or non-cacheable.
4. **Uniform Interface**: The way resources are accessed and manipulated must be consistent.
5. **Layered System**: Clients cannot ordinarily tell whether they are connected directly to the server or an intermediary.



## 8. Anatomy of a REST API

A typical REST API includes:
- **Base URL**: The root address of the API (e.g., `https://api.example.com/`).
- **Resources**: Entities that represent data (e.g., `/users`, `/products`).
- **HTTP Methods**: Operations on resources (GET, POST, PUT, DELETE).
- **Response Codes**: Indicate the status of the request (200 for success, 404 for not found, etc.).
- **Request & Response Formats**: JSON or XML are commonly used for data interchange.


## 9. CRUD Operations

CRUD stands for:
- **Create**: Add a new resource (POST).
- **Read**: Retrieve data (GET).
- **Update**: Modify an existing resource (PUT/PATCH).
- **Delete**: Remove a resource (DELETE).

These operations are the fundamental actions for interacting with resources in a RESTful API.


## 10. Best Practices for REST APIs

To build robust and maintainable REST APIs, consider the following best practices:
- **Use HTTP Status Codes Appropriately**: 200 for success, 201 for resource creation, 400 for bad requests, 404 for not found, 500 for server errors.
- **Version Your API**: Use versioning in the API URL (e.g., `/v1/resource`) to maintain backward compatibility.
- **Use Consistent Naming Conventions**: Stick to plural nouns for resource names, e.g., `/users`, `/posts`.
- **Validate Input**: Always validate input to avoid security vulnerabilities.
- **Authentication & Authorization**: Use OAuth, JWT, or API keys for secure access control.



## 11. Building a REST API

Steps to build a basic REST API:
1. **Choose a Technology Stack**: Select a backend framework (e.g., Express.js, Flask, Django) and database (e.g., MongoDB, PostgreSQL).
2. **Define Resources**: Identify the resources your API will expose (e.g., users, products).
3. **Set Up Routing**: Define routes that correspond to HTTP methods for each resource.
4. **Implement CRUD Operations**: Use the correct HTTP methods to interact with data.
5. **Add Error Handling**: Ensure that your API responds with meaningful error messages for failed requests.
6. **Deploy**: Once developed, deploy the API to a server or cloud provider like AWS or Heroku.



