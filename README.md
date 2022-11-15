# youdeyiwu-hosting

该仓库提供了 docker-compose 模板，部署尤得一物前后端程序示例，

使用 docker-compose 部署，简化了原来需要手动 mq、minio 所需配置，

如果你不想使用 docker-compose，可以参考前后端项目仓库中的步骤来托管.

## 1. 主页

- 访问

演示 [www.youdeyiwu.com](https://www.youdeyiwu.com)

- 相关

前端 [youdeyiwu-frontend](https://github.com/dafengzhen/youdeyiwu-frontend)

后端 [youdeyiwu-frontend](https://github.com/dafengzhen/youdeyiwu-backend)

## 2 要求

请确保存在以下程序，安装可以参考[官方文档](https://docs.docker.com/engine/install/centos)，或者参考这里[相关示例](https://www.youdeyiwu.com/sections/26)

- docker（v20+）
- docker compose（v2+）

## 3. 使用

- 拷贝仓库

```bash
git clone https://github.com/dafengzhen/youdeyiwu-hosting.git && cd youdeyiwu-hosting
```

- 运行程序

配置文件修改，前端 youdeyiwu-fronted.env ，后端 youdeyiwu-backend.env

并且可根据需要修改调整 docker-compose 文件

```bash
docker compose up -d
```

- 访问程序

启动成功后，访问 http://localhost:3000

## 4. 升级

程序会定期的更新，如果你需要应用这些更新，使用 docker 更新升级变成非常容易，你需要执行如下操作：

```bash
docker-compose down --remove-orphans
```

```bash
docker compose pull dafengzhen/youdeyiwu-backend
```

```bash
docker compose pull dafengzhen/youdeyiwu-frontend
```

```bash
docker compose up -d
```

## 5. 注意

- 默认你的域名应该是使用 HTTPS 传输协议（如果没有证书，需要服务器后台免费生成并部署）

## 6. 其它

如果你有相关问题建议 PR、可以交流改进

- [issues](https://github.com/dafengzhen/youdeyiwu-hosting/issues)
- [youdeyiwu](https://www.youdeyiwu.com)

## 7. License

[MIT](https://opensource.org/licenses/MIT)







