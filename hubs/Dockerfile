FROM node:8-alpine

RUN apk add -U --no-cache git && \
    git clone https://github.com/yukimochi-mixedreality/hubs.git && \
    cd hubs && \
    sed -i -e "s/\"hubs.local:8080\",/\"hubs.vr.yukimochi.io\",/" webpack.config.js && \
    yarn install

WORKDIR /hubs

CMD ["yarn", "start"]
