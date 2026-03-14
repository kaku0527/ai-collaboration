# 任务 #005：配置 GitHub 并推送文件

## 任务背景
您已完成本地文件准备，现在需要推送到 GitHub。

## 任务目标
1. 配置 GitHub 认证
2. 将本地文件推送到 GitHub

## 第一步：配置 GitHub Token

### 如果已有 Token
在 OpenCLAW 配置文件中更新 token：
文件路径：D:\Clawopen\.openclaw\openclaw.json

内容：
```json
{
  "github": {
    "token": "YOUR_GITHUB_TOKEN",
    "username": "kaku0527"
  }
}
```

### 如果没有 Token
1. 访问 https://github.com/settings/tokens
2. 点击 "Generate new token (classic)"
3. 勾选 `repo` 权限
4. 生成并复制 token

## 第二步：推送文件

在本地 Git 仓库执行：
```bash
cd D:\GoogleAdManager-KnowledgeBase\3月14日github文件
git init
git remote add origin https://github.com/kaku0527/ai-collaboration.git
git pull origin main --allow-unrelated-histories
git add .
git commit -m "Add knowledge base files"
git push origin main
```

## 第三步：验证结果

推送完成后，验证 GitHub 仓库：
```
https://api.github.com/repos/kaku0527/ai-collaboration/contents/data
```

## 输出要求

在 results 目录创建 `task_005_result.md`，记录：
- 是否成功配置
- 推送了哪些文件
- 遇到的错误（如有）
