from node:alpine

WORKDIR '/app'

COPY ./package.json .
#RUN npm config set http-proxy http://docker.for.win.localhost:3128
#RUN npm config set https-proxy http://docker.for.win.localhost:3128

RUN yarn install

COPY . .

CMD ["yarn", "run", "dev"]