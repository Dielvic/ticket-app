FROM node:alpine

WORKDIR /app
COPY package.json .
RUN npm install --only=prod
COPY . .

RUN npm install @types/express
CMD ["npm", "start"]
#