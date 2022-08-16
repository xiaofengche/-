
## 前置条件
注册一个微信公众号

https://mp.weixin.qq.com/debug/cgi-bin/sandbox?t=sandbox/login 

扫码登录成功后，就可以生成微信公众测试号的appID和appsecret
扫描测试号二维码后会生成微信号，那个账号需要接收就扫码

## 新增测试模板
模板标题: 自定义，例如: 宝宝，晚上好!  
模板内容参考:  
```
{{date.DATA}}  
城市：{{city.DATA}}  
天气：{{weather.DATA}}  
最低气温: {{min_temperature.DATA}}  
最高气温: {{max_temperature.DATA}}  
今天是我们恋爱的第{{love_day.DATA}}天  
距离小宝的生日还有{{birthday.DATA}}天  


{{note_en.DATA}}  
{{note_ch.DATA}}
```
## 安装python3 
官方网站: https://www.python.org/getit/

## 安装requests包
打开cmd，执行以下命令
```commandline
pip3 install requests
```

## 修改配置文件
`app_id`: 测试号信息里的appID 

`app_secret`: 测试信息里的appsecret

`template_id`: 模板消息接口里的模板ID

`user`: 测试号里的用户微信号

`province`: 所在省份

`city`: 所在城市

`birthday`: 生日

`love_date`: 纪念日

## 运行程序
```commandline
python3 main.py
```
