FROM jenkins/inbound-agent:4.11.2-4
USER root

RUN apt update -y && apt install curl -y
RUN VERSION="v1.25.0"
RUN wget https://github.com/kubernetes-sigs/cri-tools/releases/download/$VERSION/crictl-$VERSION-linux-amd64.tar.gz
RUN tar zxvf crictl-$VERSION-linux-amd64.tar.gz -C /usr/local/bin
RUN rm -f crictl-$VERSION-linux-amd64.tar.gz

USER root
