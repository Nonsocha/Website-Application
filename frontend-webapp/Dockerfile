# Use the official Node.js 14 image as the base
FROM node:14

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY webapp/package.json webapp/package-lock.json ./

# Install dependencies
RUN npm install

# Copy the entire webapp folder into the container
COPY webapp/ .

# Expose port 3000 for the React app
EXPOSE 3000

# Start the app
CMD ["npm", "start"]
