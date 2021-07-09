# MonoRun

## 简介/Introduction
This is a container based on [mono](https://registry.hub.docker.com/_/mono) which you can run your .NET Framework exe

一个可以运行 .NET Framework 应用程序的 Docker 容器，基于官方 [mono](https://registry.hub.docker.com/_/mono) 制作

## 使用方法/How to use
docker cli
```
docker run -d \
    --name=monorun \
    -e APP="/app/yourdotnet.exe" \
    -v /mnt/user/appdata/monorun:/app \
    xingkongsync/monorun
```

Just replace the path with your actual exe path

将本机的实际程序所在目录映射到容器中，并通过环境变量传入程序映射后的路径即可

## Docker Hub
[https://registry.hub.docker.com/r/xingkongsync/monorun](https://registry.hub.docker.com/r/xingkongsync/monorun)
