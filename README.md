# Cross-Origin Resource Sharing (CORS)

## Same-Origin Policy (SOP):
It is a security mechanism that is enforced by browsers to control access to data between the web applications.

It does not prevent writing between web applications, it prevents reading between applications.

Access is determined based on the origin.

## What is Origin?

Origin is defined with the combination of scheme(protocol), hostname(domain name) and port of the url used to access it.

eg: http://rudrayesh.com:80
Here 'http' is scheme, 'rudrayesh.com' is the domain name, port is '80'.

## Cross-Origin Resource Sharing(CORS):
It is a mechanism that uses HTTP headers to define Origins that the browser permits loading resources

CORS uses 2 HTTP headers
1. Access-Control-Allow-Origin
2. Access-Control-Allow-Credentials

### Access-Control-Allow-Origin:
This response header indicates that whether the response can be shared with the requesting code from the given origin.

### Syntax:
Access-Control-Allow-Origin: *

Access-Control-Allow-Origin: < origin >

Access-Control-Allow-Origin: null

## Note: 
Access-Control-Allow-Origin it allows us to access only public pages in the application, in order to access authenticated pages we need to use Access-Control-Allow-Credentials header.

### Access-Control-Allow-Credentials:
This response header allows cookies (or other user credentials) to be included in cross-origin requests.

### Syntax:
Access-Control-Allow-Credentials: true

## Note:
If the server is configured with wildcard character ("*") as the value of Access-Control-Allow-Origin header, then the use of credentials is not allowed.
