ARG SWIFT_VERSION=6.2
FROM swift:${SWIFT_VERSION}

RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true \
    && apt-get -q update \
    && apt-get -q dist-upgrade -y \
    && apt-get -q install -y \
      curl \
      sqlite3 \
      libsqlite3-dev \
      libncurses5-dev \
      python3 \
      build-essential
