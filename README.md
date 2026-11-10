# 汴京四时 · Bianjing Seasons

以张择端《清明上河图》为底本的沉浸式数字艺术长卷。在汴河、市井与郊野之间缓慢漫游，静观四季、昼夜与雨雪流转。

[在线体验](https://shen-dongshan.github.io/bianjing-sishi/) · [下载 V14_bianjing](https://github.com/Shen-Dongshan/bianjing-sishi/releases/tag/V14_bianjing) · [完整更新日志](CHANGELOG.md) · [反馈问题](https://github.com/Shen-Dongshan/bianjing-sishi/issues)

## 项目概览

- **主站**：https://shen-dongshan.github.io/bianjing-sishi/
- **当前版本**：`V14_bianjing`（V14 · 画中闲话与流畅漫游）
- **作者**：[Shen Dongshan](https://github.com/Shen-Dongshan)
- **发布日期**：2026-11-10（Europe/Budapest）
- **形式**：全屏横向数字长卷，桌面与移动端均可浏览。

## 主要功能

- 横向拖动、滚轮漫游、平滑缩放、自动游览及可拖动的底部长卷缩略导航；暂停时可点击中央半透明图标继续。
- 36处场景、67个人物点位及251组对白覆盖全卷，含4处阁楼场景；轻量半透明气泡随人物坐标移动，最多两组，虹桥节奏放缓。
- 手机自动档以60帧为目标，按设备负载调整清晰度，提供自动、清晰优先、省电三档；实际帧率取决于设备。
- 春、夏、秋、冬四幅 38414 × 1800 AI 辅助重绘底图，按视口加载多分辨率瓦片，并保留原卷静赏。
- 清晨、正午、黄昏、夜晚与四季组成 16 个状态，每 30 秒推进一次，可手动切换或暂停自动流转。
- 细雨、大雨、粉雪与远近分层天气；春夏随机一个时辰落雨，冬季默认飘雪。
- 场景、季节、时辰与天气共同调节环境音；六首配乐随机直接切换，音乐与环境音独立控制。
- 18 段场景标题、16 首宋代诗词、素纸展卷入场、沉浸模式与统一宋体字形。
- 开放世界仍在开发中，当前入口禁用；自由浏览与自动漫游正常开放。

## 使用与下载

### 在线浏览

打开[汴京四时主站](https://shen-dongshan.github.io/bianjing-sishi/)，点击画卷展开。该次点击用于启用声音，展开后开始自动漫游。

| 操作 | 方式 |
| --- | --- |
| 漫游 | 鼠标或单指拖动；滚轮、触摸板滑动 |
| 缩放 | Ctrl / ⌘ + 滚轮；双指缩放；页面加减按钮 |
| 自动游览 | 页面底部暂停 / 继续，支持三档速度；暂停后也可点击画面中央继续 |
| 缩略导航 | 点击或拖动底部长卷，保持当前缩放 |
| 人物对白与画质 | “调息”中可关闭对白，并选择自动、清晰优先或省电 |
| 四季与昼夜 | 右侧四季、顶部时辰；在“调息”中控制自动流转 |
| 声音与天气 | 在“调息”中分别调节音乐、环境音、音量及天气 |
| 沉浸 | 页面沉浸按钮；Esc 返回 |

### 本地运行

从 [Releases](https://github.com/Shen-Dongshan/bianjing-sishi/releases/tag/V14_bianjing) 下载 `site.zip` 并解压。该包包含完整可运行网页、画卷瓦片、字体、配乐与环境音，共 1824 个文件。

在解压目录启动任意静态 HTTP 服务。例如已安装 Python 3 时：

```bash
python -m http.server 8000
```

随后访问 `http://localhost:8000`。无需前端依赖安装或额外构建；ES Modules 与资源请求需要 HTTP 服务。

请选择发行版附件 `site.zip`；GitHub 自动生成的 Source code 压缩包对应仓库中的文档与发布配置。

```text
SHA-256 (site.zip)
12406409c1005e96d7fe6b331eaf04a88a915cc0abe7aa900aea6c9077e9698a
```

## 作者与制作

| 内容 | 署名 |
| --- | --- |
| 网站作者、项目策划与艺术指导 | Shen Dongshan |
| 界面设计与开发协作 | Codex（OpenAI） |
| 四季长卷与行者素材制作 | 项目方与 AI 绘图工具 image_gen 协作 |
| 原作 | 北宋 · 张择端《清明上河图》，原作藏故宫博物院 |

## 素材版权与来源

各类素材分别遵循其来源记录与许可。原作数字复制图的公有领域标记不延伸至配乐、其他音效或当代四季重绘；仓库公开展示不表示全部素材采用同一开源许可。

### 原画与四季重绘

- **数字底本**：[Wikimedia Commons · Alongtheriver QingMing.jpg](https://commons.wikimedia.org/wiki/File:Alongtheriver_QingMing.jpg)，38414 × 1800；来源页标注 PD-Art / [Public Domain Mark 1.0](https://creativecommons.org/publicdomain/mark/1.0/)，复制图来源记为 Baidu Tieba。
- **四季图像**：参考原卷及项目方确认的虹桥四季样张，经 224 个 AI 分区编辑、配准与接缝整理形成四幅完整长卷。
- 四季底图、行者、夜景和局部动画为当代艺术演绎。AI 重绘局部的人物、建筑和自然细节可能与原作不同；可使用“原卷静赏”对照。
- 相关制作与来源记录随网页资源保存在 `assets/ATTRIBUTION.md`、`assets/seasons-direct/PROVENANCE.json` 及站内作者版权说明中。

### 背景配乐

专辑：**《古剑奇谭三》音乐集·天予风流**。参与创作的艺术家：**上海烛龙**。曲名、艺术家与专辑名据项目方提供的录音文件元数据记录。

| 曲目 | 署名与来源 |
| --- | --- |
| 采桑子 | 上海烛龙 · 上述专辑；项目方提供录音 |
| 花下重门（Live） | 上海烛龙 · 上述专辑；项目方提供录音 |
| 澄心若璃（Live） | 上海烛龙 · 上述专辑；项目方提供录音 |
| 山月调（Live） | 上海烛龙 · 上述专辑；项目方提供录音 |
| 春芜长·变调 | 上海烛龙 · 上述专辑；项目方提供录音 |
| 鹿饮银溪（Live） | 上海烛龙 · 上述专辑；项目方提供录音 |

词曲、演奏及录音等权利归相应权利人。公开播放与再分发的授权范围尚待项目方补充；本项目不向下载者授予这些录音的额外使用许可。录音摘要见 `assets/music/manifest.json`。

### 环境音与原创拟音

19 条下载素材结合项目原创的更鼓、枯叶与踏雪程序拟音，按画面内容组合播放。现代录音、拟音和 AI 音效均用于艺术化音景。

其中 18 条按来源页记录标注为 CC0 1.0。中文古风叫卖来自趣听科技公开试听页，原页标示版权所有；公开使用及再分发授权范围待核实，非 CC0。

<details>
<summary>查看全部 19 条环境音素材及作者</summary>

| 素材 | 作者 / 原页署名 | 来源与许可记录 |
| --- | --- | --- |
| 缓水拍岸（现代码头野录） | Joseph SARDIN | [来源](https://bigsoundbank.com/pontoon-marina-s1444.html) · [CC0 1.0](https://bigsoundbank.com/licenses.html) |
| 细流流水 | Joseph SARDIN | [来源](https://bigsoundbank.com/small-stream-s0823.html) · [CC0 1.0](https://bigsoundbank.com/licenses.html) |
| 草叶风声 | Joseph SARDIN | [来源](https://bigsoundbank.com/wind-in-tall-grass-s0908.html) · [CC0 1.0](https://bigsoundbank.com/licenses.html) |
| 晨间群鸟 | Joseph SARDIN | [来源](https://bigsoundbank.com/wake-birds-3-s0999.html) · [CC0 1.0](https://bigsoundbank.com/licenses.html) |
| 暮鸟低鸣 | Joseph SARDIN | [来源](https://bigsoundbank.com/evening-birds-s1859.html) · [CC0 1.0](https://bigsoundbank.com/licenses.html) |
| 夜虫鸣 | Joseph SARDIN | [来源](https://bigsoundbank.com/insect-song-4-s3187.html) · [CC0 1.0](https://bigsoundbank.com/licenses.html) |
| 夏日群蝉 | Clarisse | [来源](https://bigsoundbank.com/cicadas-s3002.html) · [CC0 1.0](https://bigsoundbank.com/licenses.html) |
| 细雨（伞下收音） | Pierre SIBANARCO | [来源](https://bigsoundbank.com/rain-under-an-umbrella-s2679.html) · [CC0 1.0](https://bigsoundbank.com/licenses.html) |
| 骤雨与远雷 | Joseph SARDIN | [来源](https://bigsoundbank.com/rain-and-storm-s0124.html) · [CC0 1.0](https://bigsoundbank.com/licenses.html) |
| 水洼落雨 | Joseph SARDIN | [来源](https://bigsoundbank.com/rain-on-puddle-s1290.html) · [CC0 1.0](https://bigsoundbank.com/licenses.html) |
| 路径马蹄 | Joseph SARDIN | [来源](https://bigsoundbank.com/horse-walking-on-a-path-s1854.html) · [CC0 1.0](https://bigsoundbank.com/licenses.html) |
| 缓慢划水（木板水箱拟音） | Joseph SARDIN | [来源](https://bigsoundbank.com/rowing-slowly-s1514.html) · [CC0 1.0](https://bigsoundbank.com/licenses.html) |
| 碎石土路脚步 | Joseph SARDIN & Axeline T. | [来源](https://bigsoundbank.com/footsteps-on-gravels-4-s3216.html) · [CC0 1.0](https://bigsoundbank.com/licenses.html) |
| 木地板脚步 | DavidGreck | [来源](https://bigsoundbank.com/man-footsteps-on-the-wooden-floor-s0165.html) · [CC0 1.0](https://bigsoundbank.com/licenses.html) |
| 鸡鸣报晓 | DenisChardonnet | [来源](https://bigsoundbank.com/song-of-rooster-s0283.html) · [CC0 1.0](https://bigsoundbank.com/licenses.html) |
| 木门开合 | Joseph SARDIN | [来源](https://bigsoundbank.com/opening-and-closing-light-door-s0377.html) · [CC0 1.0](https://bigsoundbank.com/licenses.html) |
| 远处市井低语（下载的 AI 音效） | SFXMint / flreey | [来源](https://sfxmint.com/sounds/market-ambience-02) · [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) |
| 旧马车行进（公开 HQ 试听版） | bruno.auzet | [来源](https://freesound.org/people/bruno.auzet/sounds/538438/) · [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) |
| 中文古风街头叫卖 | 趣听科技（原页版权方；配音演员未注明） | [来源](https://kukabala.com/home/play?audio_id=2849) · 版权所有；授权范围待核实 |

</details>

来源与录制类型逐项保存在 `assets/audio/immersive/PROVENANCE.json`；远处市井低语属于下载的 AI 音效，缓慢划水为现代拟音。

### 字体、诗词与界面

- **字体**：内置 Bianjing Serif，基于 Google / Adobe 的 [Noto Serif CJK SC Regular](https://github.com/notofonts/noto-cjk/tree/main/Serif)提取网站所需字形子集并更名，保持原始轮廓，采用 [SIL Open Font License 1.1](https://shen-dongshan.github.io/bianjing-sishi/assets/fonts/OFL.txt)。许可与来源记录随资源包保留。
- **诗词**：节选 16 首宋代诗词，保留原作者、篇名和原文来源。四季、时辰与诗作的配对属于展览编排，不表示原诗描写汴京或画中人物。
- **标志与界面**：四季色印、素纸展卷、页面界面和天气动画由 Shen Dongshan 策划并与 Codex 协作设计、实现。

<details>
<summary>查看 16 首诗词的作者与出处</summary>

| 季节 | 时辰 | 作者与作品 |
| --- | --- | --- |
| 春 | 清晨 | [宋祁《玉楼春·春景》](https://www.gushiwen.cn/mingju/juv_1c7403a5ab73.aspx) |
| 春 | 正午 | [秦观《行香子·树绕村庄》](https://www.gushiwen.cn/shiwenv.aspx?id=8005cc89b888) |
| 春 | 黄昏 | [苏轼《惠崇春江晚景》](https://zh.wikisource.org/zh-hans/惠崇春江晚景) |
| 春 | 夜晚 | [王安石《春夜》](https://zh.wikisource.org/zh-hans/春夜_(王安石)) |
| 夏 | 清晨 | [杨万里《晓出净慈寺送林子方》](https://zh.wikisource.org/zh-hans/晓出净慈寺送林子方) |
| 夏 | 正午 | [苏舜钦《夏意》](https://zh.wikisource.org/wiki/Page:Sibu_Congkan0825-蘇舜欽-蘇學士文集-3-1.djvu/163) |
| 夏 | 黄昏 | [秦观《纳凉》](https://www.gushiwen.cn/mingju/juv_ab1a0b87feee.aspx) |
| 夏 | 夜晚 | [辛弃疾《西江月·夜行黄沙道中》](https://www.gushiwen.cn/gushiwen_4bd68017ff.aspx) |
| 秋 | 清晨 | [陆游《秋夜将晓出篱门迎凉有感二首·其一》](https://m.gushiwen.cn/mingju/juv_ebbbf236246c.aspx) |
| 秋 | 正午 | [范仲淹《苏幕遮·怀旧》](https://zh.wikisource.org/zh-hans/蘇幕遮_(范仲淹)) |
| 秋 | 黄昏 | [秦观《满庭芳·山抹微云》](https://www.gushiwen.cn/mingju/juv_0371eb5cbe86.aspx) |
| 秋 | 夜晚 | [苏轼《阳关曲·中秋月》](https://www.gushiwen.cn/shiwenv_76c8331c8937.aspx) |
| 冬 | 清晨 | [陆游《除夜雪》](https://www.gushiwen.cn/shiwenv_2d803c7ec16d.aspx) |
| 冬 | 正午 | [王安石《梅花》](https://www.gushiwen.cn/shiwenv_846e626d74d3.aspx) |
| 冬 | 黄昏 | [林逋《山园小梅二首·其一》](https://www.gushiwen.cn/mingju.aspx?id=885) |
| 冬 | 夜晚 | [杜耒《寒夜》](https://zh.wikisource.org/zh-hans/寒夜_(杜耒)) |

</details>

### 画中闲话

人物称谓、对话与季节天气反应由本项目创作，属于艺术化演绎，非史料原文，也不代表画中人物的真实身份。点位按四季底图逐场景校准；枝叶遮挡的人物按季节停用。

### 使用说明与致谢

原创内容署名：© 2026 Shen Dongshan。第三方素材的作者与授权范围以上述逐项记录为准；如需复用，请核对对应素材的许可与权利人授权。

体验参考：[xianxie6 / qingming-riverside](https://github.com/xianxie6/qingming-riverside)。感谢原作、数字复制图、字体、音景与配乐的创作者及资料提供者。

## 更新日志

### V14_bianjing · 2026-11-10

- 新增覆盖全卷的轻量人物对白、四处阁楼场景与四季人物点位校准；半透明小号气泡保持人物坐标，缩短连线并避开边缘。
- 对话分布更均匀，虹桥节奏放缓，保留最多两组及场景冷却。
- 提高手机默认画质与流畅度，复用高清缓冲，增加三档画质控制。
- 支持拖动缩略长卷、点击中央半透明图标继续漫游；标签页标题简化为“汴京四时”。
- 完整保留原尺寸四季图、全部高清瓦片、六首配乐与含中文叫卖的19条环境音；开放世界仍在开发中。

[V14 完整记录](docs/releases/V14.md) · [全部开发日志](CHANGELOG.md)


### V13_bianjing · 2026-11-08

- 开放世界以“开发中”显示，原生按钮禁用，点击与模式处理另有关闭状态保护；继续提供自由漫游、缩放与四时音景。
- 发布内置宋体Bianjing Serif，桌面与手机使用同一字形；原始Noto Serif CJK SC字体、OFL 1.1许可和取字形子集记录保留。
- 手机使用1.25倍像素上限及总像素预算，自动漫游目标24帧、操作30帧、环境18帧；复用静止底图，减少粒子、局部变形和图像缓存。
- 未展卷、关闭动画的暂停画面与隐藏页面避免持续重绘；隐藏页面暂停音频上下文。手机尺寸浏览器实测自动漫游约22帧，静止时全屏重绘为0；不是实际手机表面温度测试。
- 同步发布素纸双卷、悬停微启、自然阴影、白天墨色标题、透视雨雪和44处新增室内灯光。

[V13 完整记录](docs/releases/V13.md) · [全部开发日志](CHANGELOG.md)

### 历史正式版本

| 版本 | 发布日期 | 更新主题 |
| --- | --- | --- |
| [V14](docs/releases/V14.md) | 2026-11-10 | 画中闲话与流畅漫游 |
| [V13](docs/releases/V13.md) | 2026-11-08 | 素纸展卷与移动端优化 |
| [V12](docs/releases/V12.md) | 2026-11-07 | 展卷入宋与沉浸音景 |
| [V11](docs/releases/V11.md) | 2026-11-06 | 原尺寸AI四季全卷与自动漫游 |
| [V10](docs/releases/V10.md) | 2026-11-04 | 四季原卷细节保真与原尺寸高清层 |
| [V09](docs/releases/V09.md) | 2026-11-04 | 六首背景音乐随机连播 |
| [V08](docs/releases/V08.md) | 2026-11-03 | 完整长卷加载保护 |
| [V07](docs/releases/V07.md) | 2026-11-03 | 四季全卷与取消试览 |
| [V06](docs/releases/V06.md) | 2026-11-03 | 虹桥试览加载保护 |
| [V05](docs/releases/V05.md) | 2026-11-03 | 虹桥四季AI局部试览 |
| [V04](docs/releases/V04.md) | 2026-11-03 | 环境微动与昼夜系统 |
| [V03](docs/releases/V03.md) | 2026-10-31 | 城内出发与位置音景 |
| [V02](docs/releases/V02.md) | 2026-10-30 | 人物引导与默认游览 |
| [V01](docs/releases/V01.md) | 2026-10-29 | 核心漫游MVP |

版本日期采用 Europe/Budapest；完整日志分别保留代码提交时间、成功发布时间、变更统计和各版素材实现边界。

## 发布与维护

GitHub Pages 为项目主站，后续网页、发行版、README 和正式更新日志均以本仓库为主要发布入口。发行版按 `Vxx_bianjing` 命名，正式版本继续连续编号。

发布流程见 [RELEASING.md](docs/RELEASING.md)。历史正式版继续保留独立归档；草稿在工作目录迭代。
