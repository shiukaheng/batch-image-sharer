FROM ubuntu:20.04

# Install node.js and npm, flask, and python3
RUN apt-get update && apt-get install -y \
    curl \
    git \
    gnupg \
    nano \
    python3 \
    python3-pip \
    python3-venv \
    && curl -sL https://deb.nodesource.com/setup_16.x | bash - \
    && apt-get install -y nodejs \
    && pip3 install flask

# Install pdm
RUN pip3 install pdm

# CD to the ~/workspace directory and run npm install and pdm install
WORKDIR /root/workspace
# RUN npm install
# RUN pdm install