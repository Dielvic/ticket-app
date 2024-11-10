FROM node:alpine
#
ENV NODE_OPTIONS=--openssl-legacy-provider
WORKDIR /app
COPY package.json .
RUN npm install
# RUN npx browserslist@latest --update-db 
COPY . .

RUN npm run build
CMD ["npm", "run", "dev"]
