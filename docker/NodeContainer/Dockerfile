FROM node:10-alpine
RUN mkdir -p /src/app
WORKDIR /src/app
COPY package.json /src/app/package.json
COPY . /src/app
RUN npm install
CMD ["npm", "start"]
EXPOSE 3000
