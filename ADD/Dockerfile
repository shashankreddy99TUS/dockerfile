# FROM almalinux:9
# RUN dnf install nginx -y
# RUN rm index.html /usr/share/nginx/html/index.html
# ADD https://github.com/shashankreddy99TUS/dockerfile/blob/main/RUN/Dockerfile  index.html /usr/share/nginx/html/index.html
# CMD ["nginx","-g","daemon off;"]
FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/DAWS-82S/dockerfiles/refs/heads/main/RUN/Dockerfile /usr/share/nginx/html/index.html
RUN chmod +r /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]