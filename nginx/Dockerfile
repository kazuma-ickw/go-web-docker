FROM centos:7

RUN yum -y install http://nginx.org/packages/centos/7/noarch/RPMS/nginx-release-centos-7-0.el7.ngx.noarch.rpm
RUN yum -y install --enablerepo=nginx nginx

ADD ./files/etc/nginx/conf.d/app.conf /etc/nginx/conf.d/app.conf

CMD nginx -g 'daemon off;'
