# Class 08 Reading Notes *(11/15/22)*

[*back*](../README.md)

## API Design Best Practices

1. REST is an architectural style for building distributed systems based on hypermedia
2. resources
3. a URI that uniquely identifies that resource <https://adventure-works.com/orders/1>
4. GET, POST, PUT, PATCH, and DELETE.
5. chatt api talks alot
6. <https://adventure-works.com/orders>
7. the more request to a api the more chatty it is. this can cause overloads.
8. retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource.
9. creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources.
10. either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated.
11. emoves the resource at the specified URI.
