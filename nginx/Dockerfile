FROM nginx:1.27.2
# 作業ディレクトリ変更
WORKDIR /var/www

COPY nginx/html /var/www/html

# nginxユーザーで起動
RUN touch /var/run/nginx.pid && \ 
chown -R nginx:nginx /var/run/nginx.pid && \
chown nginx:nginx /var/cache/nginx
USER nginx