FROM nginx:mainline-alpine

COPY nginx.conf /etc/nginx/
COPY expires.conf /etc/nginx/
COPY protect-system-files.conf /etc/nginx/
COPY noslite /etc/nginx/sites-enabled/noslite
RUN rm -rf /etc/nginx/conf.d
