FROM nodered/node-red
USER node-red
RUN npm install node-red-dashboard
RUN npm install node-red-contrib-kafka-manager
COPY flows.json /data/flows.json