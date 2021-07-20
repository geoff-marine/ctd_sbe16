# how to build and run the moxa simulator

## Build

    docker build -t moxasim .

## Run

Create a network to run this instance(and later for the other parts of the env)

    docker network create --driver bridge sbe16

    docker run -d --name moxasim --network sbe16 -p 1881:1880 moxasim:latest
