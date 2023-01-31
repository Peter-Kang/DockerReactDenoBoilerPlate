# Dockerfile
# Pull the base image
FROM node:19-alpine3.17
# Set the working directory
WORKDIR /usr/src/app/react-app
# Copy app dependencies and app to container
COPY react-app/. .
# Add `/app/node_modules/.bin` to $PATH
ENV PATH /app/node_modules/.bin:$PATH
# Install dependencies
RUN npm install
# Deploy app for local development
CMD npm start --host 0.0.0.0 --port 3000 --disableHostCheck true