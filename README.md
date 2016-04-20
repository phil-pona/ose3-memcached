# OpenShift Ruby Passenger Example

## How to Deploy

### Create New OpenShift Project
```
$ oc new-project example-ruby-passenger-helloworld
```

#### Create Application and expose Service
```
$ oc new-app https://github.com/phil-pona/ose3-memcached.git  --strategy=docker --name=memcached

$ oc expose service appuio-ruby-pass-ex
```

