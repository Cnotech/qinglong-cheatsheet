# 青龙面板-京豆薅羊毛小抄

## 部署 Docker
```
docker run -dit \
  -v $PWD/ql:/ql/data \
  -p 5700:5700 \
  --name qinglong \
  --hostname qinglong \
  --restart unless-stopped \
  whyour/qinglong:latest
```

## 订阅仓库
`https://github.com/KingRan/KR.git`

## 订阅后执行
```
cp -r /ql/data/repo/KingRan_KR_main/* /ql/data/scripts/KingRan_KR_main
cp /ql/data/repo/KingRan_KR_main/jdCookie.js /ql/data/scripts
cp /ql/data/repo/KingRan_KR_main/USER_AGENTS.js /ql/data/scripts
```

## 安装依赖
Node.js
```
png-js
date-fns
axios
crypto-js
ts-md5
tslib
@types/node
requests
tough-cookie
jsdom
download
tunnel
fs
ws
form-data
js-base64
qrcode-terminal
silly-datetime
ts-node
typescript
canvas
got
http-server
request
dotenv
```
Python
```
requests
```

## 配置环境变量
- `JD_COOKIE` 配置为 Cookie，[登录](https://m.jd.com)后在网络请求选项卡中复制 Cookie
- `JD_CART` 配置为 `true` （用于自动清理购物车）