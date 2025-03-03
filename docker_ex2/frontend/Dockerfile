# 使用 Node.js 14 作为基础镜像
FROM node:14

# 设置工作目录
WORKDIR /usr/src/app

# 复制依赖文件
COPY package.json yarn.lock .

# 安装依赖
RUN yarn install

# 复制前端代码
COPY . .

# 暴露端口
EXPOSE 3000

# 运行前端应用
CMD ["yarn", "start"]