FROM node:12.8.1-alpine

ENV APP_DIR=/usr/local/app
RUN mkdir -p $APP_DIR
WORKDIR $APP_DIR

# Expose web port
EXPOSE 1234

# Update image packages
RUN apk update

# Add repo to directory
ADD . $APP_DIR

# Install node modules
RUN npm install

CMD npm start
