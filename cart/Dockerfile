FROM                           node:20
RUN                            useradd roboshop
RUN                            mkdir /app
WORKDIR                        /app
RUN                            chown -R roboshop:roboshop /app
RUN                            npm install
CMD                            ["node","/app/server.js"]


