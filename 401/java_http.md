# read 09

## Review: High-level HTTP

What are the five steps in the HTTP Request Lifecycle?

1. Local Processing
2. Resolve an IP
3. Establish a TCP Connection
4. Send an HTTP Request
5. Tearing Down and Cleaning Up

What are the two things the client needs before it can make an HTTP Request?

1. URL/IP
2. HTTP Method

Explain the four way handshake and what it does.

Step 1: Client sends a SYN (Synchronize) packet:

> The client initiates the active open by sending a SYN7 "control"8 packet to the server. The client sets the sequence number for the first packet to a random value purposely, in service of security. We’ll refer to this number as x for now.

Step 2: Server sends a SYN-ACK (Synchronize-Acknowledge) packet:

> The server responds with a SYN-ACK9 message, which contains an acknowledgement number for the original message that is always x+1, and a new sequence number for the response itself, which is another random number y.

Step 3: Client sends an ACK (Acknowledge) packet:

> In the third step, the client sends an ACK10 message back to the server with a sequence number equal to x+1, which should match the SYN-ACK message’s acknowledgment number and ensure that our data is being delivered reliably. The ACK message’s acknowledgment number (since it is acknowledging the SYN-ACK) is set to one more than the received sequence number, or y+1.

Step 4: Termination:

When Client or server side wants to close down the connection, it sends a FIN packet (finish) to the other side. The recipient of the packet acknowledges with an ACK, then sends it's FIN packet for termination.

## Java HTTP Request example

True or False: When making an HTTP request, you MUST follow any redirect returned by the request. Back up your answer.

False, it is not mandotory to follow a redirect. It depends on the nature of the request and the requirements of the client application. HTTP gives out status codes to indicate wheter a redirect is required.

Which built-in Java class can be used to perform an HTTP request?

`HttpURLConnection` which is part of the `java.net` package.

What HTTP status codes represent a successful response? A redirect? A client error?

successful response: (200)

* 200: OK
* 201: Created
* 204: No Content

redirect: (300)

* 301: Moved Permanently
* 302: Found
* 307: Temporary Redirect

client error: (400)

* 400: Bad Request
* 401: Unauthorized
* 404: Not Found

## Things I want to know more about

## References

[High-level HTTP](https://dev.to/dangolant/things-i-brushed-up-on-this-week-the-http-request-lifecycle-)

[Java HTTP Request](https://www.baeldung.com/java-http-request)
