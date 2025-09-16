FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ONBUILD COPY index.html /usr/share/nginx/html/index.html
CMD ["nginx", "-g","daemon off;"]
# ONBUILD: Triggers instructions when a new image is built FROM this one, enabling reusable “parent” images
#While devloping images you can put some conditions while others are using your images...