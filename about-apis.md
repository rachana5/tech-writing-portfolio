# About APIs

This document briefly guides you through the concept of APIs, how they work, and the API types and protocols.

## What is an API?

An API (Application Programming Interface) enables applications to communicate for various purposes. Let’s look at it with an example.

Consider that you have a website for your restaurant. You want to add the location of the restaurant to the site so that users can easily find the place. To retrieve the location, you can use the Google Maps APIs. We can extend this example to include an online payment system for our website. To implement this, you can use PayPal’s APIs. Your website is the client and the API service providers (in this case, Google Maps and PayPal) are the servers.

Similarly, many other services build APIs to provide features to client apps. APIs are a set of protocols that other software or hardware can use. APIs are helpful as developers don’t need to build those applications from scratch. In our restaurant example, since you are implementing existing applications, you don’t need to build geolocation software or payment systems.

Additionally, APIs are usually built for a specific purpose. This reduces the cost and errors. Since APIs only share the necessary information, internal data is hidden, keeping the system secure. In many cases, APIs also require user authentication so only authorized users and applications can access the services.

## How do APIs work?

In our restaurant example, we are using the PayPal API payment system to process customer payments. Let’s break down how the payment system works in simple terms:

* On our website, a customer chooses to pay with PayPal. The customer enters the required information.
* Our website makes a request to the payment system through an API call. An API call can consist of a PayPal API URI, request headers, and request body containing the customer data.
* The API receives the valid information and sends the request to the PayPal payment system server.
* The server then responds to the API with the processed request.
* Our website’s payment portal receives that response via the API.

The customer experiences a quick and seamless transaction through this process.

## Types of APIs

Based on the scope of use, the four types of APIs are:

* Public or open APIs

Public API endpoints are open to everyone for use. You may need to authenticate by creating a username and password or by generating API keys. The APIs may also be free or paid.

* Internal or private APIs

Internal API endpoints built for use only within a specific organization. These are used to improve communication between internal systems and other processes. External users do not have access to this type of APIs.

* Partner APIs

Partner APIs are used by partnered organizations to communicate and exchange data. At a certain cost, the business offering the API services allows other businesses to use their APIs to integrate various features.

* Composite APIs

Composite APIs help you execute complex and interdependent tasks. To do this, several endpoints are accessed in the same call. This improves the application performance and increases efficiency since the number of calls to the server are reduced.

## API protocols

API protocols are a set of rules that API developers need to follow when creating APIs. The protocol to be used depends on the purpose of the API. The following are the four common API protocols:

* Simple Object Access Protocol (SOAP)

The server and client communicate using XML as the data format. The SOAP protocol can be used to invoke processes independent of the language and platform. It is recommended to use SOAP for complex applications that require strong security measures to handle sensitive data. For example, financial services and online banking applications.

* Remote Procedure Call (RPC)

RPC APIs allow a client program to remotely execute tasks on the server. The three common RPC implementations include XML-RPC, JSON-RPC, and gRPC. RPC APIs are generally suited to perform basic functions.

* Websocket

Websocket APIs support two-way communication between clients and servers using JSON objects. You can use this protocol to implement real-time communication and data transfer.

* Representational State Transfer (REST)

REST APIs are the most commonly used APIs. REST APIs are stateless. This means that when you send requests to the server, the APIs do not hold to the client data in between the requests. REST APIs are used for both web and mobile applications. They are ideal for cases where you need interoperability, scalability, and flexibility in retrieving data.

## Examples

Some common examples of APIs that we see in our daily lives include:

* Third-party login

You would have seen the options like “Login with Google” and “Login with Facebook” on many sites and apps. This enables you to use your Google or Facebook credentials to access various platforms. These platforms incorporate the Google or Facebook APIs in their user login flow for quick authentication.

* Social media apps

Social media apps such as Twitter and Facebook provide APIs that other organizations and apps can use to integrate the features in their systems. This facilitates content sharing on other platforms. Additionally, real-time communication service providers such as Twilio provide APIs to integrate SMS and notification features.

* Weather apps

Various weather APIs provide real-time data such as temperature, precipitation, alerts, and so on. The weather apps use the APIs to display the data to you.

* Navigation apps

Similar to the previous service providers, navigation APIs provide maps, routes, traffic information, and other location-based services. For example, Google Maps.

> **Note:** For a hands-on guide to using APIs, see the [Translate text with DeepL API](deepl-postman.md) topic.
