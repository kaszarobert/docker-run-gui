# Use an Ubuntu base image
FROM ubuntu:latest

# Install required packages
RUN apt-get update && apt-get install -y \
    x11-apps \
    xauth \
    xserver-xorg-video-dummy \
    && rm -rf /var/lib/apt/lists/*

# Set the DISPLAY environment variable
ENV DISPLAY=:0

# Run a command to keep the container running forever
CMD ["tail", "-f", "/dev/null"]
