# HTTP Front Proxy demo

### 环境说明
五个Service:
- envoy：Front Proxy,地址为172.31.6.2
- webserver01：第一个后端服务
- webserver01-sidecar：第一个后端服务的Sidecar Proxy,地址为172.31.6.11
- webserver02：第二个后端服务
- webserver02-sidecar：第二个后端服务的Sidecar Proxy,地址为172.31.6.12

### 运行和测试
1. 创建
```
docker-compose up
```

2. 测试
```
# 请求webserver01
curl -H "host: www.magedu.com" 172.31.6.2

# 请求webserver02
curl 172.31.6.2
```

3. 停止后清理
```
docker-compose down
```

## 版权声明
本文档版本归[马哥教育](www.magedu.com)所有，未经允许，不得随意转载和商用。
