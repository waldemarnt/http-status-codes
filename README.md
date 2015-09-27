# Http Status Codes 

> Useful informations about each kind of http code

*Inspired by the awesome lists*


## List of codes

The list is separated by kind.

### Informational 1xx
- [100](http://httpstatus.es/100) - Continue - Client should continue with request.
- [101](http://httpstatus.es/101) - Switching Protocols - Server is switching protocols.
- [102](http://httpstatus.es/102) - Processing - Server has received and is processing the request.
- [103](http://httpstatus.es/102) - Processing - Server has received and is processing the request.
- [122](http://httpstatus.es/102) - Request-uri too long - URI is longer than a maximum of 2083 characters.

### Success 2xx
These codes indicate success. The body section if present is the object returned by the request. It is a MIME format object. It is in MIME format, and may only be in text/plain, text/html or one fo the formats specified as acceptable in the request.

- [200](http://httpstatus.es/200) - Ok - The request was fulfilled.
- [201](http://httpstatus.es/201) - Created - Following a POST command, this indicates success, but the textual part of the response line indicates the URI by which the newly created document should be known.
- [202](http://httpstatus.es/202) - Accepted - The request has been accepted for processing, but the processing has not been completed. The request may or may not eventually be acted upon, as it may be disallowed when processing actually takes place. there is no facility for status returns from asynchronous operations such as this.
- [203](http://httpstatus.es/203) - Partial Information - When received in the response to a GET command, this indicates that the returned metainformation is not a definitive set of the object from a server with a copy of the object, but is from a private overlaid web. This may include annotation information about the object, for example.
- [204](http://httpstatus.es/204) - No Response - Server has received the request but there is no information to send back, and the client should stay in the same document view. This is mainly to allow input for scripts without changing the document at the same time.
- [205](http://httpstatus.es/205) - Reset Content - Request processed, no content returned, reset document view.
- [206](http://httpstatus.es/206) - Partial Content - partial resource return due to request header.
- [207](http://httpstatus.es/207) - Multi-Status - XML, can contain multiple separate responses.
- [208](http://httpstatus.es/208) - Already Reported - results previously returned.
- [226](http://httpstatus.es/226) - Im Used - request fulfilled, reponse is instance-manipulations.

### Redirection 3xx
The codes in this section indicate action to be taken (normally automatically) by the client in order to fulfill the request.

- [301](http://httpstatus.es/301) - Moved - The data requested has been assigned a new URI, the change is permanent. (N.B. this is an optimisation, which must, pragmatically, be included in this definition. Browsers with link editing capabiliy should automatically relink to the new reference, where possible)
- [302](http://httpstatus.es/302) - Found - The data requested actually resides under a different URL, however, the redirection may be altered on occasion (when making links to these kinds of document, the browser should default to using the Udi of the redirection document, but have the option of linking to the final document) as for "Forward".
- [303](http://httpstatus.es/303) - Method - Like the found response, this suggests that the client go try another network address. In this case, a different method may be used too, rather than GET.
- [304](http://httpstatus.es/304) - Not Modified - If the client has done a conditional GET and access is allowed, but the document has not been modified since the date and time specified in If-Modified-Since field, the server responds with a 304 status code and does not send the document body to the client.
- [305](http://httpstatus.es/305) - Use Proxy - Content located elsewhere, retrieve from there.
- [306](http://httpstatus.es/306) - Switch Proxy - Subsequent requests should use the specified proxy.
- [307](http://httpstatus.es/307) - Temporary Redirect - Connect again to different URI as provided.
- [308](http://httpstatus.es/308) - Permanent Redirect - Connect again to a different URI using the same method.

### Client side errors 4xx
The 4xx codes are intended for cases in which the client seems to have erred, and the 5xx codes for the cases in which the server is aware that the server has erred. It is impossible to distinguish these cases in general, so the difference is only informational.

The body section may contain a document describing the error in human readable form. The document is in MIME format, and may only be in text/plain, text/html or one for the formats specified as acceptable in the request.

- [400](http://httpstatus.es/400) - Bad Request - The request had bad syntax or was inherently impossible to be satisfied.
- [401](http://httpstatus.es/401) - Unauthorized - The parameter to this message gives a specification of authorization schemes which are acceptable. The client should retry the request with a suitable [Authorization](http://www.w3.org/Protocols/HTTP/HTRQ_Headers.html#z9) header.
- [402](http://httpstatus.es/402) - Payment Required - The parameter to this message gives a specification of charging schemes acceptable. The client may retry the request with a suitable ChargeTo header.
- [403](http://httpstatus.es/403) - Forbidden - The request is for something forbidden. Authorization will not help.
- [404](http://httpstatus.es/404) - Not Found - The server has not found anything matching the URI given.

### Server side error 5xx
- [500](http://httpstatus.es/500) - Internal Error - The server encountered an unexpected condition which prevented it from fulfilling the request.
- [501](http://httpstatus.es/501) - Not Implemented - The server does not support the facility required.
- [502](http://httpstatus.es/502) - Service temporarily overloaded - The server cannot process the request due to a high load (whether HTTP servicing or other requests). The implication is that this is a temporary condition which maybe alleviated at other times.
- [503](http://httpstatus.es/503) - Gateway timeout - This is equivalent to Internal Error 500, but in the case of a server which is in turn accessing some other service, this indicates that the respose from the other service did not return within a time that the gateway was prepared to wait. As from the point of view of the clientand the HTTP transaction the other service is hidden within the server, this maybe treated identically to Internal error 500, but has more diagnostic value.



## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.


## License

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Sindre Sorhus](http://sindresorhus.com) has waived all copyright and related or neighboring rights to this work.
