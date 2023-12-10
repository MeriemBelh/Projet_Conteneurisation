FROM node:latest as builder
WORKDIR /usr/src/app
COPY . .
RUN npm install
RUN npm run build
FROM nginx:1-alpine-slim
COPY --from=builder /usr/src/app/dist/angular-16-crud /usr/share/nginx/html
EXPOSE 80