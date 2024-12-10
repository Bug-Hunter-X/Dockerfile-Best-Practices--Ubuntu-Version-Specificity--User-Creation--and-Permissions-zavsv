# Dockerfile Best Practices

This repository demonstrates a common error in Dockerfiles and shows how to fix it. The main issue involves using `ubuntu:latest`, missing user creation, and not setting correct file permissions.  This can lead to unexpected behavior and security vulnerabilities in production environments.

**Bug:**

The original Dockerfile uses `ubuntu:latest`, which is not best practice. Using a specific version is recommended for reproducibility and security.

**Solution:**

The solution provides a Dockerfile with a specific version of Ubuntu, creating a non-root user, and setting appropriate file permissions. This ensures better security and predictability. 