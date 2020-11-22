# proxypool

本项目是 proxypool 的个人自用修改版，由于原作者经常删库，故在此备份以免代码失传。我修改的版本在 [master](https://github.com/ClarkeCheng/proxypool/tree/master) 分支，原版在 [master_old](https://github.com/ClarkeCheng/proxypool/tree/master_old) 分支，需要请自取。

[我修改的与原版的差异](https://github.com/ClarkeCheng/proxypool/compare/master_old...ClarkeCheng:master)

## 部署

### Docker

```bash
docker run -d --name proxypool -v /your/path/config.yaml:/proxypool-src/config.yaml -v /your/path/source.yaml:/proxypool-src/source.yaml clarkecheng/proxypool
```

### Docker Compose

```bash
mkdir proxypool
wget https://raw.githubusercontent.com/ClarkeCheng/proxypool/master/docker-compose.yml
docker-compose up -d
```

## 更新日志

- 2020 年 9 月 10 日，更新至 v0.3.10，移除代理名字中的广告
- 2020 年 9 月 25 日，移除代理名字中的 emoji
- 2020 年 11 月 23 日，移除在线聊天、谷歌统计、首页中的广告；为订阅链接增加超链接，增加多平台 Docker 镜像
