# Use official Node.js LTS image
FROM node:18

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json (if available)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy backend code
COPY . .

# Expose the backend port
EXPOSE 8000

# Start the server
CMD ["npx", "nodemon", "index.js"]
