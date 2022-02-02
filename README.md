# nonebot-plugin-setu2

- 另另一个涩图插件
- 仅支持 NoneBot beta1 以上
- 指定群启用
- 代理使用**SOCKS5**模式
- 根据上游代码进行精简调整
- 采用**即时下载**发送，不在本地对图片进行保存
- 支持私聊获取~~特殊~~涩图

# 安装配置
```
pip install -U nonebot-plugin-setu2
```

## .env

```ini
SUPERUSERS=<list[str]>

SETU2_CD=<int>
SETU2_ENABLE_GROUPS=<list[int]>
PROXIES_SOCKS5=<str>
```
- `SUPERUSERS` NoneBot超级管理员
- `SETU2_CD` 单位：秒
- `SETU2_ENABLE_GROUPS` 启用群号列表
- `PROXIES_SOCKS5` 代理地址

## bot.py

```
nonebot.load_plugin("nonebot_plugin_setu2")
```

# 使用

- 指令 `(setu|来点色色)\s?(r18)?\s?(.*)?`
  - `setu|来点色色` 任意关键词
  - `r18` 可选（仅在私聊可用）
  - `关键词` 可选
- 例子
  - `来点色色 臭鼬`
  - `setu r18`

# 特别感谢

- [Mrs4s / go-cqhttp](https://github.com/Mrs4s/go-cqhttp)
- [nonebot / nonebot2](https://github.com/nonebot/nonebot2)
- [kexue-z / nonebot-plugin-setu-now](https://github.com/kexue-z/nonebot-plugin-setu-now)