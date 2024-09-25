# Use the official Node.js image from the Docker Hub
FROM node:14

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json into the container
COPY package*.json ./

# Install the dependencies
RUN npm install

# Copy the rest of your application code into the container
COPY . .

# Expose the port that the frontend runs on
EXPOSE 3000

# Command to run your application
CMD ["npm", "run", "dev"]