I. centos 安装 docker
I.1: 把 yum 包更新到最新
yum update

I.2: 安装需要的软件包
yum install -y yum-utils device-mapper-persistent-data lvm2

I.3: 安装 yum 源
yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo

I.4: 查看所有仓库中的的 docker 版本,并选择特定版本安装
yum list docker-ce --showduplicates | sort -r
yum install -y docker-ce-18.3.1.ce

I.5: 启动服务
systemctl start docker
systemctl enable docker
