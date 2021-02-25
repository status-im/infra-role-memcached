# Description

This role installs and configures [memcached](https://memcached.org/) and [memcached\_exporter]() services.

The exporter is available on port `9150` and the prometheus metrics can be fetched via the `/metrics` http endpoint:

```
curl 0.0.0.0:9150/metrics
```

# Configuration

The defaults are sane, but the basics would be:
```yaml
memcached_addr: '127.0.0.1'
memcached_port: 11211
memcached_size_mb: 64
memcached_maxconn: 1024
```

The installation of memcached\_exporter is optional. It is installed by default but can be disabled by setting:

```yaml
memcached_exporter_enabled: false
```
