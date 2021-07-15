FROM nodered/node-red
USER node-red
RUN npm install lru-cache
RUN npm install node-red-dashboard
RUN npm install node-red-contrib-batcher
RUN npm install node-red-contrib-kafka-manager
RUN npm install node-red-contrib-postgrestor-next
RUN npm install node-red-contrib-mssql-plus
COPY data/flows.json /data/flows.json
COPY data/settings.js /data/settings.js
