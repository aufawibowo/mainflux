aufawibowo@aufawibowo-VBox:~$ docker ps
CONTAINER ID        IMAGE                             COMMAND                  CREATED             STATUS              PORTS                                                                                                                               NAMES
fd5e6513db86        mainflux/influxdb-writer:latest   "/exe"                   19 minutes ago      Up 19 minutes       0.0.0.0:8900->8900/tcp                                                                                                              mainflux-influxdb-writer
ddd208253cd5        grafana/grafana:5.1.3             "/run.sh"                19 minutes ago      Up 19 minutes       0.0.0.0:3001->3000/tcp                                                                                                              mainflux-grafana
72f4b6f0860c        influxdb:1.6.4-alpine             "/entrypoint.sh infl…"   19 minutes ago      Up 19 minutes       0.0.0.0:8086->8086/tcp                                                                                                              mainflux-influxdb
6efefd8cffff        mainflux/influxdb-reader:latest   "/exe"                   19 minutes ago      Up 19 minutes       0.0.0.0:8905->8905/tcp                                                                                                              mainflux-influxdb-reader
40604a9e3e3f        mainflux/mongodb-writer:latest    "/exe"                   19 minutes ago      Up 19 minutes       0.0.0.0:8901->8901/tcp                                                                                                              mainflux-mongodb-writer
84cc223dbc71        mongo:3.6-jessie                  "docker-entrypoint.s…"   19 minutes ago      Up 19 minutes       0.0.0.0:27017->27017/tcp                                                                                                            mainflux-mongodb
8e6c2efeed02        mainflux/mongodb-reader:latest    "/exe"                   19 minutes ago      Up 19 minutes       0.0.0.0:8904->8904/tcp                                                                                                              mainflux-mongodb-reader
60e15cb42299        mainflux/mqtt:latest              "node mqtt.js"           19 minutes ago      Up 19 minutes       0.0.0.0:1883->1883/tcp, 0.0.0.0:8880->8880/tcp                                                                                      mainflux-mqtt
5761f8ffa0ac        mainflux/http:latest              "/exe"                   19 minutes ago      Up 19 minutes       0.0.0.0:8185->8185/tcp                                                                                                              mainflux-http
3d0bd9b90c67        mainflux/ws:latest                "/exe"                   19 minutes ago      Up 19 minutes       0.0.0.0:8186->8186/tcp                                                                                                              mainflux-ws
fa36c331731b        mainflux/coap:latest              "/exe"                   19 minutes ago      Up 19 minutes       0.0.0.0:5683->5683/tcp, 0.0.0.0:5683->5683/udp                                                                                      mainflux-coap
9a09e9828b42        mainflux/things:latest            "/exe"                   19 minutes ago      Up 19 minutes       0.0.0.0:8182-8183->8182-8183/tcp, 0.0.0.0:8989->8989/tcp                                                                            mainflux-things
3154c83c8736        mainflux/users:latest             "/exe"                   19 minutes ago      Up 19 minutes       0.0.0.0:8180->8180/tcp, 8181/tcp                                                                                                    mainflux-users
d198b0f88996        mainflux/normalizer:latest        "/exe"                   19 minutes ago      Up 19 minutes       0.0.0.0:8184->8184/tcp                                                                                                              mainflux-normalizer
9ae42344d58b        mainflux/ui:latest                "/entrypoint.sh"         20 minutes ago      Up 19 minutes       80/tcp, 0.0.0.0:3000->3000/tcp                                                                                                      mainflux-ui
ffc3197de37a        nats:1.3.0                        "/gnatsd -c gnatsd.c…"   20 minutes ago      Up 19 minutes       4222/tcp, 6222/tcp, 8222/tcp                                                                                                        mainflux-nats
36242f414ea9        postgres:10.8-alpine              "docker-entrypoint.s…"   20 minutes ago      Up 19 minutes       5432/tcp                                                                                                                            mainflux-users-db
63c9ec7195f5        redis:5.0-alpine                  "docker-entrypoint.s…"   20 minutes ago      Up 19 minutes       6379/tcp                                                                                                                            mainflux-es-redis
1e9e811e3035        jaegertracing/all-in-one:1.13     "/go/bin/all-in-one-…"   20 minutes ago      Up 19 minutes       5775/udp, 0.0.0.0:5778->5778/tcp, 0.0.0.0:14268->14268/tcp, 6832/udp, 0.0.0.0:16686->16686/tcp, 0.0.0.0:6831->6831/udp, 14250/tcp   mainflux-jaeger
ad04cc840c9e        redis:5.0-alpine                  "docker-entrypoint.s…"   20 minutes ago      Up 19 minutes       6379/tcp                                                                                                                            mainflux-things-redis
d50c1c3789fc        nginx:1.16.0-alpine               "/entrypoint.sh"         20 minutes ago      Up 19 minutes       0.0.0.0:80->80/tcp, 0.0.0.0:443->443/tcp, 0.0.0.0:8883->8883/tcp                                                                    mainflux-nginx
c73c05983efe        postgres:10.8-alpine              "docker-entrypoint.s…"   20 minutes ago      Up 19 minutes       5432/tcp                                                                                                                            mainflux-things-db
ecf630999f55        redis:5.0-alpine                  "docker-entrypoint.s…"   20 minutes ago      Up 19 minutes       6379/tcp                                                                                                                            mainflux-mqtt-redis


aufawibowo@aufawibowo-VBox:~/smartcampus-mainflux$ ./up
Creating mainflux-mqtt-redis   ... done
Creating mainflux-nginx        ... done
Creating mainflux-things-db    ... done
Creating mainflux-es-redis     ... done
Creating mainflux-users-db     ... done
Creating mainflux-things-redis ... done
Creating mainflux-jaeger       ... done
Creating mainflux-nats         ... done
Creating mainflux-ui           ... done
Creating mainflux-normalizer   ... done
Creating mainflux-users        ... done
Creating mainflux-things       ... done
Creating mainflux-ws           ... done
Creating mainflux-coap         ... done
Creating mainflux-http         ... done
Creating mainflux-mqtt         ... done
Creating mainflux-mongodb-reader ... done
Creating mainflux-mongodb ... done
Creating mainflux-mongodb-writer ... done
Creating mainflux-influxdb-reader ... done
Creating mainflux-influxdb ... done
Creating mainflux-grafana         ... done
Creating mainflux-influxdb-writer ... done

