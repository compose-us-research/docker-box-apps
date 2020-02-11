FROM node:12
WORKDIR /reimemonster
RUN apt-get install -y git && \
    git clone https://github.com/Narigo/reimemonster.git . && \
    npm ci
CMD npm run demo
