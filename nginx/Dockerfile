FROM nginx:stable-alpine
RUN rm /etc/nginx/conf.d/*
COPY ./default.conf /etc/nginx/conf.d/default.conf
# Turn off daemon to avoid "Bind for 0.0.0.0:80 failed: port is already allocated"
CMD [ "nginx", "-g", "daemon off;" ]