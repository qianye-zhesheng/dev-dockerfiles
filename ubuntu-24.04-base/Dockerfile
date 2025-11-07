FROM ubuntu:24.04

RUN apt update && \
  apt upgrade -y && \
  apt install -y sudo tzdata && \
  apt clean && \
  ln -sf /usr/share/zoneinfo/Asia/Tokyo /etc/localtime && \
  echo "Asia/Tokyo" > /etc/timezone && \
  usermod -aG sudo ubuntu && \
  echo "ubuntu ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

USER ubuntu
WORKDIR /home/ubuntu

CMD ["/bin/bash"]
