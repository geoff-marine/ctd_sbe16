# info on how to build and run the docker image

## Build

    docker build -t noderedkafkaconn .

## Run

    docker run -d --name noderedkafkaconn --network sbe16 -p 1884:1880 noderedkafkaconn:latest 