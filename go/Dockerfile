FROM centos:7
EXPOSE 5000

ARG goversion
RUN echo ${goversion}

RUN yum -y install git vim-enhanced
RUN curl -kLO https://storage.googleapis.com/golang/go${goversion}.linux-amd64.tar.gz
RUN tar -C /usr/local -xvzf go${goversion}.linux-amd64.tar.gz

ENV PATH $PATH:/usr/local/go/bin
ENV GOBIN $HOME/projects/bin
ENV GOPATH $HOME/projects

CMD tail -f /dev/null
