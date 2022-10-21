FROM nginx:1.23.1-alpine

# Remove default config files in NGINX image
RUN rm /etc/nginx/nginx.conf /etc/nginx/conf.d/default.conf

COPY index.html /etc/nginx/html/
COPY nginx.conf /etc/nginx