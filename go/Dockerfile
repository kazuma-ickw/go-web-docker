FROM centos:7
EXPOSE 5000

RUN yum -y install git
RUN curl -LO https://storage.googleapis.com/golang/go1.7.4.linux-amd64.tar.gz
RUN tar -C /usr/local -xvzf go1.7.4.linux-amd64.tar.gz

ENV PATH $PATH:/usr/local/go/bin
ENV GOBIN $HOME/projects/bin
ENV GOPATH $HOME/projects

CMD tail -f /dev/null
