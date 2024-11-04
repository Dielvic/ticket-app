FROM node:alpine
#
ENV NODE_OPTIONS=--openssl-legacy-provider
WORKDIR /app
COPY package.json .
RUN npm install
RUN npx browserslist@latest --update-db 
COPY . .

CMD ["npm", "run", "dev"]
