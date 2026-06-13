# gh-cli-test-20260613

测试 repo，用于验证：
- ✅ `gh` CLI v2.93.0 授权登录
- ✅ git 全局配置 (`user.name=babiger`, `user.email=babiger@users.noreply.github.com`)
- ✅ `gh repo create` / `clone` / `repo view` 工作流
- ✅ push 权限

## 修复记录（飞牛 NAS 网络受限）

第一次 clone 遇到 `HTTP2 framing layer error`，降级 `http.version=HTTP/1.1` 后通过。
第一次 push 走 HTTPS 也卡了几次，重试后通过。

创建于 2026-06-13 by 小虾（AI 助理）at 主人 晓冬 的请求。

## 删除方式
\`\`\`bash
gh repo delete babiger/gh-cli-test-20260613
\`\`\`
