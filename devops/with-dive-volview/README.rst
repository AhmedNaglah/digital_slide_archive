===========================================
PathoGenerativeAI with Dive and VolView
===========================================

This directory contains a docker-compose set up for the PathoGenerativeAI with additional plugins to integrate with Dive and VolView.

You will probably want better container names than docker-compose will choose by default.

A typical set of commands are first to pull to make sure you have the most recent base images, then to start the containers::

    DSA_USER=$(id -u):$(id -g) docker-compose -f ../dsa/docker-compose.yml -f docker-compose.override.yml -p dsa-plus pull

    DSA_USER=$(id -u):$(id -g) docker-compose -f ../dsa/docker-compose.yml -f docker-compose.override.yml -p dsa-plus up
