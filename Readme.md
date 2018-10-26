# Bookstack using kubernetes and docker-compose
## Bookstack using kubernetes

### Config

First step is to set environment variables. You can use secrets if you prefer. I recommend it.

If you have more than one service you can use an ingress.

You can set an external static IP in bookstack service with the next parameter:

```
type: LoadBalancer
loadBalancerIP: xx.xx.xx.xx
```

## Bookstack using docker-compose

You can change the routes of volumes, ports and environment variables as you wish.


Execute the next command to start docker-compose:

```
$ docker-compose up -d
```

## Bookstack default user

Default user: admin@admin.com \
Default pass: password

* You should delete default admin user and disabled guest user for security reasons.