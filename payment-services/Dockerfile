# Use an official Node.js runtime as a parent image
FROM node:18-alpine

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application source code to the container
COPY . .

# Expose port 3003 to the outside world
EXPOSE 3003

# Define environment variable
ENV NODE_ENV=production

# Command to run the application
CMD ["node", "index.js"]