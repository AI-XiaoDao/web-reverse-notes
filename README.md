# Web 协议逆向实战笔记

网站协议逆向与纯算复现的实战经验，整理成一个可复用的 Codex Skill。

## 内容

- **五条核心原则**：抓包基线、逐字节验证、对照实验、真实样本、指纹分层
- **12 步工作流**：干净会话 → 反复触发 → 逐参数溯源 → 定位 JS → 算法还原 → 重写 → 补环境 → 纯算模拟 → HTTP/WS 复现 → 验证 → 回归
- **11 条真实踩坑**：dfp 矛盾、UA-CH、固定 cookie、首帧语义、dt 栅格等
- **验收清单**：7 项可勾选检查
- **案例索引**：爱奇艺短信登录的关键结论

## 使用

### 方式一：克隆后安装

```bash
git clone https://github.com/AI-XiaoDao/web-reverse-notes.git
mkdir -p ~/.codex/skills/web-reverse-notes
cp web-reverse-notes/SKILL.md ~/.codex/skills/web-reverse-notes/
```

### 方式二：手动复制

打开仓库页面，复制 `SKILL.md` 内容，保存到：

```text
~/.codex/skills/web-reverse-notes/SKILL.md
```

之后在相关任务（前端签名、加密参数、滑块、设备指纹、短信登录）中会自动匹配。

## 结构

```text
SKILL.md    完整笔记（工作流 / 原则 / 踩坑 / 验收）
README.md   本文件
```

## 说明

本仓只包含方法与经验，**不含**任何凭证、手机号、cookie、抓包样本或可执行攻击代码。
