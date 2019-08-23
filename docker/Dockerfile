FROM debian
MAINTAINER devarshisathiya5@gmail.com
RUN apt-get update \
 && apt-get install wget -y \ 
 && rm -rf /var/lib/apt/lists/*
RUN wget https://github.com/actions/migrate/releases/latest/download/migrate-actions-linux.tar
RUN tar -xvf migrate-actions-linux.tar
COPY ./entrypoint.sh /
ENTRYPOINT [ "/entrypoint.sh" ]

