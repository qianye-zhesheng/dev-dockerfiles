FROM qianyezhesheng/ubuntu-24.04-base:latest

SHELL [ "/bin/bash", "-c" ]

RUN sudo apt update && \
  sudo apt install -y curl && \
  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash && \
  . "$HOME/.nvm/nvm.sh" && \
  nvm install 22 && \
  # 子イメージ用Dockerfile内でnodeコマンドを使えるように永続化
  sudo ln -s $(which node) /usr/local/bin/node && \
  sudo ln -s $(which npm) /usr/local/bin/npm && \
  sudo ln -s $(which npx) /usr/local/bin/npx
  