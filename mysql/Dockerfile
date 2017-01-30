FROM mysql:5.7
EXPOSE 3306

ADD ./setup.sh /setup.sh
RUN chmod 755 /setup.sh
RUN ./setup.sh
CMD tail -f /dev/null
