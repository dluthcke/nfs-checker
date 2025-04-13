# NFS Docker CI

A Docker Compose setup with `nfs-checker` to verify NFS shares and an `app` running `hello-world`.

## Structure

- `nfs-checker/Dockerfile`: Builds `nfs-checker`.
- `nfs-checker/entrypoint.sh`: Verifies NFS shares.
- `docker-compose.yml`: Defines services.
- `.github/workflows/ci.yml`: CI pipeline.
- `README.md`: This file.

## Local Setup

1. **Build**:
   ```bash
   cd nfs-checker
   docker build -t nfs-checker:latest .
   cd ..
