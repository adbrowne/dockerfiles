Repository for EventStore (geteventstore.com)

Will expose port *2114* (not 2113 as this is bound to localhost and I haven't worked out how to get eventstore and mono to expose
this as well has http://*:2113/).

To run you probably want something like this:

docker run -d -p 2114:2114 -p 1113:1113 adbrowne/eventstore

Then to use the Web UI: http://192.168.59.103:2114/web/index.html

Note that 192.168.59.103 might be different on your machine. If it is try: boot2docker ip to find out what IP your docker is using.
