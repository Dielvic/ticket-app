FROM node:alpine

WORKDIR /app
COPY package.json .
RUN npm install --save-dev @types/express
RUN npm install --only=prod
COPY . .

CMD ["npm", "start"]
#