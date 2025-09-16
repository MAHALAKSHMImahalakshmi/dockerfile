FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
# remove previous existed index.html
COPY webAPP/assets/ /usr/share/nginx/html/
# copy <source> <destination>
CMD ["nginx", "-g", "daemon off;"]
