FROM node:20.12.2-bookworm-slim 

# Install necessary packages
RUN apt-get update && apt-get install -y --no-install-recommends \
    curl \
    wget \
    tar \
    gzip \
    git \
    ca-certificates \
    openssh-client \  
    && npm install -g pnpm \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# Create necessary directories and set permissions
RUN mkdir -p /app \
    && chown -R node:node /app \
    && mkdir -p /home/node/.ssh \
    && chmod 700 /home/node/.ssh \
    && chown -R node:node /home/node/.ssh \
    # Create directory for SSH agent socket
    && mkdir -p /ssh-agent \
    && chown -R node:node /ssh-agent \
    && chmod 700 /ssh-agent

# Add known hosts for GitHub
RUN ssh-keyscan -t rsa github.com >> /home/node/.ssh/known_hosts \
    && chown node:node /home/node/.ssh/known_hosts \
    && chmod 644 /home/node/.ssh/known_hosts

# Switch to non-root user
USER node

# Set working directory
WORKDIR /app

# Set host environment variable
ENV HOST=0.0.0.0