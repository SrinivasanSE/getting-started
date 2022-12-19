# syntax=docker/dockerfile:1
FROM node:18-alpine
WORKDIR /app
COPY package.json yarn.lock ./
RUN yarn install --production
COPY . .
ENTRYPOINT ["node"]
CMD ["src/index.js"]
EXPOSE 3000
