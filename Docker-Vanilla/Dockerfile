FROM ghcr.io/linuxserver/code-server:latest

RUN \
  echo "**** install build dependencies ****" && \
  apt-get update && \
  apt-get install -y \
    gnupg \
    build-essential \
    libx11-dev \
    libxkbfile-dev \
    libsecret-1-dev \
    pkg-config && \
  echo "**** install runtime ****" && \
  apt-get install -y \ 
    htop \
    default-jre && \
  echo "**** clean up ****" && \
  apt-get clean && \
  rm -rf \
    /tmp/* \
    /var/lib/apt/lists/* \
    /var/tmp/*
