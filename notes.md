Web Fundamentals and Burp Suite Setup

Overview

This session introduced the fundamentals of web communication and the use of Burp Suite with Firefox to inspect HTTP traffic in an authorized learning environment.

1. Burp Suite and Firefox Setup

I installed and configured Burp Suite to work with Firefox.

- Proxy address: "127.0.0.1"
- Proxy port: "8080"
- Certificate: Installed the Burp CA certificate in Firefox to support HTTPS inspection through the local proxy.

What I learned

Burp Suite acts as an intermediary between the browser and a web server. It allows me to inspect HTTP requests and responses and understand how browser-server communication works.

Safety note: Keep the proxy configuration limited to my intended testing browser and authorized lab environments. The Burp CA certificate should only be trusted where needed for testing.

2. Client and Server

- Client: The application requesting a resource, such as a web browser.
- Server: The system that receives requests and returns responses.

3. HTTP Requests and Responses

An HTTP request is sent by a client to a server. The server processes it and sends back an HTTP response.

GET

GET is commonly used to retrieve information from a server.

POST

POST is commonly used to submit data to a server, such as a form submission.

The exact behavior depends on the application and its implementation.

4. URL Structure

A URL can contain several components:

- Scheme: For example, "https"
- Host: The domain name
- Port: An optional network port
- Path: The requested resource
- Query string: Optional parameters following "?"

Example:

"https://example.com/products?id=10"

Here, "https" is the scheme, "example.com" is the host, "/products" is the path, and "id=10" is the query string.

5. Basic HTTP Flow

1. The user enters a URL or follows a link.
2. DNS resolution helps the client find the server's IP address.
3. The browser establishes the necessary network connection.
4. The browser sends an HTTP request.
5. The server processes the request and returns an HTTP response.
6. The browser displays the resulting content.

When a browser is configured to use Burp Suite, its HTTP traffic can pass through the local proxy for inspection.

6. DNS Fundamentals

The Domain Name System (DNS) helps translate domain names, such as "example.com", into IP addresses that clients can use to locate servers.

DNS resolution can involve caching and multiple DNS servers; the process does not always require a new lookup.

Key Takeaways

- How clients and servers communicate.
- The difference between HTTP requests and responses.
- Common uses of GET and POST.
- The basic components of a URL.
- How DNS helps resolve domain names to IP addresses.
- How Burp Suite can be used to inspect browser traffic.

Next Steps


- Inspect a normal request and response in Burp Suite.
- Identify the HTTP method, URL, status code, and response headers.
- Compare GET and POST requests in an authorized lab.
- Continue learning HTTP and web application security fundamentals.

Learning approach: Practice in authorized environments, document observations, and build understanding one concept at a time.
