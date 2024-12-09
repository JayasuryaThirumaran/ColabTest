# Use an official lightweight Python image
FROM mcr.microsoft.com/devcontainers/python:3.10

# Install necessary tools
RUN apt-get update && apt-get install -y \
    curl \
    git \
    && apt-get clean

# Install Jupyter Notebook and other Python dependencies
RUN pip install --no-cache-dir \
    jupyter \
    notebook \
    colabcode

# Set workspace directory
WORKDIR /workspaces

# Expose the Jupyter port
EXPOSE 8888
