FROM ruby:2.6.3-buster

# Point APT sources to the archived repository for Debian Buster
RUN echo "deb http://archive.debian.org/debian buster main" > /etc/apt/sources.list && \
    echo "deb http://archive.debian.org/debian-security buster/updates main" >> /etc/apt/sources.list && \
    apt-get update -qq && apt-get install -y --no-install-recommends \
    build-essential \
    libpq-dev \
    nodejs \
    npm \
    git \
    curl

# Install Yarn
RUN npm install -g yarn

WORKDIR /workspace

CMD ["sleep", "infinity"]