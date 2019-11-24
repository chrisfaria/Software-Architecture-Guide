# Software Architecture Considerations
## What the guide is about
This guide outlines the steps to document when first planning out an app. There are 9 areas to consider and fill out as a starting point. More areas may come out of it as you work through the process, which is great

1. App overview
1. App features
1. Domain security
1. Domain rules
1. Logging
1. Services / Communication
1. Data Models
1. Feature components
1. Shared functionality

It also includes some links with official best practices, which are mostly quick reads

## The Considerations
### 1 App Overview
What is the app for? What are the overall goals? How will the app be used? Key requirements?

### 2 App Features
List as many app features that you can and detail them. All may not be known initially

### 3 Domain Security
How is security to be handled? What external products will be used? Are we using roles, groups, claims? How will security be communicated to and from the app? Possible security updates down the road? Go through security layers
### 4 Domain Rules
What will be run on front end / back end / both? Business rules, validation, etc

### 5 Logging
What is done when an error is encountered? Write to a cloud option, API, or local storage? How to control logging levels? Make sure it’s easy to support when an issue is raised

### 6 Services/Communication
How will this app talk to other pieces? HTTP? Web Sockets? REST? JSON/XML/MessagePack? Other services?

(Angular) HTTP Interceptor?

### 7 Data Models
What data are we expecting? Do we need subsets of data sent to us? What data do we need to send? What data is being viewed? 

(Angular) Use classes or interfaces? If you need functions within then use classes else use interfaces as they don’t get bundled up in the app when built reducing size

### 8 Feature Components
What are our top level components and how will be structure them? How to organize in the code? Draw out layout	

(Angular) How will we communicate between components? What lazy loads? Visual structure

### 9 Shared Functionality
Are we using 3rd party products? Do we need a wrapper around the 3rd party products so that we can easily replace them with another down the road? Is the shared functionality shareable in the 1 app or can it also be shared with other apps?

## Official (and unofficial) guides
Follow guides but note things that will be tweaked

#### Angular
[Style best practices](https://angular.io/guide/styleguide)

#### C#
[Coding conventions](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/inside-a-program/coding-conventions)

#### ASP.NET
[What and what not to do](https://docs.microsoft.com/en-us/aspnet/aspnet/overview/web-development-best-practices/what-not-to-do-in-aspnet-and-what-to-do-instead)
[Performance best practices](https://docs.microsoft.com/en-us/aspnet/core/performance/performance-best-practices?view=aspnetcore-3.0)

#### .NET
[Guides on microservices, DevOps, modernizing, Azure CloudApps, ASP.NET web apps, mobile apps, and UWP desktop apps](https://dotnet.microsoft.com/learn/dotnet/architecture-guides)
[(Unofficial) Best Practices As Specified By .NET Design Guidelines](https://www.c-sharpcorner.com/blogs/best-practices-as-specified-by-net-design-guidelines)
