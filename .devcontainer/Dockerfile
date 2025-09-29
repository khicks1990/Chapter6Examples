# Start from the universal image
FROM mcr.microsoft.com/devcontainers/java:1-21


# Install openbox
RUN apt-get update && \
    DEBIAN_FRONTEND=noninteractive apt-get -y install --no-install-recommends openbox && \
    apt-get clean && rm -rf /var/lib/apt/lists/*

# Set openbox to start automatically
RUN echo 'openbox-session &' >> ~/.xinitrc
