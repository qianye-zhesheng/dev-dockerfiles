FROM qianyezhesheng/ubuntu-24.04-base:latest

SHELL [ "/bin/bash", "-c" ]

RUN sudo apt update && \
  sudo apt install -y curl && \
  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash && \
  . "$HOME/.nvm/nvm.sh" && \
  nvm install 22
  