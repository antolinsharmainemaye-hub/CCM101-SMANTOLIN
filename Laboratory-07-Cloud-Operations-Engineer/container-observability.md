# Container Observability

## Application Logs

### 404 Error Log

```text
172.17.0.1 - - [10/Oct/2026:07:22:33 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"
```

### Importance of Application Logs

Application logs help identify errors and show which requests succeeded or failed. They make troubleshooting easier by providing details about user requests and helping engineers determine what went wrong.

## Container Metrics

- **Container Name:** client-website
- **Memory Usage:** 2.727 MiB
- **Memory Limit:** 1.859 GiB
- **CPU Usage:** 0.00%
- **Memory Percentage:** 0.14%
- **Network I/O:** 2.75 kB / 2.35 kB
- **Block I/O:** 0 B / 12.3 kB
- **PIDs:** 2