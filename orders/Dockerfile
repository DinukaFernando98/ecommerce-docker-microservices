FROM node:alpine
ENV CI=true
RUN npm install -g nodemon
 
WORKDIR /app
COPY package.json .
RUN npm install --only=prod
COPY . .
 
CMD ["npm", "start"]