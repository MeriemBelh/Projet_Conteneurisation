FROM node:18-alpine as builder
WORKDIR /usr/src/app
COPY package*.json .
RUN npm install
COPY . .
RUN npm run build
FROM nginx:1-alpine-slim
COPY --from=builder /usr/src/app/dist/angular-16-crud /usr/share/nginx/html
EXPOSE 80
