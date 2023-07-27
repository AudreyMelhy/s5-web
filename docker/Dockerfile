FROM httpd
LABEL maintainer="ektech"
LABEL date="07/26/2013"
LABEL modified_by="Audrey"
ARG port=80
USER root
RUN apt -y update 
WORKDIR /usr/local/apache2/htdocs/

RUN rm -rf *
ADD ./code/* /usr/local/apache2/htdocs/

ENTRYPOINT ["httpd-foreground"]
EXPOSE ${port}
