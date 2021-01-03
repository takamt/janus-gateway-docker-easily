FROM nginx:1.19.4

RUN apt-get update \
&& apt-get install -y \
ssl-cert \
zip \
unzip \
vim \
wget

RUN DEBIAN_FRONTEND=noninteractive make-ssl-cert generate-default-snakeoil


WORKDIR /var/www/html
