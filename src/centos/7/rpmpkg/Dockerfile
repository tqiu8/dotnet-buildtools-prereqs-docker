FROM mcr.microsoft.com/dotnet-buildtools/prereqs:centos-7

# Install the rpm packaging toolchain required to build rpms
RUN yum clean all \
    && yum install -y \
        gcc \
        rpm-build \
        ruby-devel \
        rubygems \
    && gem install --no-document fpm \
    && yum clean all

