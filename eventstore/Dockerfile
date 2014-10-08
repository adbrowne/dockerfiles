# EventStore (geteventstore.com)
#
# VERSION               0.0.1

FROM      ubuntu
MAINTAINER Andrew Browne <brownie@brownie.com.au>

RUN apt-get update && apt-get install -y curl

RUN curl http://download.geteventstore.com/binaries/EventStore-OSS-Linux-v3.0.0.tar.gz | tar xz -C /opt

EXPOSE 2114

COMMAND cd /opt/EventStore-OSS-Linux-v3.0.0; ./run-node.sh --http-prefixes=http://*:2114/
