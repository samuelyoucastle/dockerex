# 使用官方的 Python 3.8 slim 镜像作为基础镜像
FROM python:3.8-slim

# 设置容器内的工作目录
WORKDIR /usr/src/app

# 将当前目录的所有文件复制到容器的工作目录
COPY . .

# 安装 Python 依赖（从 requirements.txt 中读取）
RUN pip install --no-cache-dir -r requirements.txt

# 暴露端口 5000，供后端监听
EXPOSE 5000

# 指定运行后端应用的命令
CMD ["python", "app.py"]