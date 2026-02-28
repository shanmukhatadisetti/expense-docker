FROM node:20 AS builder
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install

FROM node:20
EXPOSE 8080
WORKDIR /opt/server
RUN useradd expense
COPY --from=builder /opt/server /opt/server
USER expense 
CMD [ "node", "index.js" ]