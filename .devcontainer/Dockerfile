FROM wpilib/roborio-cross-ubuntu:2024-22.04

ARG USERNAME=parts
ARG USER_UID=1000
ARG USER_GID=$USER_UID

# Create the user
RUN groupadd --gid $USER_GID $USERNAME \
    && useradd --uid $USER_UID --gid $USER_GID -m --shell /usr/bin/bash $USERNAME

# Set the default user
USER $USERNAME