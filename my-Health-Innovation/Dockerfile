# Use official Node.js image
FROM node:18

# Set working directory
WORKDIR /app

# Copy package files and install deps
COPY package*.json ./
RUN npm install

# Copy rest of the app
COPY . .

# Expose frontend port (Vite default dev server)
EXPOSE 2525

# Start the dev server
CMD ["npm", "run", "dev"]
