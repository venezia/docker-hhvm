
Public Repository is located [https://github.com/venezia/docker-hhvm](https://github.com/venezia/docker-hhvm)
Private Repository is located [https://stash.mtvi.com/projects/CRAB/repos/docker-hhvm/browse](https://stash.mtvi.com/projects/CRAB/repos/docker-hhvm/browse)

# What is this

HHVM LTS 3.6 (3.6.1) in fastcgi mode.  It is expecting connections at port 9000 for normal web processing and 9001 for administrative panel.

It was compiled against/with

* Ubuntu 14.10

It also has phpunit and composer support as well, should you need that sort of thing.

# TODO

* World Domination

# Usage

* For the lazy/insecure

`docker run -d -P --net=host -v /your/host/directory:/destination/location viacommedianetworks/hhvm`

* Admin panel enabled

`docker run -d -p 9000:9000 -p 9001:9001 -v /your/host/directory:destination/localation viacommedianetworks/hhvm`

* Just the main engine

`docker run -d -p 9000:9000 -v /your/host/directory:destination/localation viacommedianetworks/hhvm`



