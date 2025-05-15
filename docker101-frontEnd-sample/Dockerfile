FROM node:22-alpine3.21
WORKDIR /app
COPY . .
RUN npm install
ENV API_URL=http://api.docker101.com/
EXPOSE 3000