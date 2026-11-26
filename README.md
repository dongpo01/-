# 谈吐素养 · 经典训练系统

以历史、人文、古诗词、典故与全球经典为素材，系统提升谈吐素养与口才的在线训练工具。

在线体验（部署后替换为你的 GitHub Pages 地址）：
**https://你的用户名.github.io/tantu-training/**

---

## 功能概览

| 模块 | 说明 |
|------|------|
| **经典素材库** | 270+ 条精选素材，支持按类别、场景、难度筛选与搜索 |
| **场景化练习** | 金句嵌入、即兴发言、辩论反驳、角色扮演、结构模板、快速反应等 |
| **即时反馈** | 自动检测素材使用、结构完整性，给出得分与改进建议 |
| **练习记录** | 本地保存历史成绩（浏览器本地存储） |

## 素材覆盖

- 古诗词金句
- 典故与成语
- 诸子百家与经典语录
- 史传与人物对话
- 全球经典名言
- 职场 / 演讲 / 辩论专项补充

## 快速开始（本地预览）

```bash
# 克隆仓库
git clone https://github.com/你的用户名/tantu-training.git
cd tantu-training

# 直接用浏览器打开
open index.html
# 或使用任意静态服务器
npx serve .
```

## 部署到 GitHub Pages

1. 在 GitHub 新建仓库，命名为 `tantu-training`（或任意名称）
2. 将本目录所有文件推送到仓库的 `main` 分支：

```bash
git init
git add .
git commit -m "Initial commit: 谈吐素养经典训练系统"
git branch -M main
git remote add origin https://github.com/你的用户名/tantu-training.git
git push -u origin main
```

3. 打开仓库 **Settings → Pages**
4. Source 选择 `Deploy from a branch`
5. Branch 选择 `main`，目录选择 `/ (root)`
6. 点击 Save，等待 1–2 分钟即可通过  
   `https://你的用户名.github.io/tantu-training/` 访问

> 如果仓库名不是 `username.github.io`，访问路径会带上仓库名。

## 目录结构

```
tantu-training/
├── index.html              # 主页面（可独立运行）
├── README.md
└── data/                   # 完整数据（可选扩展用）
    ├── phase1_materials.json
    ├── exercises_batch1.json
    └── scoring_config.json
```

当前 `index.html` 已内嵌精简数据，**无需额外配置即可直接使用**。  
`data/` 目录中的 JSON 为完整版素材与练习，方便后续二次开发。

## 技术说明

- 纯静态 HTML / CSS / JavaScript，无后端依赖
- 兼容现代浏览器（Chrome / Edge / Firefox / Safari）
- 使用 `localStorage` 保存练习记录（沙箱环境自动降级为内存存储）

## 后续可扩展方向

- 接入完整 JSON 数据动态加载
- 增加语音输入与评测
- 用户账号与云端同步
- 更精细的六维能力雷达与成长曲线
- 深色模式 / 多语言

## 许可

本项目内容基于中国古典文献与公开经典语录整理，仅供学习交流使用。  
代码部分可自由使用与修改。

---

**腹有诗书气自华。** 愿这个小工具能帮你把经典真正用到嘴边。
