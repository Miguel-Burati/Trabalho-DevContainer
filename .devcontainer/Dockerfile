FROM node:18-bullseye

RUN npm install -g expo-cli

WORKDIR /app/app

COPY ./app/package.json ./app/package-lock.json ./

RUN npm install

COPY ./app ./

EXPOSE 19000 19001 19002

CMD ["npx", "expo", "start", "--tunel"]