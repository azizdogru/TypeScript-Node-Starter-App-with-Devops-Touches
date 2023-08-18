# Base the image on an appropriate version of Node.js
FROM node:14
# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy project files
COPY . .
RUN npm run build

# Start the application
CMD ["npm", "start"]
