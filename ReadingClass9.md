# Reading Class 09
> What are the five steps in the HTTP Request Lifecycle?
- **Local Processing**: In this step, the browser processes the URL to extract the protocol, host, port (optional), resource path, and query strings. It also resolves the IP address of the host using various caches and the DNS server.

- **Resolve an IP**: The browser sends a DNS request to resolve the IP address of the host. If the cache lookup fails, it uses UDP to send the DNS request. The request travels through network devices, and the DNS server responds with the IP address or passes the request to another server recursively.

- **Establish a TCP Connection**: The client establishes a TCP connection with the server using a three-way handshake. This involves sending SYN, SYN-ACK, and ACK packets to ensure reliable and ordered data transmission.

- **Send an HTTP Request**: With the TCP connection established, the client sends an HTTP request containing a request line, headers, and an optional body. The request is sent over the established TCP connection.

- **Tearing Down and Cleaning Up**: Once the server processes the request, it sends an HTTP response back to the client over the established TCP connection. After the response is received, the TCP connection is torn down through a four-way handshake, and the client processes the response

> What are the two things the client needs before it can make an HTTP Request?

- **IP Address**: The client needs the IP address of the server it intends to communicate with. This IP address is obtained through a DNS (Domain Name System) resolution process, where the client's request is translated into an IP address that identifies the server on the network.

- **TCP Connection**: The client establishes a TCP (Transmission Control Protocol) connection with the server. This connection is necessary for reliable and ordered data transmission between the client and the server. The TCP connection ensures that data packets are delivered in the correct order and that acknowledgment mechanisms are in place for successful communication.

> Explain the four way handshake and what it does.

- **Client Sends FIN**: The client initiates the closing process by sending a FIN (Finish) packet to the server. This packet indicates that the client has finished sending data and wants to close the connection.

- **Server Acknowledges FIN**: Upon receiving the FIN packet from the client, the server acknowledges it by sending an ACK (Acknowledgment) packet back to the client. This ACK acknowledges the receipt of the FIN packet and confirms that the server is aware of the client's intention to close the connection.

- **Server Sends FIN**: After acknowledging the client's FIN packet, the server also initiates the closing process by sending its own FIN packet to the client. This indicates that the server has finished sending data and wants to close its end of the connection.

- **Client Acknowledges FIN**: Finally, upon receiving the server's FIN packet, the client sends an ACK packet back to the server to acknowledge the receipt. This confirms that the client is aware of the server's intention to close the connection.


> True or False: When making an HTTP request, you MUST follow any redirect returned by the request. Back up your answer.
- False. While it's a common practice to follow redirects when making HTTP requests, it's not an absolute requirement that you must follow every redirect returned by the request. Whether you should follow redirects depends on your specific use case and requirements.

>Which built-in Java class can be used to perform an HTTP request?

- The built-in Java class that can be used to perform an HTTP request is the HttpURLConnection class. 

> What HTTP status codes represent a successful response? A redirect? A client error?
- Successful Responses (2xx): 200 OK
- Redirection Responses(3xx): 301, 302, 303, 307
- Client Error Responses (4xx): 401, 400, 403, 404, 405, 409, 408