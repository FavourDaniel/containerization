# Base Image
FROM node:20-alpine

WORKDIR /var/www/app

COPY package.json package-lock.json ./

RUN npm install

COPY . .

EXPOSE 5173

CMD ["npm", "run", "dev", "--", "--host"]