# 户用离网光伏发电系统 · 课程设计

本仓库用于 **2026 年专业课程创新研修——户用离网光伏发电系统课程设计** 的多人协作与资料共享。

## 📁 目录结构

```
├── README.md                      # 本说明（协作指南）
└── docs/                          # 课程设计文档资料
    ├── 任务1-设计指导书-户用离网光伏发电系统.docx
    ├── 任务1-课程设计任务书-户用离网光伏发电系统.docx
    ├── 任务1-进度检查与考核标准-户用离网光伏发电系统.docx
    ├── 实验测试.doc
    └── 本科毕业论文（设计）书写范例（理工类）.doc
```

## 👀 查看（无需任何操作）

公开仓库，任何人都可以直接在网页上浏览、下载所有文件：
`https://github.com/<owner>/offgrid-pv-course-design`

## ✏️ 多人编辑（三种方式）

### 方式一：作为协作者直接编辑（推荐给固定小组成员）

1. 仓库管理员在 **仓库 → Settings → Collaborators and teams** 中添加成员 GitHub 用户名；
2. 协作者把仓库克隆到本地：
   ```bash
   git clone https://github.com/<owner>/offgrid-pv-course-design.git
   ```
3. 改完文件后提交并推送：
   ```bash
   git add .
   git commit -m "说明改了什么"
   git push
   ```

### 方式二：Fork + Pull Request（适合临时参与或公开投稿）

1. 在仓库页面点 **Fork**，得到自己的副本；
2. 克隆自己的副本修改、提交、推送；
3. 回到原仓库点 **New Pull Request**，请求合并你的修改。

### 方式三：网页直接编辑（适合小改动）

GitHub 网页上打开任意文件 → 点 ✏️ 编辑 → 修改 → **Commit changes**（协作者可直接提交；非协作者会自动创建 Pull Request）。

## 🤝 协作规范（建议）

- **不要直接往 `main` 分支推**。每个成员开自己的分支：
  ```bash
  git checkout -b 姓名/功能名
  ```
  完成后发起 Pull Request 合并，便于追溯谁改了什么。
- 提交信息写清楚「改了什么、为什么」。
- 每次开始工作前先 `git pull` 拉取最新版本，避免冲突。
- 冲突不可避免时，先 `git pull`，按提示手动解决冲突文件后再提交。

## 🔧 常用命令速查

| 操作 | 命令 |
|------|------|
| 克隆仓库 | `git clone https://github.com/<owner>/offgrid-pv-course-design.git` |
| 查看状态 | `git status` |
| 拉取最新 | `git pull` |
| 提交本地 | `git add .` → `git commit -m "描述"` |
| 推送到远端 | `git push` |
| 查看历史 | `git log --oneline` |

## 📌 说明

- 文档为课程设计原始资料，请勿随意删改他人文件；大改动建议先讨论。
- 遇到问题请在仓库 **Issues** 里提出。
