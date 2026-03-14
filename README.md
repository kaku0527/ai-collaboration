# AI 协作仓库

这是 CodeBuddy 与 OpenCLAW 之间的协作仓库。

## 目录说明
- `instructions/` - 任务指令（CodeBuddy 写入）
- `results/` - 执行结果（OpenCLAW 写入）
- `data/` - 共享数据
- `status/` - 状态文件

## 协作流程
1. CodeBuddy 在 `instructions/` 创建任务
2. OpenCLAW 读取并执行
3. 结果写入 `results/`
4. CodeBuddy 读取结果并继续
