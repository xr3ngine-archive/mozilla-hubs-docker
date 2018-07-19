FROM node:8-alpine

RUN apk add -U --no-cache git && \
    git clone https://github.com/yukimochi-mixedreality/hubs.git && \
    cd hubs && \
    yarn install

WORKDIR /hubs

CMD ["yarn", "start"]
