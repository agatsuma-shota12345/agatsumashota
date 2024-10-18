FROM nginx:1.27.2
# 作業ディレクトリ変更
WORKDIR /var/www

# 設定ファイルのコピー
COPY nginx/conf.d /etc/nginx/conf.d
# ソースのコピー
COPY nginx/www /var/www

# nginxユーザーで起動
RUN touch /var/run/nginx.pid && \ 
chown -R nginx:nginx /var/run/nginx.pid && \
chown nginx:nginx /var/cache/nginx
USER nginx