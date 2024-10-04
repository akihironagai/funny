# syntax=docker/dockerfile:1

# https://github.com/devcontainers/images/tree/main/src/cpp
FROM mcr.microsoft.com/devcontainers/cpp:ubuntu-24.04

# Environment variable VCPKG_FORCE_SYSTEM_BINARIES must be set on arm, s390x, ppc64le and riscv platforms.
ENV VCPKG_FORCE_SYSTEM_BINARIES=1

RUN apt-get update && apt-get install -y \
    clangd \
    ninja-build \
    && rm -rf /var/lib/apt/lists/*
