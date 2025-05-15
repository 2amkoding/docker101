FROM node:22-alpine3.21
RUN addgroup app && adduser -S -G app app
USER app
WORKDIR /app
COPY package*.json .
RUN npm install
COPY . .
ENV API_URL=http://api.docker101.com/
EXPOSE 3000
CMD ["npm", "start"]