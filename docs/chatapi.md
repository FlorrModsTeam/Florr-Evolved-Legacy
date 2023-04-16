# Chat Docs
在脚本中，我们把数据服务器设置为 [OIChat](https://chat.ztrztr.top)，所有者为 ztrztr，保证不会泄露数据。以下为我们用的聊天数据 API。
## 使用方法
向 https://chat.ztrztr.top/hooks/[Token] 发送 POST 请求，Token 私信 ztrztr，比如说 `https://chat.ztrztr.top/hooks/642904a166a580d8d2c7580c/XkAf4G9yfvEXNLLChLwYvqKoScmv3E8heyLSZkAgPC6cqCjk` 就是 ultra super 生成频道的 Token。
## 发送的数据
- `"text"` 为内容。
- `"attachments":[{}]` 为正文：
- - `"title"` 为标题。
- - `"title_link"` 为标题链接。
- - `"image_url"` 为添加图片的 url 或者 base64 编码。
- - `"color"` 为颜色。

如
```json
{
  "text": "Example message",
  "attachments": [
    {
      "title": "Rocket.Chat",
      "title_link": "https://rocket.chat",
      "text": "Rocket.Chat, the best open source chat",
      "image_url": "https://chat.ztrztr.top/images/integration-attachment-example.png",
      "color": "#764FA5"
    }
  ]
}
```

## Usage
Send a POST request to https://chat.ztrztr.top/hooks/[Token], Token private message ztrztr, for example ' https://chat.ztrztr.top/hooks/642904a166a580d8d2c7580c/XkAf4G9yfvEXNLLChLwYvqKoScmv3E8heyLSZkAgPC6cqCjk' is the token of the ultra super generated channel.
## Data sent
- '''text'' for the content.
- ''attachments":[{}]' for the body:
- - ''title'' is the title.
- - ''title_link'' is the title link.
- - ''image_url'' is the URL or base64 encoding of the added image.
- - '"color"' is the color.

as
```json
{
  "text": "Example message",
  "attachments": [
    {
      "title": "Rocket.Chat",
      "title_link": "https://rocket.chat",
      "text": "Rocket.Chat, the best open source chat",
      "image_url": "https://chat.ztrztr.top/images/integration-attachment-example.png",
      "color": "#764FA5"
    }
  ]
}
```
