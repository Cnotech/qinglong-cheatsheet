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

## 添加通知渠道
### Server 酱

  `https://sct.ftqq.com/sendkey`
### 企业微信应用
- corpid 

  `https://work.weixin.qq.com/wework_admin/frame#profile`

  底部“企业ID”

- corpsecret

  `https://work.weixin.qq.com/wework_admin/frame#apps/modApiApp`

  进入对应应用之后点击“查看Secret”

- touser

  `https://work.weixin.qq.com/wework_admin/frame#contacts`

  点击需要推送的用户，复制其“帐号”

- agentid

  `https://work.weixin.qq.com/wework_admin/frame#apps/modApiApp`

  进入对应应用之后复制“AgentId”

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