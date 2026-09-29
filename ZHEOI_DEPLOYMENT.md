# 本项目开发记录

本仓库基于 [dreamhunter2333/cloudflare_temp_email](https://github.com/dreamhunter2333/cloudflare_temp_email) 修改。以后需要继续开发或同步上游大版本时，直接克隆本仓库即可：

```bash
git clone git@github.com:yangzhe0/project_temp_email.git
```

## 已保留的两项改动

### Telegram 消息

- Telegram 命令说明改为只显示中文。
- 长消息按 Telegram 的单条消息长度限制分段发送，避免上下文或邮件内容被截断。

### 前端邮件 ID

- 邮件列表使用新的显示序号列（从 1 开始），按当前列表顺序重新编号。
- 这个显示序号不依赖数据库原始 ID，因此删除邮件后仍然连续。

具体的新需求以后按实际情况单独评估，不把本次运行数据、密钥或邮件备份放进仓库。
