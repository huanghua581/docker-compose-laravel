# docker-compose-laravel
基于 `docker-compose` 工作流的本地 `Laravel` 开发环境（LEMP）。

## 使用手册

开始之前，确保系统已经安装好 [Docker](https://docs.docker.com/docker-for-mac/install/) ，同时 `git clone` 本项目到本地。

添加你的 Laravel 项目源码到 `src` 目录, 打开终端进入此文件夹目录并在命令行中执行 `docker-compose up -d --build`。打开浏览器输入 [http://localhost:8080](http://localhost:8080) ，测试 Laravel 是否正常运行。

**对应的开发工具命令** :
- `docker-compose run --rm composer update`
- `docker-compose run --rm npm run dev`
- `docker-compose run --rm artisan migrate` 

容器映射端口为:
- **nginx** - `:8080`
- **mysql** - `:3307`
- **redis** - `:6380`
- **php** - `:9001`
- **npm**
- **composer**
- **artisan**


