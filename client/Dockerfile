FROM node:alpine

WORKDIR /app
COPY package.json .
RUN npm install
RUN export NODE_OPTIONS=--openssl-legacy-provider
RUN npx browserslist@latest --update-db && npm update
COPY . .

CMD ["npm", "run", "dev"]
