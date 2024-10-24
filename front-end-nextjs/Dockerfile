# Use the official Node.js 18 image
FROM node:18

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json into the container
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the front-end code into the container
COPY . .

# Expose the port the Next.js app runs on
EXPOSE 3000

# Run the Next.js server
CMD ["npm", "run", "dev"]
