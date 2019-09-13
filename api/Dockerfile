FROM node:12.8.1-alpine

ENV APP_DIR=/usr/local/app/
RUN mkdir -p $APP_DIR
WORKDIR $APP_DIR

# Expose api port
EXPOSE 3000

# Update image packages
RUN apk update

# Add repo to directory
ADD . $APP_DIR

# Install node modules
RUN npm install

CMD npm start

