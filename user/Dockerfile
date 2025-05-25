FROM                           node:20
RUN                            useradd roboshop
RUN                            mkdir /app
RUN                            chown -R roboshop:roboshop /app
WORKDIR                        /app
COPY                           code/* /app/
RUN                            npm install
CMD                            ["node","/app/server.js"]