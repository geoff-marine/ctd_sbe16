# info on how to build and run the docker image

## Build

    docker build -t moxatokafka .

## Run

    docker run -d --name moxatokafka --network sbe16 -p 1882:1880 moxatokafka:latest 