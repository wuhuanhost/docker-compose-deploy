# docker-compose-deploy

使用 docker-compose 快速部署 web 项目（nodejs）

### 项目文件结构图

```shell
.
├── docker-compose.yml          容器启动配置文件
├── Dockerfile                  node构建配置文件
├── conf                        配置目录
│   ├── mysql                   MySQL配置文件目录
│   │   └── my.cnf              MySQL配置文件
│   └── nginx                   Nginx配置文件目录
│       ├── conf.d              站点配置文件目录
│       │   ├── certs           SSL认证文件、密钥和加密文件目录
│       │   │   └── site2       站点2的认证文件目录
│       │   ├── site1.conf      站点1 Nginx配置文件
│       │   └── site2.conf      站点2 Nginx配置文件
│       └── nginx.conf          Nginx通用配置文件
├── log                         日志目录
│   ├── mysql                   MySQL日志目录
│   ├── nginx                   Nginx日志目录
│   └── node                    node日志目录
├── mysql                       MySQL数据文件目录
└── www                         站点根目录
    ├── site1                   站点1根目录
    └── site2                   站点2根目录
```
