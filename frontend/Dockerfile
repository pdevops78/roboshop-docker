FROM                     nginx
RUN                      rm -rf /usr/share/nginx/html/*
RUN                      rm -rf /etc/nginx/conf.d/default.conf
COPY                     code/ /usr/share/nginx/html/
COPY                     roboshop.conf /etc/nginx/conf.d/default.conf
