FROM debian
MAINTAINER devarshisathiya5@gmail.com
RUN apt-get update && apt-get install wget -y \
 && rm -rf /var/lib/apt/lists/*
RUN wget https://github.com/actions/migrate/releases/download/2019-08-06%4020-47/migrate-actions-linux.tar
RUN tar -xvf migrate-actions-linux.tar
COPY ./entrypoint.sh /
ENTRYPOINT [ "/entrypoint.sh" ]

