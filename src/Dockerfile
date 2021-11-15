FROM node:8.7-alpine
USER foo@example.com
HEALTHCHECK --interval=30s --timeout=30s --start-period=5s --retries=3 CMD [ "executable" ]

WORKDIR /home/app

COPY package.json /home/app
RUN npm install
COPY . /home/app

CMD ["npm", "start"]

EXPOSE 3000
