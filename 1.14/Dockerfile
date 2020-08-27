FROM cimg/base:stable

RUN sudo apt-get update && sudo apt-get install -y \
        bison \
        llvm \
        zlib1g-dev \
        xz-utils && \
    sudo rm -rf /var/lib/apt/lists/*

ENV GO_VERSION=1.14.1

RUN curl -sSL "https://golang.org/dl/go${GO_VERSION}.linux-amd64.tar.gz" | \
    sudo tar -xz -C /usr/local/
