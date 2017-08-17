# About this Repo

This is a fork of the official Docker image for [nginx](https://registry.hub.docker.com/_/nginx/). The maintainers of the officially endorsed Docker images have a fairly lax grasp of operational security and incorporate upsteam security patches such as version bumps of underlying images only sporadically. Also, they're slow to bump their images to new nginx versions.

Also, the official docker image does not play nice with php-fpm because linux user and group ids don't match up. This has been rectified in this image.

Changes compared with upstream:
- bumped alpine version
- generally more up to date nginx version
- fixed user and group IDs to correspond to those used by php:*-fpm-alpine

Find the Docker image here: (https://hub.docker.com/r/zyrill/nginx/)
