# Use an official Ubuntu as a base image
FROM ubuntu:20.04

# Set environment variables to avoid interaction during package installation
ENV DEBIAN_FRONTEND=noninteractive

# Update the package list and install basic utilities
RUN apt-get update && apt-get install -y \
    curl \
    vim \
    sudo \
    git \
    && rm -rf /var/lib/apt/lists/*

# Set the working directory
WORKDIR /app

# Copy a script or application file into the container (optional)
# COPY your_script.sh /app/your_script.sh

# Expose port 80 (optional, in case you run a web server or app that requires a port)
# EXPOSE 80

# Define the default command to run when the container starts
CMD ["bash"]
