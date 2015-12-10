Repository for EventStore (geteventstore.com)

1. Download and run the image `docker run -d -p 2113:2113 -p 1113:1113 adbrowne/eventstore`
2. Open Docker and find the ip of your Virtual Box `docker-machine ls`
```
NAME      ACTIVE   DRIVER       STATE     URL                         SWARM   ERRORS
default   *        virtualbox   Running   tcp://192.168.99.100:2376
```
3. Enter the url you found with the geteventstore port like this `http://192.168.99.100:2113/web/index.html`
4. Enter username `admin` and password `changeit`