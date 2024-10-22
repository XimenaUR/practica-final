
# Adjust NODE_VERSION as desired
FROM node:22.9.0-alpine


# Set directory
WORKDIR /app

# Copy packages
COPY package.json ./

# Install dependencies
RUN npm install

# Copy application code
COPY . .


# Start the server by default, this can be overwritten at runtime
EXPOSE 3000

# Command
CMD [ "npm", "run", "start" ]
