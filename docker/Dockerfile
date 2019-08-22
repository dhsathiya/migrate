FROM debian
MAINTAINER devarshisathiya5@gmail.com
RUN apt update 
RUN apt install wget -y
RUN wget https://github.com/actions/migrate/releases/download/2019-08-06%4020-47/migrate-actions-linux.tar
RUN wget https://storage.googleapis.com/golang/go1.9.3.linux-amd64.tar.gz 
RUN tar -xvf go1.9.3.linux-amd64.tar.gz 
RUN tar -xvf migrate-actions-linux.tar
RUN cp go/bin/go /bin/ 
COPY ./entrypoint.sh /
RUN chmod +x /entrypoint.sh
ENTRYPOINT [ "/entrypoint.sh" ]

