FROM wordpress:latest

# Install make tool
ENV DEBIAN_FRONTEND=noninteractive PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/var/www/drupal/git/vendor/drush/drush/
RUN apt update && \
    apt full-upgrade -y
#RUN apt install wget
RUN apt-get -y install git
RUN cd /var/www/html/wp-content/themes && mkdir ./fundament && chmod +x ./fundament && ls -la && cd ./fundament && \
     git clone https://github.com/acdh-oeaw/fundament_wp . && ls -la
