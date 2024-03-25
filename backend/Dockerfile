FROM node:14-alpine3.12

WORKDIR /app

# Copy package.json and package-lock.json to install dependencies
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy the entire backend directory to the working directory
COPY . .

# Expose port 4000
EXPOSE 4000

# Start the application
CMD ["node", "backend/index.js"]
