FROM nginx
RUN apt-get update && apt-get install -yq --no-install-recommends \
    apt-utils \
    apache2 \
    git\
    curl\
    dos2unix\
    nodejs\
    npm\
    software-properties-common
CMD apachectl -DFOREGROUND
RUN mkdir ./home/CAVSweb

EXPOSE 80

RUN echo "ServerName example.com" >> /etc/apache2/apache2.conf