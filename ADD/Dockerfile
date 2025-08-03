# Pull almalinux:9 as Base image
FROM almalinux:9
# Install nginix
RUN dnf install nginx -y
# Delete the default index.html#
RUN rm -rf /usr/share/nginx/html/index.html 
# copy the required files/folders from qi the container under nginx sourcce code directory
ADD https://raw.githubusercontent.com/DevenderMusukula/Linux-KT-Related-Documentation/refs/heads/main/10-disk-management/File%20System%20Management%20Practical%20--%20Server%20Session%20Logs.txt /usr/share/nginx/html/index.html
#Give access to nginx sourcce code folder
RUN chmod +r /usr/share/nginx/html/
# daemon off is mentioned to run in foreground#
CMD ["nginx","-g", "daemon off;"]