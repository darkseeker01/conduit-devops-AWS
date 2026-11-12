# Use Node.js LTS Alpine image
FROM node:22-alpine

# Set working directory inside container
WORKDIR /app

# Copy dependency files
COPY package*.json ./

# Install production dependencies
RUN npm install --omit=dev

# Copy backend source code
COPY . .

# Backend port
EXPOSE 3001

# Start backend application
CMD ["npm", "start"]