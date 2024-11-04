FROM node:alpine

WORKDIR /app
COPY package.json .
RUN npm install
RUN npx browserslist@latest --update-db && npm update caniuse-lite
COPY . .

CMD ["npm", "run", "dev"]
