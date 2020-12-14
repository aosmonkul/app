FROM alpine

RUN apk update
RUN apk add mysql-client
CMD mysql {mysql-client-options} < {sql.script}

COPY import.sh /opt
COPY mydatabase.sql /opt 

WORKDIR /opt
