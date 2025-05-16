FROM ruby:3.1-bullseye

# Install required packages
RUN apt-get update && apt-get install -y \
    build-essential \
    git \
    && rm -rf /var/lib/apt/lists/*

# Set working directory
WORKDIR /workspace

SHELL ["/bin/bash", "-l", "-c"]

# Install Jekyll and Bundler
RUN gem install jekyll bundler