FROM almalinux:8

# Install nginx
RUN yum install -y nginx

# Remove default nginx index page
RUN rm -rf /usr/share/nginx/html/index.html

# Create a new custom index page
RUN echo "<h1>Hello, I am from app2</h1>" > /usr/share/nginx/html/index.html

# Start nginx in the foreground
CMD ["nginx", "-g", "daemon off;"]
