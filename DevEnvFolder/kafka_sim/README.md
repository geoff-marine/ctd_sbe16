# How to run

    docker-compose up -d

## network

have to join the contianers manually to sbe16 network.

    docker network connect sbe16 7497b9b03148

For GUI: http://10.11.1.30:9021/clusters

Following guide here https://docs.confluent.io/platform/current/quickstart/ce-docker-quickstart.html?utm_medium=sem&utm_source=google&utm_campaign=ch.sem_br.nonbrand_tp.prs_tgt.kafka_mt.xct_rgn.emea_lng.eng_dv.all_con.kafka-docker&utm_term=kafka%20docker&creative=&device=c&placement=&gclid=CjwKCAjwlrqHBhByEiwAnLmYUPSP_0Fpsl7pqklWtenG31dOymvOdCvUmponSSBldUm1IV_svetVzxoC-C4QAvD_BwE#step-2-create-ak-topics

### gotcha

For this dev enviroment all containers are in the same network so make sure that your aiming at right port numbers.  For example in this network 29092 is the kafka port number, not the standard 9092.


