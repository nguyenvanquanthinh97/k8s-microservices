FROM node:12.13.0-alpine3.10

WORKDIR /app
COPY package.json yarn.lock ./
RUN yarn install --frozen-lockfile
COPY . .
RUN yarn build
CMD [ "yarn", "start" ]
