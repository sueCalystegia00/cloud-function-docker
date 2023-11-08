# Google Cloud FunctionsのNode.jsランタイムは Node.js18が推奨
# https://cloud.google.com/functions/docs/concepts/python-runtime?hl=ja

FROM node:18

WORKDIR /workspace

RUN yarn global add firebase-tools

WORKDIR /workspace/functions

COPY functions/package.json ./

RUN yarn install

COPY functions .

CMD ["yarn", "serve"]