# Docker Project - MBDS
AIT ERRAMI Amine<br/>
GAUTHIER Thomas

## How to run it
* `git clone https://github.com/aiterramimine/mbds_docker.git`
* `docker-compose up`
* Once launched, you can access the app with the url http://localhost:4200/

## Project details
The previous commands will create 3 running docker images :
- One for MongoDB
- One containing an Angular app (see the "angular" folder)
- One for a NodeJS/ExpressJS ("express" folder)

We use the official image for Mongo, but we created a Dockerfile for the 2 other images, at their respective folder root.<br/>
The Mongo and Node containers use the ports 27017 and 3000, for both their host and containers ports.<br/>
Concerning the Angular container, its host port is 5555 and its container port is 4200.<br/><br/>

The archive "backup_mbdsdocker.tar" contains 2 images :
- mbdsdocker_angular is the angular image
- mbdsdocker_express is the express image

As the archive was too heavy to be put on git, we shared it on [this drive](https://drive.google.com/open?id=1KeOwAhQ-MPvC46l3y4L_iMX7eiMyBW8u).

## Other details
We used the NodeJS and Angular CRUD app from [this repository](https://github.com/CodAffection/MEAN-Stack-CRUD-Operations).