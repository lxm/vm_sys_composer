FROM centos:7
RUN yum -y install epel-release
RUN rpm -ivh http://rpms.famillecollet.com/enterprise/remi-release-7.rpm
RUN yum -y --enablerepo=remi-php70 install php php-mysql php-xml php-json php-gd php-fpm && yum clean all
EXPOSE 9000
ENTRYPOINT /usr/sbin/php-fpm --nodaemonize