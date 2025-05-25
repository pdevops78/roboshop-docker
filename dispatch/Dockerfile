FROM                             golang:1.24
RUN                              useradd roboshop
RUN                              mkdir /app
RUN                              chown -R roboshop:roboshop /app
WORKDIR                          /app
RUN                              go mod init dispatch
RUN                              go get
RUN                              go build
