# pm2
pm2知识
> 服务器部署

### 文件案例
```
apps:
  - script: ./server/server.js
    name: vue-todo
    env_production:
      NODE_ENV: production
      HOST: localhost
      PORT: 8888
```
### 启动
> pm2  start  pm2.yml --env  production 

### 重启
> pm2 restart  vue-todo

### 停止
> pm2 stop  vue-todo

### 查看启动的服务
> pm2 list 

### 快速查看日志
> pm2 log vue-todo

## 安装使用
> npm i pm2 -g
