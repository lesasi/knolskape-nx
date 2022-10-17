FROM node:lts-alpine
WORKDIR /app
COPY ./dist/packages/genie-webapp/ .
ENV PORT=3010
EXPOSE ${PORT}
RUN npm install
# dependencies that nestjs needs
# RUN npm install reflect-metadata tslib rxjs @nestjs/platform-express
CMD npm exec next start