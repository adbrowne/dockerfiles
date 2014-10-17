Repository for EventStore (geteventstore.com)

To run you probably want something like this:

docker run -d -p 2113:2113 -p 1113:1113 adbrowne/eventstore

Then to use the Web UI: http://192.168.59.103:2113/web/index.html

Note that 192.168.59.103 might be different on your machine. If it is try: boot2docker ip to find out what IP your docker is using.
