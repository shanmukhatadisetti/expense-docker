FROM nginx
RUN rm -rf /usr/share/nginx/html/*
COPY static /usr/share/nginx/html/
COPY . /usr/share/nginx/html/
COPY nginx.conf /etc/nginx/conf.d/expense.conf


