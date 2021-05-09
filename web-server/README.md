# Building a Web Server from scratch

## Based on a serie from the [Ruslan's Blog](https://ruslanspivak.com/lsbaws-part1/)

## Steps WSGI web server

1. Loads the *application* callable provided by your framework
2. The server reads the request from the client
3. The server parses the request
4. The server creates a dictionary of variables using the request data
5. The server calls the *application* callable and passes to it the dictionary and the *start_response*
6. The application sends back the response body to the web server
7. The server assembles an HTTP response using the date returned by the app.
8. The server transmits the HTTP response back to the client