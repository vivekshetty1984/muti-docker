#Specify base image
FROM node:alpine
WORKDIR /app
COPY ./package.json ./
RUN npm config set strict-ssl false
RUN npm config set unsafe-perm true
RUN npm config set registry http://registry.npmjs.org/
RUN npm install
COPY ./ ./
CMD ["npm", "run" ,"start" ]
