# Prometheus Certificate Generation (Quick Guide for Programmers)

Generate self-signed certificates for Prometheus using OpenSSL in Git Bash. Ideal for local development and testing.

## Prerequisites

- **Git Bash:** Ensure you have Git Bash installed (comes with Git for Windows).
- **OpenSSL:** Git Bash usually includes OpenSSL. Verify with `openssl version`.

## Generate Certificates (Copy & Paste to Git Bash)

```bash
openssl req -new -newkey rsa:2048 -days 365 -nodes -x509 \
-keyout prometheus/certs/prometheus.key \
-out prometheus/certs/prometheus.crt
```
