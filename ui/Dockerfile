FROM arduosoft/rawcms-ui-preview


COPY ./nginx-heroku.conf /etc/nginx/nginx-heroku.conf



CMD  envsubst '\$PORT' < /etc/nginx/nginx-heroku.conf > /etc/nginx/conf.d/default.conf && sh /bootstrap.sh &&   nginx -g "daemon off;"