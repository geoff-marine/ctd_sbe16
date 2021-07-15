# info on how to build and run the docker image

## Build

    docker build -t noderedtodb .

## Run

    docker run -d --name noderedtodb --network sbe16 -p 1883:1880 noderedtodb:latest 