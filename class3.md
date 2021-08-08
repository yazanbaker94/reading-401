What’s the difference between PUT and PATCH?

The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.
 <hr> <hr> <hr> <hr> <hr> <hr>
Provide links to 3 services or tools that allow you to “mock” an API for development like json-server

1. https://github.com/nock/nock
2. http://www.mock-server.com/
3. https://beeceptor.com/
 <hr> <hr> <hr> <hr> <hr> <hr>

Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

swagger:


                  '400':
                  description: Bad request. User ID must be an integer and larger than 0.
                '401':
                  description: Authorization information is missing or invalid.
                '404':
                  description: A user with the specified ID was not found.
                '5XX':
                  description: Unexpected error.
                  
                  
  apiDocs:
  
              	All parameters will be grouped by this name.
              Without a group, the default Error 4xx is set.
              You can set a title and description with @apiDefine.
              
              
 <hr> <hr> <hr> <hr> <hr> <hr>
              
SOAP :

                   301	Moved permanently	Server	The requested page has been permanently moved. The server automatically redirects the request to the new location.
                  304	Not Modified	Server	The server has decided, based on information in the request, that the requested data has not been modified since the last request and so it does not need to be sent again.
                  307	Temporary Redirect	Server	The requested page has been moved, but this change may not be permanent. The server automatically redirects the request to the new location.
                  400	Bad Request	Client.BadRequest	
                  The HTTP request is incomplete or malformed.

                  401	Authorization Required	Client.Authorization	
                  Authorization is required to use the service, but a valid user name and password were not supplied.

                  403	Forbidden	Client.Forbidden	
                  You do not have permission to access the database.

                  404	Not Found	Client.NotFound	
                  The named database is not running on the server, or the named web service does not exist.

                  408	Request Timeout	Server.RequestTimeout	
                  The maximum connection idle time was exceeded while receiving the request.

                  411	HTTP Length Required	Client.LengthRequired	The server requires that the client include a Content-Length specification in the request. This typically occurs when uploading data to the server.
                  413	Entity Too Large	Server	
                  The request exceeds the maximum permitted size.

                  414	URI Too Large	Server	
                  The length of the URI exceeds the maximum allowed length.

                  500	Internal Server Error	Server	
                  An internal error occurred. The request could not be processed.

                  501	Not Implemented	Server	
                  The HTTP request method is not GET, HEAD, or POST.

                  502	Bad Gateway	Server	The document requested resides on a third-party server and the server received an error from the third-party server.
                  503	Service Unavailable	Server	
                  The number of connections exceeds the allowed maximum.
                  
                  
   ReST:
   
   
           1xx: Informational – Communicates transfer protocol-level information.
        2xx: Success – Indicates that the client’s request was accepted successfully.
        3xx: Redirection – Indicates that the client must take some additional action in order to complete their request.
        4xx: Client Error – This category of error status codes points the finger at clients.
        5xx: Server Error – The server takes responsibility for these error status codes.
   


Term ---- 
Web Server - 
Definition: A web server is a computer that runs websites
Express - The primary use of Express is to provide server-side logic for web and mobile applications, and as such it's used all over the place
Routing - Routing is a process which is performed by layer 3 (or network layer) devices in order to deliver the packet by choosing an optimal path from one network to another.
WRRC - not known
