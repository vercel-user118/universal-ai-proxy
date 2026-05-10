
markdown
# 通用人工智能代理 (universal-ai-proxy)

一个万能大模型代理接口，支持一键切换调用 DeepSeek 等主流大模型，兼容 OpenAI API 格式。

## ✨ 功能特点
- 统一接口格式：兼容 OpenAI API 规范，无需修改客户端代码即可接入
- 多模型支持：通过 `model` 参数自由切换不同大模型服务
- 安全密钥管理：API Key 存储在环境变量中，避免代码泄露风险
- 一键部署：支持 Vercel 平台快速部署，开箱即用

## 🚀 快速开始

### 1. 部署方式
本项目已部署在 Vercel 平台，访问地址：
`https://universal-ai-proxy.vercel.app`

### 2. 环境变量配置
项目根目录 `.env` 文件已配置 DeepSeek API Key：
```env
# DeepSeek API Key
DEEPSEEK_KEY=sk-f99xxxxxx
3. 调用示例
bash
运行
curl -X POST https://universal-ai-proxy.vercel.app/api/route \
-H "Content-Type: application/json" \
-d '{
  "model": "deepseek-chat",
  "messages": [{"role": "user", "content": "你好！请介绍一下自己"}]
}'
📌 支持的模型
表格
model 名称	对应大模型
deepseek-chat	DeepSeek 对话模型
📄 许可证
MIT License
plaintext

---

### 📝 使用说明
1.  点击 GitHub 仓库里的「添加 README 说明」按钮
2.  清空默认内容，粘贴上面的模板
3.  把 `sk-f99xxxxxx` 替换成你自己的 DeepSeek API Key（也可以留空，只保留格式）
4.  点击「提交变更」完成添加



PPT 生成

更多

