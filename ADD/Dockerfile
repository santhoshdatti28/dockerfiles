FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/santhoshdatti28/dockerfiles/refs/heads/main/COPY/index.html /usr/share/nginx/html
RUN chmod +r /usr/share/nginx/html/index.html
ADD sample-1.tar /tmp
CMD ["nginx", "-g", "daemon off;"] 