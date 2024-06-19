<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [HTTP response status codes](#http-response-status-codes)
  - [Information responses](#information-responses)
  - [Successful responses](#successful-responses)
  - [Redirection messages](#redirection-messages)
  - [Client error responses](#client-error-responses)
  - [Server error responses](#server-error-responses)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# HTTP response status codes

## Information responses

**100 Continue:** Client should continue with the request or ignore if already complete.

**101 Switching Protocols:** Server is switching to the protocol specified by the client.

**102 Processing (WebDAV):**  Server is processing the request, but no response is ready yet.

**103 Early Hints:** Allows the user agent to preload resources or preconnect while the server prepares the response.

## Successful responses

**200 OK:** Request succeeded, with response depending on the HTTP method used.

**201 Created:** Request succeeded, and a new resource was created.

**202 Accepted:** Request received but not yet acted upon.

**203 Non-Authoritative Information:** Metadata returned is from a copy, not the origin server.

**204 No Content:** No content to send, but headers may be useful.

**205 Reset Content:** Instructs the user agent to reset the document.

**206 Partial Content:** Only part of the resource is returned as requested by the client.

**207 Multi-Status (WebDAV):** Conveys multiple resource statuses.

**208 Already Reported (WebDAV):** Avoids repeating internal member listings in a collection.

**226 IM Used:** GET request fulfilled with instance-manipulated response.

## Redirection messages
**300 Multiple Choices:** Multiple possible responses; user or agent should choose one.

**301 Moved Permanently:** Resource URL permanently changed; new URL provided.

**302 Found:** Resource URL temporarily changed; use the same URL for future requests.

**303 See Other:** Retrieve the resource using a GET request at another URI.
**304 Not Modified:** Resource not modified; use cached version.

**305 Use Proxy (Deprecated):** Resource must be accessed through a proxy; deprecated.

**306 Unused:** Reserved, no longer used.

**307 Temporary Redirect:** Resource temporarily at another URI; same method must be used.

**308 Permanent Redirect:** Resource permanently at another URI; same method must be used.

## Client error responses
**400 Bad Request:** The server cannot process the request due to client error.

**401 Unauthorized:** The client must authenticate to get the requested response.

**402 Payment Required:** Reserved for future use, rarely used.

**403 Forbidden:** The client does not have access rights to the content.

**404 Not Found:** The server cannot find the requested resource.

**405 Method Not Allowed:** The request method is not supported by the target resource.

**406 Not Acceptable:** No content matches the user agent’s criteria.

**407 Proxy Authentication Required:** Authentication with a proxy is needed.

**408 Request Timeout:** The server timed out waiting for the request.

**409 Conflict:** The request conflicts with the server's current state.

**410 Gone:** The content has been permanently deleted from the server.

**411 Length Required:** The server requires the Content-Length header field.

**412 Precondition Failed:** The server does not meet the preconditions set by the client.

**413 Payload Too Large:** The request entity is too large.

**414 URI Too Long:** The requested URI is too long for the server to interpret.

**415 Unsupported Media Type:** The media format is not supported.

**416 Range Not Satisfiable:** The specified range cannot be fulfilled.

**417 Expectation Failed:** The expectation indicated in the request header cannot be met.

**418 I'm a teapot:** A humorous response code indicating the server refuses to brew coffee.

**421 Misdirected Request:** The request was directed at an inappropriate server.

**422 Unprocessable Content (WebDAV):** The request is well-formed but cannot be processed due to semantic errors.

**423 Locked (WebDAV):** The resource is locked.

**424 Failed Dependency (WebDAV):** The request failed due to the failure of a previous request.

**425 Too Early:** The server is unwilling to process the request to prevent replay attacks.

**426 Upgrade Required:** The client needs to upgrade to a different protocol.

**428 Precondition Required:** The request must be conditional to prevent conflicts.

**429 Too Many Requests:** The client has sent too many requests in a given time period.

**431 Request Header Fields Too Large:** The request headers are too large.

**451 Unavailable For Legal Reasons:** The resource is unavailable due to legal restrictions.

## Server error responses
**500 Internal Server Error:** The server encountered an unknown error.

**501 Not Implemented:** The request method is not supported by the server.

**502 Bad Gateway:** The server received an invalid response while acting as a gateway.

**503 Service Unavailable:** The server is not ready to handle the request, often due to maintenance or overload.

**504 Gateway Timeout:** The server, acting as a gateway, did not get a response in time.

**505 HTTP Version Not Supported:** The HTTP version used in the request is not supported.

**506 Variant Also Negotiates:** Internal server configuration error related to content negotiation.

**507 Insufficient Storage (WebDAV):** The server cannot store the representation to complete the request.

**508 Loop Detected (WebDAV):** The server detected an infinite loop while processing the request.

**510 Not Extended:** Further extensions to the request are needed for fulfillment.

**511 Network Authentication Required:** The client needs to authenticate to gain network access.





