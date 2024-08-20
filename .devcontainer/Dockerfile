# Use a base image
FROM mcr.microsoft.com/vscode/devcontainers/base:ubuntu

# Install prerequisites
RUN apt-get update && apt-get install -y \
    curl \
    && rm -rf /var/lib/apt/lists/*

# Install arduino-cli
RUN curl -fsSL https://raw.githubusercontent.com/arduino/arduino-cli/master/install.sh | sh

# Optionally, set the PATH
ENV PATH="/root/.arduino15/bin:${PATH}"
