---
layout: post
title: Why do we have to use GraphQL?
description: >
  Compare GraphQL with RESTFUL APIs
image: /assets/img/blog/graphql.jpg
sitemap: false
---

When I created APIs in the last few years I always used RESTFUL APIs. Most companies still use RESTFUL APIs. In fact, even I was trying to write an article about RESTFUL APIs. These days most companies use GraphQL for their APIs. I also wanted to see how GraphQL is going to solve the problems we have.

This is the first article of the GraphQL series that I’m intending to write. In this article, I’m planning to compare GraphQL with RESTFUL API.

Before start the comparison, let’s talk about what GraphQL really is and where we can use it.
In a typical client-server architecture model, the client requests data from the server. A server returns a response.


![](/assets/img/blog/what_is_rest_api.png)

Instead of RESTFUL API client can use GraphQL to request data from the server. GraphQL stands for Graph Query Language. It provides only one endpoint to the client to fetch any data from the server. It’s very interesting, isn’t it? Because when we used RESTFUL APIs we had to use multiple endpoints to serve one page.

## What are the advantages of GraphQL?
- It’s fast
- It’s flexible
- It’s easy to use and easy to maintain

## What makes GraphQL faster than RESTFUL APIS?

In a RESTFUL API approach, we need to use multiple endpoints on a single page.

Eg: When we display an article page with comments, we need an endpoint like this to fetch an article
GET /posts/123123
and also endpoint like this

GET /posts/123123/comments to fetch comments. And also another endpoint to fetch Author’s details.

But if we use GraphQL we need to provide only one endpoint to the client. It’s simple as that. Since it doesn’t need multiple API calls, GraphQL becomes faster.
GraphQL endpoint will look like POST /graphql (Don’t worry about this endpoint name for the moment.)

## What makes GraphQL more flexible?

Unlike RESTFUL API, GraphQL can provide different data for different client interfaces. Let me elaborate on this using an example.

Eg: We don’t need to display the comments in the article on a mobile device unless the user really wants to see it. But on the desktop device, we can display the article with all the comments. To cater to this GraphQL can provide different data set to each device using the same endpoint.

I know some of you can say we can still achieve the same thing with RESTFUL API by providing query parameters. Absolutely you can. But it’s like trying to reinvent the thing that GraphQL has already done.


## What makes GraphQL easy to use and easy to maintain?
Since we have only one endpoint to use in GraphQL all it needs is to change the query string when it needs different data. How cool is that? That makes the frontend to use and maintain endpoints easier.

## Conclusion
I’m still a beginner at GraphQL. But I can see there are so many benefits that we can get from GraphQL. I’m planning to explore more on GraphQL and would love to share my learnings with you guys.
