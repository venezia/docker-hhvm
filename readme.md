Repository is located [https://stash.mtvi.com/projects/CRAB/repos/docker-hhvm/browse](https://stash.mtvi.com/projects/CRAB/repos/docker-hhvm/browse)

# What is this

HHVM 3.5.1 in fastcgi mode.  It is expecting connections at port 9000 for normal web processing and 9001 for administrative panel.

It was compiled against/with
* Ubuntu 14.04
* wget

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

* Want to run phpunit?

`docker run -v /your/host/directory:destination/localation viacommedianetworks/hhvm /usr/local/bin/phpunit /destination/location/tests`


