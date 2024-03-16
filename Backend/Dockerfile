# Define base image
FROM node:latest

# Define work directory
WORKDIR /usr/src/app

ENV HOST 0.0.0.0

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all files
COPY . .

# Expose port
EXPOSE 3001

# Run the app
CMD ["node", "app.js"]