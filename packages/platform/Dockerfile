FROM node:lts-alpine
WORKDIR /app
COPY ./dist/packages/platform/ .
ENV PORT=3090
EXPOSE ${PORT}
RUN npm install
# dependencies that nestjs needs
# RUN npm install reflect-metadata tslib rxjs @nestjs/platform-express
CMD node ./main.js