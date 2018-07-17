#FROM is the base image for which we will run our application
FROM nginx:latest

RUN ["apt-get","update"]
RUN ["apt-get","install","-y","vim"]

# Copy files and directories from the application
COPY index.html /usr/share/nginx/html
COPY favicon.ico /usr/share/nginx/html
COPY Rakefile /usr/share/nginx/html
COPY style/ /usr/share/nginx/html/style/
COPY meta/ /usr/share/nginx/html/meta/
COPY js/ /usr/share/nginx/html/js/

# Tell Docker we are going to use this port
EXPOSE 80
