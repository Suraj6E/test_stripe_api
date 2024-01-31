# Use an official Node.js runtime as the base image
FROM node:20.11.0

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install project dependencies
RUN npm install

# Copy the rest of your application's source code into the container
COPY . .

# Expose the port your Express application listens on (e.g., 8080)
EXPOSE 8080

# Start your application
CMD ["npm", "start"]
