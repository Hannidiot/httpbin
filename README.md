# httpbin(1): HTTP Request & Response Service


A [Kenneth Reitz](http://kennethreitz.org/bitcoin) Project.

![ice cream](http://farm1.staticflickr.com/572/32514669683_4daf2ab7bc_k_d.jpg)

Run locally:
```sh
docker pull kennethreitz/httpbin
docker run -p 80:80 kennethreitz/httpbin
```

See http://httpbin.org for more information.

## Functionality (gen by AI)

1. **HTTP Request Inspection**:
   - Returns data about the incoming HTTP request (e.g., headers, IP, method, path).
   - Endpoints like `/get`, `/post`, `/put`, `/delete` simulate different HTTP methods.

2. **Response Testing**:
   - Generates different HTTP responses (e.g., status codes, headers, body).
   - Examples:
     - `/status/{code}` – Returns a specific HTTP status code (e.g., `/status/404`).
     - `/response-headers` – Allows setting custom response headers.

3. **Authentication Testing**:
   - Supports testing Basic Auth (`/basic-auth/{user}/{passwd}`), Bearer Tokens, and Digest Auth.

4. **Dynamic Data Generation**:
   - `/uuid` – Generates a UUID.
   - `/bytes/{n}` – Returns `n` random bytes.
   - `/stream/{n}` – Streams `n` lines of JSON data.

5. **Cookies & Sessions**:
   - `/cookies` – Inspects sent cookies.
   - `/cookies/set` – Sets cookies.
   - `/cookies/delete` – Deletes cookies.

6. **Redirects**:
   - `/redirect/{n}` – Returns a `302` redirect `n` times.
   - `/relative-redirect/{n}` – Relative URL redirects.

7. **Delay Simulation**:
   - `/delay/{n}` – Delays response by `n` seconds (useful for timeout testing).

8. **IP & Geolocation**:
   - `/ip` – Returns the requester's IP address.
   - `/user-agent` – Returns the user-agent header.

9. **Image & Binary Data**:
   - `/image/png`, `/image/jpeg` – Returns sample images.
   - `/xml`, `/html` – Returns structured data formats.

10. **Request Echo**:
    - Echoes back request details (e.g., `/headers` shows request headers, `/anything` returns full request data).


## Officially Deployed at:

- http://httpbin.org
- https://httpbin.org
- https://hub.docker.com/r/kennethreitz/httpbin/


## SEE ALSO

- http://requestb.in
- http://python-requests.org
- https://grpcb.in/
