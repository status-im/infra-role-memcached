# Description

This role installs and configures [memcached](https://memcached.org/) service.

# Configuration

The defaults are sane, but the basics would be:
```yaml
memcached_addr: '127.0.0.1'
memcached_port: 11211
memcached_size_mb: 64
memcached_maxconn: 1024
```
