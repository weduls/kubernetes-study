# image
FROM node:12

# expose port
EXPOSE 3000 3000

# work directory
WORKDIR /usr/src/app

# package install
COPY package*.json ./
RUN npm install

# copy image
COPY . .

# container inner command
CMD ["npm", "start"]

