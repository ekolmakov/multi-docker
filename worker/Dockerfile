FROM node:alpine

WORKDIR /usr/local/app/

COPY package.json .

# install step
RUN npm install

# What we will update outside container
RUN npm update

RUN npm audit fix


COPY . .

CMD ["npm","run","start"]

