FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
# remove previous existed index.html
COPY qi/ /usr/share/nginx/html/
# copy <source> <destination>
RUN chmod +r /usr/share/nginx/html/
CMD ["nginx", "-g", "daemon off;"]
