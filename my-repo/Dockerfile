FROM  centos:latest
LABEL ADD afaqaliawan5@gmail.com
RUN  yum install -y httpd \
zip\
unzip 
ADD  https://www.free-css.com/files/from-css-templates/download/page254/photogenic.zip /var/www/html/
WORKDIR   /var/www/html/
RUN unzip photogenic.zip
RUN cp -rvf photogenic/*
RUN rm -rf photogenic photogenic.zip
CMD ["/usr/sbin/httpd","-D", "FOREGROUND"]
EXPOSE 80 22
