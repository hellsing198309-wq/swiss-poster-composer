# Fine Art Poster Translator

> 将每张上传照片独立转译为一张 3:4 高级艺术海报：上半部保留真实摄影，下半部在暖白纸张留白中用艺术媒介重绘同一主体。

[打开独立视觉主页](./index.html) · [阅读完整 Skill](./SKILL.md) · [返回 Swiss Poster Composer](../index.html)

## 适合什么

这套 Skill 面向艺术展视觉、艺术书封面、博物馆商店艺术印刷品和独立艺术出版物。它的核心不是把照片套成某种滤镜，而是建立“真实对象 → 纸上转译”的对应关系：照片负责记录，艺术媒介负责提炼。

## 核心规则

| 规则 | 要求 |
| --- | --- |
| 独立输出 | 每张照片单独生成一张完整海报，不拼接、不合成、不共用主体 |
| 画幅 | 3:4 竖版 |
| 分区 | 上下约 1:1，各占画面 50% |
| 上半部 | 保留真实主体、环境、比例、姿态、材质与方向，只做轻微高级调色 |
| 下半部 | 用指定艺术媒介转译同一主体；未指定时默认克制水彩 / 墨彩 |
| 留白 | 下半部中央主体约占 45%–70%，周围保留大量暖白纸张留白 |
| 文字 | 只用少量英文标题、编号和年份，面积不超过下半部 5% |
| 禁止 | 卡通化、满版插画、随机背景、主体变形、廉价滤镜、乱码与多图拼接 |

## 快速使用

1. 将 `SKILL.md` 放入你的 Skill 目录。
2. 上传一张照片并调用 `$fine-art-poster-translator`。
3. 多张照片必须逐张调用，确保每张照片都有独立的主体分析和艺术转译。
4. 需要指定媒介时，在调用中写明“使用水彩 / 木刻 / 炭笔 / 拼贴”等；没有指定时默认采用参考图中的纸上水彩 / 墨彩语言。

最短调用方式：

```text
使用 $fine-art-poster-translator，将这张照片制作成 3:4 高级艺术海报：上半部保留真实摄影，下半部用克制水彩在暖白纸张留白中转译同一主体。
```

## 正式参考样本

下面 4 张是本 Skill 的正式视觉参考。它们分别展示了倒影风景、鸟类、湖畔人物和文化乐器题材；共同标准是上方真实摄影、下方中央媒介转译、四周留白和极少信息。

| 示例 | 上方主体 | 下方转译重点 |
| --- | --- | --- |
| [SUNSET REFLECTION](./assets/sunset-reflection-watercolor.png) | 潮滩、倒影、人物与小车 | 天空与倒影的水彩洗染、人物和车辆关系 |
| [HUMMINGBIRD](./assets/hummingbird-watercolor.png) | 蜂鸟与树枝 | 鸟的轮廓、羽毛色层、喙和枝条方向 |
| [LAKE COUPLE](./assets/lake-couple-watercolor.png) | 湖边台阶与情侣 | 两人的姿态、湖面、松枝和岸边结构 |
| [MUSICIAN](./assets/musician-watercolor.png) | 演奏者、弦乐器与圆形现场结构 | 人与乐器、鼓面 / 圆形构件、绳线和材质笔触 |

## 视觉判断标准

- 上半部必须仍然是照片，而不是“照片风格的画”。
- 下半部必须仍然是同一个主体，而不是泛化的水彩插画。
- 下半部主体要集中、安静、居中，留白明显多于绘画面积。
- 媒介要有纸张、颜料或线条的真实感，但不能脏乱、廉价或装饰化。
- 任何添加的枝条、倒影、圆形、线条或环境痕迹，都必须能从当前照片找到出处。

## 与 Swiss Poster Composer 的区别

`Fine Art Poster Translator` 侧重纸张留白和艺术媒介转译；`Swiss Poster Composer` 侧重严格网格、平面几何和国际主义版式。需要几何色块、Swiss Grid、标题栏、色板与年份系统时，请使用 `$swiss-poster-composer`。

## 包结构

```text
fine-art-poster-translator/
├── SKILL.md                 # 完整规则、流程与调用模板
├── README.md                # 使用说明与参考样本
├── index.html               # 独立 Skill 视觉主页
├── agents/
│   └── openai.yaml          # Skill 展示名称与默认调用提示
└── assets/
    ├── sunset-reflection-watercolor.png
    ├── hummingbird-watercolor.png
    ├── lake-couple-watercolor.png
    └── musician-watercolor.png
```

> 星野AI聚合网站：访问 [xyhub666.com](https://xyhub666.com/) 继续探索 AI 工具与服务入口。

