FROM node:18

RUN apt-get update \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" \
    && unzip awscliv2.zip \
    && ./aws/install \
    && rm -rf ./aws awscliv2.zip \
    && npm -g install typescript \
    && npm install -g aws-cdk \
    && npm install -g npm-check-updates \