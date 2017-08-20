# About this Repo

This is a fork of the official Docker image for [nginx](https://registry.hub.docker.com/_/nginx/). The maintainers of the officially endorsed Docker images have a fairly lax grasp of operational security and incorporate upsteam security patches such as version bumps of underlying images only sporadically. Also, they're slow to bump their images to new nginx versions. And all of the build prerequisites (such as gcc and make!) are still lying around in the package which is an obvious security risk.

Also, the official docker image does not play nice with php-fpm because linux user and group ids don't match up. This has been rectified in this image.

Changes compared with upstream:
- bumped alpine version
- generally more up to date nginx version
- fixed user and group IDs to correspond to those used by php:*-fpm-alpine

Note that tagged images are released and never changed. The "latest" image however may be a few commits ahead of the last released version. This process allows incorporation of version bumps of upstream images without compromising stability of releases.

Find the Docker image here: (https://hub.docker.com/r/zyrill/nginx/)

Find development info here: (https://github.com/zyrill/docker-nginx) 
