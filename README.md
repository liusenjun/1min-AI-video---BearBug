# 1min AI Video — BearBug

> AI 生成短片 · 制作思路展示

---

## 项目概览

- **片名**：《小熊虫追着帽子去旅行》
- **主题**：治愈系1分钟AI动画短片
- **风格参考**：《宝可梦礼宾部》(Pokémon Concierge)
- **角色参考**：小熊虫表情包IP
- **制作周期**：2-3天

https://github.com/user-attachments/assets/705fbd93-c636-478a-ba05-79866f11eb3d

---

## 工具链

| 阶段 | 工具 |
|------|------|
| 剧本策划 | Gemini |
| 角色设计 | nano banana 2.0 |
| 提示词调试 | Gemini |
| 分镜图生成 | nano banana 2.0 |
| 视频生成 | flux2 in comfyUI & seedance2.0 in 小云雀|
| 剪辑配音 | capcut|

---

## 制作流程

### Phase 1 · 剧本策划

对标《宝可梦礼宾部》确定主题与叙事风格：
- 明确故事主题与情感基调
- 设计叙事节奏、具体分镜、转折点
- 确定每个镜头的时长、内容、运动方式

> 你给的方向已经很清晰了：
> 小熊虫IP + 《宝可梦礼宾部》那种定格动画质感与慢萌氛围 + 搞笑、可爱、无厘头、温馨
> 这类片子的关键不是“大剧情”，而是用一个极小的日常事件，连续堆叠几个意外笑点，最后落到一个很软的情绪点。
>
> 《小熊虫追着帽子去旅行》：小熊虫原本只是想在户外悠闲旅行，结果一阵风吹跑了它最心爱的帽子。它一路跌跌撞撞地追着帽子跑过草坡、溪边和花丛，最后在一处意想不到的美景前追上了帽子，也收获了这趟旅程里最开心的一刻。

---

### Phase 2 · 视觉风格提炼

从参考作品中提取核心视觉元素：
- 色彩体系
- 物品材质
- 光照风格
- 画面特色
<img width="320" height="160" alt="image" src="https://github.com/user-attachments/assets/3dae913c-51a8-4784-9345-1f044db2ac82" />
<img width="320" height="160" alt="image" src="https://github.com/user-attachments/assets/eb7e2016-d8d4-4d89-ba44-c57687367e3a" />
<img width="320" height="160" alt="image" src="https://github.com/user-attachments/assets/a51e7028-d23f-46d0-916a-54f9d89e8ffc" />
<img width="320" height="160" alt="image" src="https://github.com/user-attachments/assets/8e269326-d766-4f6a-ba1b-45a70567ddf7" />

→ 沉淀为**基础提示词库**，确保整体风格稳定一致

> 定格动画质感，宝可梦礼宾部式的温柔手工微缩场景氛围，手工搭建的 miniature diorama，纸板和轻木搭建的草坡场景结构，明显可见的手作痕迹，毛毡和布艺角色质感，分层纸草地，剪纸与折纸感植物，毛毡野花，小型手工石头，透明树脂质感的小溪，整体具有强烈可触摸纹理与纤维感，微距摄影，浅景深，移轴感，柔和明亮的午后暖阳，自然光穿过手工植物形成柔软电影感阴影，低饱和暖色调，童话感户外旅行氛围，镜头可爱、搞笑、无厘头、温馨、治愈，像真实拍摄的高质量定格动画电影画面。

---

### Phase 3 · 角色设计

以小熊虫表情包 IP 为原型：
- 构建 3D 羊毛毡风格角色
- 定妆照调试：材质、细节，光影
- 工具：nano banana 2.0

> 严格参考我上传的小熊虫多视角毛毡角色设定图作为唯一角色锚点，保持角色身份完全一致：身体比例一致，四肢短短，圆润可爱的轮廓，面部设计一致，毛毡与布艺材质一致，纤维与手工缝制感一致，鸭舌帽造型一致，小背包造型一致，颜色关系一致，角色不能跑型，不能改变脸型，不能改变肢体数量，不能改变材质语言。角色表演基调为：认真、慢半拍、笨拙、可爱、温柔。

<img width="1000" height="400" alt="image" src="https://github.com/user-attachments/assets/9d64eacf-f9aa-4c69-9dd8-8a01b14c76f5" />
<img width="440" height="440" alt="image" src="https://github.com/user-attachments/assets/841fc16b-e813-4a3c-808e-99665e9dba6f" />
<img width="440" height="440" alt="image" src="https://github.com/user-attachments/assets/6a00da61-5bfb-420b-ac4a-481017b79470" />


---

### Phase 4 · 场景设计

- 基于风格提示词 + 角色定妆照生成主要场景
- 多轮风格提示词迭代调试
- 逐步确定场景风格细节

> 按照之前生成的风格提示词加上角色定妆照，生成一两个主要场景的分镜。此过程需要不断调试风格提示词以保证生成场景的各种细节符合预期，经历了多轮风格提示词的调试。

<img width="200" height="110" alt="image" src="https://github.com/user-attachments/assets/65bce76d-256e-48d5-aa66-53babe046071" />
<img width="200" height="110" alt="image" src="https://github.com/user-attachments/assets/d45930f4-90e2-4eff-b69a-4c5ee68a5490" />
<img width="200" height="110" alt="image" src="https://github.com/user-attachments/assets/e072a105-9936-486e-87f1-82a0f6bcf3cc" />
<img width="200" height="110" alt="image" src="https://github.com/user-attachments/assets/f88a4e85-0c95-479a-8216-b5a0685a1059" />
<img width="2048" height="1143" alt="image" src="https://github.com/user-attachments/assets/22a064f6-df5b-488a-8aad-4e7ca0036b98" />

---

### Phase 5 · 分镜生成

- 依据剧本生成核心分镜图
- 逐镜确认风格一致性
- 为每个分镜图生成对应视频


> 确定风格后，开始生成每个分镜的核心分镜图，再依据分镜图生成每个镜头的视频。
<img width="1300" height="1214" alt="image" src="https://github.com/user-attachments/assets/c72bb1e4-1994-4953-810f-dac7c35916df" />

---

### Phase 6 · 剪辑 & 配音

- 依据分镜视频完成剪辑
- 简单配音制作

---

## 难点与解决

| 难点 | 解决思路 |
|------|---------|
| 风格一致性 | 提炼统一提示词库，逐步调试 |
| 角色稳定性 | 定妆照锚定角色形象 |
| 提示词迭代 | 多轮生成，记录有效关键词 |

---

*本项目仅供学习交流，不做任何商业用途。*
