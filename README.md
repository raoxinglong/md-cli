# 本地安装

```bash
npm install
```

# 用法

## 启动服务
```bash
node index.js
```

## 或指定端口和绑定地址
```bash
node index.js --port=9000 --host=127.0.0.1
```

##  浏览器打开
默认 http://<你的IP>:8800  
默认绑定 0.0.0.0，局域网内可直接通过 <host_ip>:8800 访问。

# 关于dist的说明
dist/ 是从 [apps/web/](https://github.com/doocs/md/tree/main/apps/web) 构建产物复制过来的。如果 upstream 源码有更新，需要重新构建：
```bash
  cd md/apps/web && npx vite build --base=/
  rm -rf md/packages/md-cli/dist && cp -r md/apps/web/dist md/packages/md-cli/
```
