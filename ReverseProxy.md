# Reverse Proxy 101

## What is a Reverse Proxy?
A reverse proxy is a server that sits between client devices (like browsers) and web servers. It manages client requests to backend servers and returns the server's response to the clients.

### Key functions of a reverse proxy:
- **Improved Security**: Acts as a barrier between client devices and backend servers, protecting the internal infrastructure.
- **Load balancing**: Distributes client requests to multiple backend servers to balance the load and prevent any single server from becoming overwhelmed.
- **Caching**: Caches content from backend servers to reduce load and improve performance.
- **SSL termination**: Handles SSL encryption/decryption on behalf of backend servers, simplifying secure connections.

### Reverse Proxy Diagram
<img src="https://www.avast.com/hs-fs/hubfs/New_Avast_Academy/What%20is%20reversed%20proxy/What_is_Reverse_Proxy_Server.png?width=660&name=What_is_Reverse_Proxy_Server.png" width="800" height="300" />

## Why Implement a Reverse Proxy?

1. **Improved Security**:
   - The reverse proxy can hide the identities and internal structure of your backend servers.
   - Protects servers from direct internet exposure, reducing the risk of attacks.
2. **Load Balancing**:
   - Distributes traffic evenly across multiple backend servers, preventing any one server from becoming overloaded.
   - Enhances scalability by allowing more servers to be added as traffic increases.
3. **Caching**:
   - Reduces server load and improves response time by caching static content and frequently requested resources.
4. **Centralized Authentication and SSL Termination**:
   - Handles authentication for multiple backend servers in one place.
   - SSL termination allows the reverse proxy to decrypt secure traffic, passing unencrypted traffic to the backend servers.

## Difference to a Forward Proxy
Unlike a forward proxy that forwards requests on behalf of clients to external resources, a reverse proxy works on behalf of servers to handle incoming client requests.
A forward proxy and a reverse proxy both act as intermediaries between clients and servers, but they serve different purposes and are positioned differently in the network.
###  Example Scenarios

#### **Forward Proxy Example**
A user in China wants to access YouTube (which is blocked). They use a forward proxy (VPN) to mask their identity and bypass restrictions.

#### **Reverse Proxy Example**
A website with high traffic (e.g., Amazon) uses an Nginx reverse proxy to distribute user requests across multiple servers, enhancing performance and security.

Forward Proxy = Protects and hides clients (users) from the internet.

Reverse Proxy = Protects and manages servers from external requests.
![Forward Proxy vs Reverse Proxy](https://www.indusface.com/wp-content/uploads/2023/04/Forward-proxy-vs-reverse-proxy-1.png)