# 测试任务 #001

## 任务类型
GitHub API 测试

## 任务内容

请使用 WebFetch 工具执行以下操作：

### 任务 1：获取仓库信息
访问以下 URL 并返回 JSON 响应：
```
https://api.github.com/repos/kaku0527/ai-collaboration
```

### 任务 2：读取 README
访问以下 URL 并返回内容：
```
https://raw.githubusercontent.com/kaku0527/ai-collaboration/main/README.md
```

## 输出要求

将任务执行结果写入：
`results/test_result_001.md`

格式如下：
```markdown
# 测试结果 #001

## 任务 1：仓库信息
[在此粘贴 JSON 响应]

## 任务 2：README 内容
[在此粘贴 README 内容]

## 执行状态
- 状态：✅ 成功 / ❌ 失败
- 执行时间：[时间戳]
```

## 备注
这是第一次交互测试，请确认 GitHub 读取功能正常工作。
