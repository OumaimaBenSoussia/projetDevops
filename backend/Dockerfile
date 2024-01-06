# Use a Node.js base image

FROM node:18.17.1-alpine



# Set the working directory in the container

WORKDIR /usr/src/app

# opy package.json and package-lock.json to the working directory

COPY package*.json ./



# Install app dependencies

RUN npm install



# Copy the rest of the app files to the working directory

COPY . .



# Expose the port the app runs on

EXPOSE 3000



# Start the Node.js app

CMD ["npm", "start", "--", "--privileged"]

