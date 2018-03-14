# base image: last debian release
FROM debian:jessie

# install the latest upgrades
RUN apt-get update && apt-get -y dist-upgrade

# TODO install nginx
RUN apt-get install -y nginx

# TODO set the default container command command (CMD) to run the nginx daemon
CMD ["nginx", "-g", "daemon off;"]

# tell the container to listen to the port 80
EXPOSE 80

# create mount from external volume
VOLUME ["/var/www/html", "/var/log/nginx"]

