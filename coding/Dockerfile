# Coding Image

# Use ubuntu
FROM ubuntu
LABEL maintainer="Aaron Chan <zwchen037@gmail.com>"
ENV DEBIAN_FRONTEND=noninteractive

# Update and install various packages
RUN apt-get upgrade -y \
  && apt-get update -y \
  && apt-get install -y wget build-essential lsb-release locales bash-completion tzdata gettext-base curl git zip unzip python3 python3-pip perl fontconfig

# Use en utf8 locales
RUN locale-gen en_US.UTF-8
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8

# Remove apt lists (for storage efficiency)
RUN rm -rf /var/lib/apt/lists/*

CMD ["bash"]
