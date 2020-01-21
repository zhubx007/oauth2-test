# 构建简易OAuth2服务器

## 按步骤执行

1. 运行服务

```bash
go run main.go

```

2. 打开浏览器，访问http://127.0.0.1:9096/credentials， 获取CLIENT_ID和CLIENT_SECRET。
 - CLIENT_ID: bca074dd
 - CLIENT_SECRET: 17fe25ed
3. 访问http://127.0.0.1:9096/token?grant_type=client_credentials&client_id=bca074dd&client_secret=17fe25ed&scope=all，获取access_token。
 - access_token: DFBMRGPDOO2DJNASKIGLEA
4. 最后访问http://127.0.0.1:9096/protected?access_token=DFBMRGPDOO2DJNASKIGLEA，页面相应“Hello, I'm protected.”，即成功、