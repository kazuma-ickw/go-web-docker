FROM mysql:5.7
EXPOSE 3306

ENV MYSQL_USER user
ENV MYSQL_ROOT_PASSWORD pass
ENV MYSQL_DATABASE db

ADD ./setup.sh /setup.sh
RUN chmod 755 /setup.sh
RUN ./setup.sh
CMD tail -f /dev/null
