# Dwellingly-Compose

This repo has code related to the creation of the dwellingly stack as a set of connected Docker containers managed through docker-compose. 

## Installation

Install [docker and docker-compose](https://docs.docker.com/compose/install/) for your host platform.

### Ubuntu 

For Ubuntu 20.04, run

```
sudo apt update
sudo apt install docker.io docker-compose -y
```

## Setup
The repo uses submodules. Run these two commands to populate the folders with the source code for the frontend and backend.

```
git submodule init
git submodule update
```

## Running
Simply running 
```
sudo docker-compose up
```
will start the process. The first time it runs it will take a while- it needs to download and setup all of the images. 

Once it is done, you should then be able to navigate to `http://localhost:3000` and see the frontend.

## Development
You can edit the `dwellingly-app` and `dwellinglybackend` subfolders as though they were cloned repos. Any changes to `.js` or `.py` files in these submodules will trigger a reload of the frontend and backend, respectively. 
