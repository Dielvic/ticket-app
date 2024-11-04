FROM node:alpine

WORKDIR /app
COPY package.json .
RUN npm install
#RUN npx browserslist@latest --update-db
RUN npm --depth 20 update --save caniuse-lite browserslist 
COPY . .

CMD ["npm", "run", "dev"]
