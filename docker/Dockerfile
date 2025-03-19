# Use the official Nginx image from the Docker Hub
FROM nginx:latest

# Copy the Nginx configuration file to the container
COPY docker/nginx.conf /etc/nginx/nginx.conf

# Copy the project files to the Nginx html directory
COPY src/index.html /usr/share/nginx/html/
COPY src/styles.css /usr/share/nginx/html/style.css
COPY src/script.js /usr/share/nginx/html/
COPY src/404.html /usr/share/nginx/html/
COPY src/500.html /usr/share/nginx/html/

# Expose port 80 to the outside world
EXPOSE 80

# Start Nginx when the container starts
CMD ["nginx", "-g", "daemon off;"]