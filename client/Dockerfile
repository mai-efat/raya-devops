#step 1: Build the Nuxt.js application
FROM node:18 AS builder

# Set the working directory
WORKDIR /app
# Copy package.json and package-lock.json


COPY package-lock.json ./


COPY package*.json ./

# Install dependencies
RUN npm install


# Copy the rest of the application code
COPY . .

# Build the Nuxt.js application
RUN npm run build



# Expose the application port (default is 3000)
EXPOSE 3000

# Start the Nuxt.js application

CMD ["npm", "run", "start"]
