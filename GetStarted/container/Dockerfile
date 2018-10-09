# 使用官方pyhton镜像作为基础镜像
FROM python:2.7-slim

# 配置工作目录
WORKDIR /app

# 拷贝当前目录下所有内容进入工作目录
COPY . /app

# 通过requirements.txt 文件安装所有python依赖
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# 使容器开发80端口
EXPOSE 80

# 定义环境变量
ENV NAME World

# 当容器启动时执行 `python app.py` 指令
CMD ["python", "app.py"]

