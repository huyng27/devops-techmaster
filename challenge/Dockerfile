
#FROM nginx
#RUN mkdir -p /usr/share/nginx/html
#COPY -r /home/parallels/Downloads/mobile-app-html-template /usr/share/nginx/html
#COPY nginx.conf /etc/nginx/nginx.conf

FROM nginx

# Create the destination directory
RUN mkdir -p /home/parallels/html

# Copy the mobile app HTML template
COPY mobile-app-html-template /home/parallels/html

# Copy the nginx configuration
COPY nginx.conf /etc/nginx/nginx.conf
