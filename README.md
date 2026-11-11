# 数据分析与可视化 — 学生项目展示

2026 秋季课程学生项目展示网站（公开路演公众入口）。

线上地址：<https://haichaozheng.github.io/data-analysis-showcase>

## 技术栈

纯静态 HTML + CSS，无构建步骤。直接推送到 GitHub Pages 即可上线。

## 页面清单

| 页面 | 说明 |
|---|---|
| index.html | 首页：hero + 六大入口卡片 |
| intro.html | 课程简介：目标、PBL+DSR、一人公司、AI 工具栈、选题三档、评分结构 |
| timeline.html | 项目之旅：17 周 4 阶段里程碑（含版本徽章 v0.1→v1.1） |
| rules.html | 课程公约：师生共建准则 |
| projects.html | 精彩项目：学生作品展示 + W16 路演信息 |
| resources.html | 课程资源：课件、代码与数据集 |
| news.html | 产业新闻：数据分析领域动态 |

## 维护约定

### 导航与页脚

导航栏与页脚在所有页面中**重复**。修改导航或页脚时，需同步更新全部 HTML 文件的 `<nav>...</nav>` 与 `<footer>...</footer>` 区块。

### 新增项目卡片（projects.html）

复制下方模板，填入内容后放在 projects.html 的 `.project-grid` 容器内：

```html
<div class="project-card">
    <div class="project-card-head">
        <div class="project-card-title">项目名称</div>
        <span class="badge badge-live">已上线</span>
    </div>
    <div class="project-card-author">作者</div>
    <div class="project-links">
        <a href="#" target="_blank" rel="noopener">项目仓库</a>
    </div>
</div>
```

#### 状态徽章

- `badge-progress` 进行中（黄）
- `badge-live` 已上线（绿）
- `badge-demo` 仅 Demo（橙）

### 新增新闻条目（news.html）

news.html 内已内置注释模板，复制后填入内容、置于 `.news-list` 顶部即可。

## 本地预览

```bash
python -m http.server 8000
```

浏览器访问 <http://localhost:8000/index.html>
