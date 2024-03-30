# Use the official Node.js 14 image as the base image
FROM node:14

# Set the working directory in the Docker container to /usr/src/app
WORKDIR /usr/src/app

# Copy the package.json and package-lock.json (if available) to the working directory
COPY package*.json ./

# Install the dependencies defined in package.json
RUN npm install

# Copy the rest of the application code to the working directory
COPY . .

# Define the command to run the application. This uses Node.js to run the server.js file
CMD [ "node", "server.js" ]