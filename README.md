# 🎼 Lenzinsel乐队乐谱版本管理仓库

这是一个为Lenzinsel乐队成员共同使用的**乐谱管理与版本控制仓库**。
我们使用 **MuseScore** 进行乐谱的查看与编辑，并通过 **Git** 实现多人协作与版本管理。

---

## 🧰 使用工具

* **MuseScore（乐谱编辑软件）**
  官网：https://musescore.org/

* **Git（版本控制工具）**
  官网：https://git-scm.com/

---

## 🚀 初次使用

1. **安装工具**

   * 安装 MuseScore
   * 安装 Git

2. **克隆仓库到本地**

   ```bash
   git clone 仓库地址
   cd 仓库名
   ```

3. 使用 MuseScore 打开 `.mscz` 乐谱文件即可开始查看或编辑。

---

## 🔊 音色配置（SoundFonts）

为了保证所有成员播放效果一致，请进行如下设置：

  ```bash
  打开 MuseScore
  进入：
  Edit编辑 → Preferences偏好设置 → 文件夹 → 声音字体SoundFonts
  将 声音字体SoundFonts 文件夹路径修改为本仓库中的 soundfonts 文件夹
  ```

这样可以确保大家使用相同的音色进行播放与导出 🎧

---

## ✏️ 修改乐谱流程

为了保证协作清晰，请按照以下流程进行修改：

### 1. 新建分支

分支命名格式：

```text
曲名-修改内容
```

示例：

```text
la-gloire-调整节奏
songA-添加鼓组
```

创建并切换分支：

```bash
git checkout -b 分支名
```

---

### 2. 修改乐谱

* 使用 MuseScore 打开 `.mscz` 文件
* 在软件内完成修改
* 保存文件

---

### 3. 提交更改

```bash
git add .
git commit -m "描述你的修改内容"
```

示例：

```bash
git commit -m "调整副歌节奏"
```

---

### 4. 推送分支并创建 PR

```bash
git push origin 分支名
```

然后在 GitHub 上：

* 创建 Pull Request（PR）
* 简要说明本次修改内容

---

### 5. Review & 合并

* 其他成员进行 Review
* 确认无问题后合并到主分支（main）

---

## 📌 协作建议

* 尽量避免多人同时修改同一首曲子
* 修改前先拉取最新代码：

  ```bash
  git pull
  ```
* 提交信息写清楚修改内容，方便追踪版本

---

## 🎯 目标

* 统一管理乐队所有乐谱
* 清晰记录每一次修改
* 提高协作效率，避免文件混乱

---

如有问题或建议，欢迎随时提出 🎵
