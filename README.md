# 🖌️ Sign-Off

> 给 AI 输出加个性化落款签名。像对讲机的 Over，让 AI 说完了你知道。

## 效果

```
杭州今天多云17°C，晚上有小雨，记得带伞。

      小橘 书于杭州 春
      🏮 [橘印]
```

一看落款 → AI 说完了 → 该你了。

## 安装

### OpenClaw

```bash
clawhub install sign-off
```

### 手动安装

1. 把 SKILL.md 复制到你的 skills 目录
2. 把 sign-off.json.example 复制为 sign-off.json，修改配置
3. 完成

## 配置

复制 sign-off.json.example 为 sign-off.json:

```json
{
  "name": "你的AI名字",
  "location": "你的城市",
  "template": "{name} 书于 {location} {season}",
  "emoji": "🏮",
  "seal": "[印章]",
  "contextMode": "auto"
}
```

也可以直接告诉 AI：
> "你的签名改成 From 小橘, Hangzhou, with 🧡"

## 预装模板

| 模板 | 风格 | 预览 |
|------|------|------|
| 🖌️ calligraphy | 书法风 | 小橘 书于杭州 春 🏮 [橘印] |
| 💌 letter | 信笺风 | From 小橘, Hangzhou, with 🧡 |
| 🎭 ancient | 古风 | 蛇年春，小橘灯下 |
| 🤖 geek | 极客风 | // signed: xiaoju @ hangzhou |
| 📻 walkie-talkie | 对讲机风 | 📻 小橘 Over |

使用模板：告诉 AI "给我换成书法风" 即可。

## 变量

详见 [变量参考文档](docs/variables.md)

## 贡献模板

欢迎提交你的签名模板！

1. Fork 本仓库
2. 在 templates/ 下新建 JSON 文件
3. 参考已有模板的格式
4. 提交 PR

## License

MIT
