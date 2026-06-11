FROM mcr.microsoft.com/devcontainers/base:ubuntu

# Switch to root to install packages
USER root

# Download and install Google Chrome
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
  && wget -q https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb \
  && apt-get install -y ./google-chrome-stable_current_amd64.deb \
  && rm google-chrome-stable_current_amd64.deb
