I: centos 安装 nodejs
I.1: 添加 NodeSource 存储库;
curl -sL https://rpm.nodesource.com/setup_16.x | bash -

I.2: 安装 nodejs
yum install -y nodejs
yum install gcc-c++ make

I.3:测试
node --version
npm --version
