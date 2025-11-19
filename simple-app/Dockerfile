# Use a lightweight Node.js base image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy HTML file into container
COPY . .

# Install a tiny static file server globally (instead of yarn)
RUN npm install -g serve

# Expose port 3000 (like your Node example)
EXPOSE 3000

# Command to run the static server
CMD ["serve", "-s", ".", "-l", "3000"]
