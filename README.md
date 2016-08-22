![](https://img.shields.io/docker/stars/redwyvern/runit.svg)
![](https://img.shields.io/docker/pulls/redwyvern/runit.svg)
![](https://img.shields.io/docker/automated/redwyvern/runit.svg)
[![](https://images.microbadger.com/badges/image/redwyvern/runit.svg)](https://microbadger.com/images/redwyvern/runit "Get your own image badge on microbadger.com")

This image is based on 'tozd/docker-runit' except that it has been adapted to use and
work with a Debian base image.

An image using [runit](http://smarden.org/runit/) for service supervision.

It can serve as a good base image for other Docker images.

In short, to create a service create `/etc/service/<name>/run` script which at the end
`exec`s into the service executable you want to run (and supervise to keep running).
