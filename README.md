# Docker Web Demo

## 项目介绍
基于 Docker 的 Web 服务部署实践，实现 Nginx 容器化运行

## 技术栈
- Docker
- Nginx
- Linux

## 功能
- 容器运行
- 端口映射
- 静态页面部署

## 启动方式
```bash
docker-compose up -d
## 遇到的问题

### 1. curl Empty reply from server
排查：
- 检查容器是否运行
- docker logs 查看日志
- 检查端口映射

原因：
nginx 未正确启动

解决：
重新启动容器并确认配置

---

### 2. 端口无法访问
排查：
- 查看 docker ps
- 检查端口映射
- 检查本地防火墙

解决：
确认 8080 端口开放
