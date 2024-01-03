# Use an official lightweight Node.js image
FROM node:alpine

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Expose port 80 to the outside world
EXPOSE 80

# Define environment variable
ENV NAME Docker_HTML_App

# Command to run the application
CMD ["node", "-v"]

# Specify that we want to run an HTML file
ENTRYPOINT ["node", "-e", "require('http').createServer((req, res) => res.end(require('fs').readFileSync('index.html'))).listen(80)"]

