# Pull almalinux:9 as Base image
FROM almalinux:9
# Install nginix
RUN dnf install nginx -y
# Delete the default index.html#
RUN rm -rf /usr/share/nginx/html/index.html 
# copy the required index.html from current location to the container
COPY index.html /usr/share/nginx/html/index.html
# daemon off is mentioned to run in foreground#
CMD ["nginx","-g", "daemon off;"]