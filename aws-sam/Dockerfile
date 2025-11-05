FROM qianyezhesheng/node:latest

RUN sudo apt update && sudo apt install -y unzip git && \
  curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" && \
  unzip awscliv2.zip && \
  sudo ./aws/install && \
  rm awscliv2.zip && \
  curl -L "https://github.com/aws/aws-sam-cli/releases/latest/download/aws-sam-cli-linux-x86_64.zip" -o "aws-sam-cli-linux-x86_64.zip" && \
  unzip aws-sam-cli-linux-x86_64.zip -d sam-installation && \
  sudo ./sam-installation/install && \
  rm aws-sam-cli-linux-x86_64.zip && \
  npm install -g esbuild
