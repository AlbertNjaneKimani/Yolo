FROM node:13.12.0-alpine
WORKDIR /app
COPY package*.json /app/
RUN npm install
COPY ./app/
EXPOSE 5000
CMD ["npm","start"]
