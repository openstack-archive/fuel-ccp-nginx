These files demonstrate the architecture of nginx proxy, which is used in
other services with enabled TLS.

- upstreams.conf.j2 contains information about all endpoint behind nginx proxy.
  There is one instance of this file should be each repository.
- servers.conf.j2 contains proxy configuration, i.e. which address:port
  should be listen, options for SSL, HTTP headers and destination endpoint.
