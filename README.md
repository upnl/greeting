유피넬 서버 안내페이지
========
서버별 안내 페이지입니다.
```shell
sudo ln -s "$PWD/sodrak" /var/www/welcome
sudo ln -s "$PWD/gemini" /usr/share/nginx/welcome
```

### Apache2/Nginx 설정
```apache
# apache2
<VirtualHost *:80>
  DocumentRoot /var/www/welcome
</VirtualHost>
```
```Nginx
# nginx
server {
  listen 80 default_server;
  server_name _;
  root /usr/share/nginx/welcome;
}
```
