FROM node:22-alpine3.21
RUN addgroup app && adduser -S -G app app
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN chown -R app:app /app
USER app
ENV API_URL=http://api.docker101.com/
EXPOSE 5173
CMD ["npm", "run", "dev"]