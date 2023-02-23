FROM node:lts-alpine AS deps

ENV NPM_CONFIG_CACHE=/cache/npm
WORKDIR /app

COPY package*.json ./
RUN --mount=type=cache,dst=/cache/npm \
    npm install

FROM deps AS dev

ENV WDS_SOCKET_HOST=0.0.0.0
ENV WDS_SOCKET_PORT=0

COPY . .
CMD ["npm", "start"]
