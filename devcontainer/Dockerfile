FROM ubuntu:24.04

RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true \
    && apt-get -q update \
    && apt-get -q install -y gpg curl
RUN curl -O https://download.swift.org/swiftly/linux/swiftly-$(uname -m).tar.gz
RUN tar zxf swiftly-$(uname -m).tar.gz
# Add in the dependencies that Swiftly requires/suggests
RUN apt-get -q install -y \
      binutils \
      git \
      unzip \
      gnupg2 \
      libc6-dev \
      libcurl4-openssl-dev \
      libedit2 \
      libgcc-13-dev \
      libpython3-dev \
      libstdc++-13-dev \
      libxml2-dev \
      libncurses-dev \
      libz3-dev \
      pkg-config \
      tzdata \
      zlib1g-dev
# Add in some additional useful dependencies for development
RUN apt-get -q install -y \
      sqlite3 \
      libsqlite3-dev \
      libncurses5-dev \
      python3 \
      build-essential
# Switch to the ubuntu user to set up swiftly for its use
USER ubuntu
RUN /swiftly init --assume-yes --quiet-shell-followup
RUN echo "if [ -f ~/.local/share/swiftly/env.sh ]; then" >> ~/.bashrc
RUN echo "  . ~/.local/share/swiftly/env.sh" >> ~/.bashrc
RUN echo "fi" >> ~/.bashrc

# docker build -f Dockerfile-swiftly -t check .
# docker run --rm -it check bash