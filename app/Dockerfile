# define from what image we want to build from
FROM node:16

# create app working directory
WORKDIR /usr/src/app

# install app dependencies
COPY package*.json ./

RUN npm install

# bundle app source code inside docker image
COPY . .

# map port 
EXPOSE 8080

# define command to run the app
CMD ["node", "index.js"]
