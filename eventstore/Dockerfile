# EventStore (geteventstore.com)
#
# VERSION               0.0.1

FROM      ubuntu
MAINTAINER Andrew Browne <brownie@brownie.com.au>

RUN apt-get update && apt-get install -y curl openssh-server

RUN curl http://download.geteventstore.com/binaries/EventStore-OSS-Linux-v3.0.0.tar.gz | tar xz -C /opt
