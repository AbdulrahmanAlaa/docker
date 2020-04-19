FROM node:alpine as Builder 
WORKDIR /app
COPY package.json .
Run npm i

COPY . .
RUN npm run build

FROM nginx 
COPY --from=Builder /app/build /usr/share/nginx/html