# Ghost on Ubuntu 14.04

Installs:

* Node.js (0.10 as newer versions break Ghost)
* Nginx
* PM2
* Ghost 0.7.0

## Vagrant

    $ vagrant up

Wait for a little bit and once it's done Ghost will be available at [localhost:8080](http://localhost:8080).

## DigitalOcean

    $ cd digitalocean
    $ cp config.default.yml config.yml

in `config.yml` add your API token

    $ vagrant up

The command will return the IP of the newly created droplet. Nginx reverse proxies Ghost on port 80.
