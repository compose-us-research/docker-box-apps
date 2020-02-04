FROM node:12
WORKDIR /app
RUN apt-get install -y git && \
    git clone https://github.com/compose-us-research/image-fun.git . && \
    npm ci
CMD npm run start
