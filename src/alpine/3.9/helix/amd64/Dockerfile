FROM python:2.7.15-alpine3.9

# Install .NET Core Dependencies for Alpine

RUN apk update && \
    apk add --no-cache \
        autoconf \
        bash \
        build-base \
        clang \
        clang-dev \
        cmake \
        coreutils \
        gcc \
        gettext-dev \
        git \
        icu-dev \
        iputils \
        krb5-dev \
        libtool \
        libunwind-dev \
        libffi \
        libffi-dev \
        linux-headers \
        llvm \
        make \
        openssl \
        openssl-dev \
        paxctl \
        py-cffi \
        python \
        python-dev \
        sudo \
        tzdata \
        util-linux-dev \
        wget \
        zlib-dev && \
    apk -X http://dl-cdn.alpinelinux.org/alpine/edge/main add --no-cache \
        userspace-rcu-dev \
        lttng-ust-dev 

# Install Helix Dependencies

RUN python -m pip install --upgrade pip==19.0.2 && \
    python -m pip install \ 
                  applicationinsights==0.11.7 \
                  certifi==2018.11.29 \
                  cryptography==2.5 \                  
                  docker==3.6.0 \
                  ndg-httpsclient==0.5.1  \
                  psutil==5.4.8 \
                  pyasn1==0.4.5 \
                  pyopenssl==18.0.0 \
                  requests==2.21.0 \
                  six==1.12.0 \
                  virtualenv==16.2.0
