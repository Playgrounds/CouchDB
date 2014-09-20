# CouchDB Playground

This is a simple Playground conntaining a current [Apache CouchDB](http://couchdb.apache.org/) installation.

## Details

The VM is based on Ubuntu 14.04 including the following services and packages
installed:

- Ubuntu's build-essentials (gcc & Co.)
- Erlang
- Spidermonkey
- libICU
- CouchDB 1.6.0

The IP address of the VM is `10.152.149.104`.

After the VM is booted you may connect to its CouchDB instance on port `5984`.
Try opening `http://10.152.149.104:5984/_utils/` to connect to the CouchDBs admin
interface.

All CouchDB related files and executables are stored in
`/home/vagrant/CouchDB`. The CouchDB sources can be found at
`/home/vagrant/Sources`.

## Installation

The following steps are needed in order to utilize this Playground:

- Checkout the git repository
```
$ git clone git@github.com:Playgrounds/Elasticsearch.git
```

- Initialize all needed ansible roles using [Composer](http://getcomposer.org)
```
$ cd Automation && composer install
```

- Make vagrant build the VM for you
```
$ vagrant up
```
