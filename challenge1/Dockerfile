# Use the Nginx image from Docker Hub
FROM nginx:alpine

# Remove the default Nginx configuration file
RUN rm /etc/nginx/conf.d/default.conf

# Replace it with our custom Nginx configuration file
COPY nginx.conf /etc/nginx/conf.d/

# Copy the 'public' folder to the Nginx web directory
COPY public/ /usr/share/nginx/html

# Expose port 80
EXPOSE 80

# Start Nginx when the container has provisioned
CMD ["nginx", "-g", "daemon off;"]