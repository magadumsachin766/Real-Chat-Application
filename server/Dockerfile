# Use Node.js
FROM node:20-alpine

# Set working directory
WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm ci --legacy-peer-deps

# Copy backend source code
COPY . .

# Backend port
EXPOSE 8000

# Start the backend
CMD ["node", "index.js"]