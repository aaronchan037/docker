# 使用Debian官方镜像作为基础镜像
FROM debian:latest

# 更新软件包列表并安装git、curl和wget
RUN apt-get update \
  && apt-get install -y git curl wget \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*

# 设置工作目录
WORKDIR /test

# 可以在这里添加其他需要的命令，例如启动脚本等
CMD ["bash"]