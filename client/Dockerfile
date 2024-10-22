FROM node:20-alpine

WORKDIR /app

COPY package.json package.json
COPY package-lock.json package-lock.json

RUN npm install

COPY public public
COPY index.html index.html
COPY tsconfig.app.json tsconfig.app.json
COPY tsconfig.json tsconfig.json
COPY tsconfig.node.json tsconfig.node.json
COPY vite.config.ts vite.config.ts
COPY src src

CMD npm run dev
