FROM nginx
RUN rm -rf /usr/share/nginx/html/*
COPY static /usr/share/nginx/html/
COPY index.html /usr/share/nginx/html/
COPY asset-manifest.json /usr/share/nginx/html/
COPY robots.txt /usr/share/nginx/html/
COPY nginx.conf /etc/nginx/conf.d/expense.conf
