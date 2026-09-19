# Use Node.js runtime environment
FROM node:20-alpine

# Set working directory inside the container
WORKDIR /app

# Copy package config files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy backend source files (server.js, db.js, etc.)
COPY . .

# Expose backend port
EXPOSE 5000

# Start backend server directly
CMD ["node", "server.js"]