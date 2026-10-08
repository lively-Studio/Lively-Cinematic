# Lively-Cinematic · 灵动电影

> 电影风格光影 · 高对比 · 暗角 · 景深 · 电影感

---

## 项目简介

**Lively-Cinematic** 是一套基于 Complementary Reimagined r5 代码，专为 Minecraft Java 版打造的电影风格光影包。  
强调高对比度、暗角、镜头光晕、景深与动态模糊，营造沉浸式影片级视觉体验。

设计理念：

> *"让每一帧都像电影画面"*

---

## 核心特性

### 镜头 & 后期
- **高对比度调色**：对比度 1.30 · 饱和度 1.10 · 淡色饱和 0.90
- **暗角效果**：为画面边缘添加暗角，聚焦中心视野
- **镜头光晕**：面向太阳时产生镜头反射效果
- **动态模糊**：镜头移动时产生运动模糊，增强电影感
- **色散效果**：色彩通道分离，模拟镜头畸变
- **泛光**：亮度 0.12，明亮物体产生柔和的辉光

### 光照 & 大气
- **全局曝光 0.85**：略暗的画面基调，符合电影风格
- **大气雾 1.00**：强化纵深感
- **大气雾距离 80**：更早出现的雾效
- **洞穴光照 10**：极低的洞穴光照，营造黑暗氛围
- **阴影亮度 80**：更深的阴影区域
- **自定义光色曲线**：日出暖调 · 夜晚冷调 · 雨天阴郁调

### 水面 & 云层
- **无界水面**：自然波纹 · 动态折射
- **高品质云层**：体积感云渲染
- **彩虹**：雨后的视觉点缀

### 兼容性
- **Mac 兼容**：Apple Silicon 色彩模拟
- **零依赖**：开箱即用

---

## 关键参数

| 参数 | 值 | 说明 |
|------|-----|------|
| SHADER_STYLE | 4 | 无界视觉风格 |
| ATM_FOG_MULT | 1.00 | 大气雾强度 |
| ATM_FOG_DISTANCE | 80 | 雾效起始距离 |
| BLOOM_STRENGTH | 0.12 | 泛光强度(65%) |
| MOTION_BLUR_EFFECT | 1 | 动态模糊开启 |
| CHROMA_ABERRATION | 2 | 色散强度 |
| LENSFLARE_MODE | 1 | 镜头光晕(仅太阳) |
| CAVE_LIGHTING | 10 | 洞穴光照 |
| AMBIENT_MULT | 80 | 阴影亮度 |
| HAND_SWAYING | 2 | 手臂晃动(普通) |
| TM_EXPOSURE | 0.85 | 全局曝光 |
| TM_CONTRAST | 1.30 | 全局对比度 |
| T_SATURATION | 1.10 | 饱和度 |
| T_VIBRANCE | 0.90 | 淡色饱和 |

---

## 快速开始

### 安装

1. 下载 `Lively-Cinematic-Shader.zip`
2. 放入 `.minecraft/shaderpacks/`（或你的 Fabric 实例目录）
3. 在 Iris 设置中选择 "Lively-Cinematic"
4. 搭配 PBR 材质包获得更佳效果

### 推荐设置

| 设置项 | 推荐值 | 说明 |
|--------|--------|------|
| 视觉风格 | 无界 | 最佳电影感效果 |
| 模拟色彩光照 | 真实色彩 | Mac 专属彩色光源替代 |
| 动态模糊 | 开启 | 增强电影运动感 |
| 暗角 | 开启 | 聚焦中心画面 |
| 镜头光晕 | 仅太阳 | 电影级镜头效果 |

---

## 开发信息

### 技术栈
- **基础架构**：Complementary Reimagined r5
- **GLSL 版本**：`#version 130`（macOS ARM 兼容）
- **包装格式**：`shaders/` 前缀 zip

### macOS 注意事项
- `COLORED_LIGHTING`（彩色光源）在 Mac 上不可用，已用 `COLOR_LIGHT_MODE` 替代
- 打包时必须保持 `shaders/` 目录结构前缀

---

## 许可

GNU General Public License v3.0 · Lively-Studio

---

**Lively-Cinematic · 灵动电影** — Lively Studio (「零」影制作组) 出品 — 让每一帧都是电影
