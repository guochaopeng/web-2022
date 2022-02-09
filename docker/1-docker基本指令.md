I.Docker 的三大基础组件
I.1: Docker 仓库, Docker 镜像
Docker 官方会给 i 共一个 Docker 仓库, 就像是手机里的 App 应用商店，里面存放着
各种各样已经打包好的 Docker 应用--Docker 镜像

I.2: Docker 镜像
Docker 镜像是为了满足特殊用途而按照 Docker 的规则制作的应用。

I.3: Docker 容器
利用 Docker 镜像可以创建 Docker 容器, 容器会启动预先定义好的进程与用户交互，对外
提供服务。
容器都是基于镜像而创建的，基于一个镜像可以创建多个名称不同但功能不同的容器

II. Docker 的帮助命令
II.1: docker command --help
II.2: docker 仓库的相关命令: docker search, docker pull
II.3: docker 容器的相关命令： docker ps, docker run
II.4: docker 镜像的相关命令: docker images, docker build
