FROM node:18-alpine

# Set working directory
WORKDIR /app

# Install dependencies
COPY package.json package-lock.json ./
RUN npm install

# Copy project files
COPY . .

# Expose Vite default port
EXPOSE 5173

# Run in development mode
CMD ["npm", "run", "dev", "--", "--host"]