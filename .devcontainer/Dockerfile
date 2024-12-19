# Use Default Linux Universal Image
FROM mcr.microsoft.com/vscode/devcontainers/base:ubuntu-22.04

# Installs Node.js and npm
RUN apt-get update && apt-get install -y \
    python3 \
    python3-pip \
    npm \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

# Installs Flask
RUN pip3 install flask

# Installs Vue.js
RUN npm install -g @vue/cli

# Sets working directory
WORKDIR /workspace
