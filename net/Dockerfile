#基础镜像 `microsoft/dotnet:latest`
FROM microsoft/dotnet:latest

#拷贝 当前web目录./Core 到 docker中的publish目录中
COPY ./Core /publish

#切换工作目录到 docker中的`/publish`
WORKDIR /publish

#暴露docker的端口号8000
EXPOSE 8000

#启动问web服务`dotnet HelloWebApp.dll`

CMD ["dotnet", "WebApp.Core.dll"]

#基础镜像
FROM nginx:latest

# copy 用本地nginx配置文件 替换 docker中
COPY ./nginx.conf /etc/nginx/nginx.conf

# 向外暴露80端口
EXPOSE 80