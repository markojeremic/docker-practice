FROM node:16-alpine
WORKDIR /frontend
ENV PATH /frontend/node_modules/.bin:$PATH
COPY package.json .
COPY package-lock.json .
RUN npm install
COPY . .
EXPOSE 3000
CMD ["npm", "start"]