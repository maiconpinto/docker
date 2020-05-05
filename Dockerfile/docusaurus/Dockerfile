FROM node:13.14.0

WORKDIR /app/website

EXPOSE 3000 35729

RUN npm install --global docusaurus-init@1.14.1

ENTRYPOINT ["npm", "run", "start"]