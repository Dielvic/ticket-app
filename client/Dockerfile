FROM node:alpine

WORKDIR /app
COPY package.json .
RUN npm install
RUN npm update && export NODE_OPTIONS=--openssl-legacy-provider
RUN npx browserslist@latest --update-db 
COPY . .

CMD ["npm", "run", "dev"]
