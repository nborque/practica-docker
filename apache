FROM library/debian:jessie
MAINTAINER NURIA
RUN apt-get update \
    && apt-get -y install apache2 libapache2-mod-php5 \
    && apt-get clean \
    && rm -rf /var/cache/apt /var/lib/{apt,dpkg}
EXPOSE 80
CMD /usr/sbin/apache2ctl -D FOREGROUND
