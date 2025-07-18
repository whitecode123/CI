FROM ubuntu:24.04

RUN apt-get update && apt-get install -y apache2 curl && a2enmod proxy && a2enmod proxy_http && apt-get clean && rm -rf /var/lib/apt/lists/*

RUN a2ensite 000-default.conf

EXPOSE 80

CMD ["apache2ctl", "-D", "FOREGROUND"]
