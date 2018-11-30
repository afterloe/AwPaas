# builder 使用须知
> create by afterloe <lm6289511@gmail.com>
> Apache License 2.0
> https://github.com/afterloe

### 构建go相关项目
```sbtshell
echo "ready to build awpaas image"
src=$1
out=$2
echo "use ${src} to build"
echo "bin export to ${out}"
docker run -it \
-v ${src}:/go/src \
-v ${out}:/app \
--rm \
awpaas/builder:1.0.0 \
go build
```
运行镜像可以使用alpine:3.8 系列镜像，构成之后的镜像约19.8MB

### awpaas系列组件中使用make来构建
```sbtshell
make -m src=/data/data-2/go/src
docker run -it awpaas/awpaas-route:1.0.0
```
### build
```sbtshell
docker build -t awpaas/builder:1.0.0 .
```
