FROM nginx:alpine

# 复制 nginx 配置
COPY nginx.conf /etc/nginx/nginx.conf

# 复制静态文件
COPY index.html /usr/share/nginx/html/index.html
#COPY custom.css /usr/share/nginx/html/w  # 可选

# 设置权限
RUN chown -R nginx:nginx /usr/share/nginx/html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]