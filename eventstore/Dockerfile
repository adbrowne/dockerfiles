# EventStore (geteventstore.com)
#
# VERSION               0.0.2

FROM      ubuntu
MAINTAINER Andrew Browne <brownie@brownie.com.au>

ENV ES_VERSION 3.2.0

RUN apt-get update && apt-get install -y curl
RUN curl http://download.geteventstore.com/binaries/EventStore-OSS-Ubuntu-v$ES_VERSION.tar.gz | tar xz -C /opt

EXPOSE 2113
EXPOSE 1113

VOLUME /data/db
VOLUME /data/logs

ENV EVENTSTORE_MAX_MEM_TABLE_SIZE 100000
ENV EVENTSTORE_WORKER_THREADS 12

WORKDIR /opt/EventStore-OSS-Ubuntu-v$ES_VERSION

CMD ./run-node.sh --ext-http-prefixes=http://*:2113/ --ext-ip=0.0.0.0 \
    --db /data/db --log /data/logs --run-projections=all
