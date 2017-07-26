#基础镜像
FROM nginx:latest

# copy 用本地nginx配置文件 替换 docker中
COPY ./nginx.conf /etc/nginx/nginx.conf

# 向外暴露80端口
EXPOSE 80

# 启动nginx服务
CMD ["nginx"]
