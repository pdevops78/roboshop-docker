FROM                           node:20
RUN                            useradd roboshop
ENV                            DOCUMENTDB=true
ENV                            MONGO_URL="mongodb://username:password@mongodb:27017/catalogue?tls=true&replicaSet=rs0&readPreference=secondaryPreferred&retryWrites=false"
RUN                            mkdir /app
WORKDIR                        /app
RUN                            chown -R roboshop:roboshop /app
RUN                            npm install
COPY                           mongo.repo /etc/yum.repos.d/mongo.repo
CMD                            ["node","/app/server.js"]


