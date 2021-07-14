FROM nodered/node-red
USER node-red
RUN npm install node-red-dashboard
RUN npm install node-red-contrib-kafka-manager
COPY data/flows.json /data/flows.json
COPY data/settings.js /data/settings.js