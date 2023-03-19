FROM centos:centos8
RUN yum install -y httpd && \
    mkdir -p /opt/sas/viya
WORKDIR /root/
COPY entrypoint.sh /root/
COPY index.html /var/www/html
RUN chmod +x entrypoint.sh
ENTRYPOINT ["/root/entrypoint.sh"]
