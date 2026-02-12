# Upypi
MicroPython MIP 包管理仓库

## 翻译
1. 初始化
    * pybabel extract -F babel.cfg -o messages.pot .
    * pybabel init -i messages.pot -d translations -l zh
    * pybabel init -i messages.pot -d translations -l en
2. 更新
    * pybabel extract -F babel.cfg -o messages.pot .
    * pybabel update -i messages.pot -d translations
    * pybabel compile -d translations

## 运行项目
1. 构建容器：podman build -t upypi .
2. 运行容器：podman run -d -p 8080:443 upypi 自行准备证书文件与持久化目录

## 项目演示
https://upypi.net