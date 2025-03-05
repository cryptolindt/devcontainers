# Use the official image as a parent image
ARG VARIANT="bullseye"
FROM mcr.microsoft.com/devcontainers/base:${VARIANT}

# Install additional packages
# RUN apt-get update && apt-get install -y \
#     curl \
#     git \
#     && apt-get clean -y && rm -rf /var/lib/apt/lists/*

# Set the default shell to bash
# SHELL ["/bin/bash", "-c"]

# Set up a non-root user for the container
# ARG USERNAME=vscode
# ARG USER_UID=1000
# ARG USER_GID=$USER_UID

# RUN groupadd --gid $USER_GID $USERNAME \
#     && useradd --uid $USER_UID --gid $USER_GID -m $USERNAME \
#     && apt-get update && apt-get install -y sudo \
#     && echo $USERNAME ALL=\(ALL\) NOPASSWD:ALL > /etc/sudoers.d/$USERNAME \
#     && chmod 0440 /etc/sudoers.d/$USERNAME

# Switch to the non-root user
USER $USERNAME

# Set the working directory
WORKDIR /workspace

# Expose port 3000
# EXPOSE 3000

# Command to run on container start
CMD ["sleep", "infinity"]