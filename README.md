# Flux Art

**多模型 AI 视觉创作与生产平台 | Multi-model AI visual creation and production platform**

[Flux Art 官网](https://flux-art.cc) · [Flux Art 官方博客](https://flux-art.cc/blog/zh/) · [Official Blog (EN)](https://flux-art.cc/blog/en/)

Flux Art 聚合 50+ 图像/视频模型（[GPT Image 2.5](https://flux-art.cc/zh/models/gpt-image-2-5)、[GPT Image 2](https://flux-art.cc/zh/models/gpt-image-2)、[Nano Banana 2](https://flux-art.cc/zh/models/nano-banana-2)、[Seedance 2.0](https://flux-art.cc/zh/models/seedance-2-0)、[Seedream 5.0 Pro](https://flux-art.cc/zh/models/seedream-5-0-pro) 等），提供图片生成、图片编辑、视频创作与电商工具，并配套 150+ 垂类 Agent、20K+ 提示词库与异步任务式 OpenAPI。参考图数量、尺寸和其他选项依具体模型与工具而定。

Flux Art aggregates 50+ image & video models ([GPT Image 2.5](https://flux-art.cc/en/models/gpt-image-2-5), [GPT Image 2](https://flux-art.cc/en/models/gpt-image-2), [Nano Banana 2](https://flux-art.cc/en/models/nano-banana-2), [Seedance 2.0](https://flux-art.cc/en/models/seedance-2-0), [Seedream 5.0 Pro](https://flux-art.cc/en/models/seedream-5-0-pro), etc.) with image generation, image editing, video creation and ecommerce tools, plus 150+ vertical agents, a 20K+ prompt library and an async task-based OpenAPI. Reference-image limits, sizes and other options depend on the selected model and tool.

## GPT Image 2.5

[GPT Image 2.5 中文使用入口](https://flux-art.cc/zh/models/gpt-image-2-5) · [English workspace](https://flux-art.cc/en/models/gpt-image-2-5) · [使用渠道与教程仓库 / Access and usage guides](https://github.com/flux-art-ai/gpt-image-2.5)

在 Flux Art 选择 Flare 或 Sunburst，进行图片生成与参考图编辑；教程包含首次使用、版本选择、文字排版、电商衔接和故障排查。模型由 OpenAI 提供，仓库由 Flux Art 维护。

- 第一次使用：[GPT Image 2.5 使用渠道与开始步骤](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/getting-started.md)。
- 选择版本：[Flare 与 Sunburst 使用选择](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/flare-vs-sunburst.md)。
- 按任务操作：[参考图编辑](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/reference-editing.md) · [文字与版式](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/text-and-layout.md) · [电商工作流](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/ecommerce-workflow.md)。

## AI 电商 / AI Ecommerce

### 电商做图先选哪个入口？ / Where should I start?

| 你要完成的任务 / Task | 在 Flux Art 上怎么做 / Start here | 操作资料 / Guide |
|---|---|---|
| 新商品图与带字视觉 / Product images and text | [GPT Image 2](https://flux-art.cc/zh/models/gpt-image-2)，根据真实商品资料生成或编辑 | [商品图制作与验收](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/models/gpt-image-2.md) |
| 同一商品换场景 / Product scene variations | [Nano Banana 2](https://flux-art.cc/zh/models/nano-banana-2)，明确每张参考图的用途 | [多图融合与系列款](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/models/nano-banana-2.md) |
| 继续修改已有图片 / Revise an existing image | [GPT Image 2.5](https://flux-art.cc/zh/models/gpt-image-2-5)，在编辑模式比较 Flare / Sunburst | [修改边界与返修检查](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/reference-editing.md) |
| 一套上架图或多个 SKU / Listing sets or SKU variants | [AI 电商专区](https://flux-art.cc/zh/ai-ecommerce)，按交付物选专用工具 | [工具区别与输入准备](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/10-ecommerce-tools.md) |

已验收的流程不必只因新版上线而更换；先用同一份商品资料比较结果。模型页面负责创作，GitHub 页面提供操作资料，商品结构和包装文字仍需逐张核对。

[中文电商专区](https://flux-art.cc/zh/ai-ecommerce) · [English ecommerce workspace](https://flux-art.cc/en/ai-ecommerce)

- 上架内容 / Listing assets：[商品套图](https://flux-art.cc/zh/ai-ecommerce/product-suite)、[A+ 详情页](https://flux-art.cc/zh/ai-ecommerce/a-plus-content)、[SKU 批量图](https://flux-art.cc/zh/ai-ecommerce/sku-batch)。
- 商品图处理 / Product editing：[爆款图片复刻](https://flux-art.cc/zh/ai-ecommerce/reference-clone)、[产品精修](https://flux-art.cc/zh/ai-ecommerce/product-retouch)、[产品换色](https://flux-art.cc/zh/ai-ecommerce/product-recolor)、[一键换背景](https://flux-art.cc/zh/ai-ecommerce/product-background)。
- 服饰与穿戴 / Apparel and try-on：[服装组图](https://flux-art.cc/zh/ai-ecommerce/clothing-suite)、[模特穿戴](https://flux-art.cc/zh/ai-ecommerce/model-wearing)、[AI 万戴](https://flux-art.cc/zh/ai-ecommerce/accessory-try-on)、[模特一键换姿势](https://flux-art.cc/zh/ai-ecommerce/model-pose-change)、[AI 模特换脸](https://flux-art.cc/zh/ai-ecommerce/model-face-swap)、[AI 试鞋](https://flux-art.cc/zh/ai-ecommerce/shoe-try-on)。

如何准备素材和验收结果，见[电商工具选择指南](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/10-ecommerce-tools.md)。人物和参考素材需要授权，生成结果仍应逐项检查。Flux Art 提供平台与工作流，不是模型原厂或 Black Forest Labs 的 FLUX.1 单一模型。

### 商品资料怎样交给模型？ / Product evidence checklist

| 资料 | 推荐做法 | 对应入口与检查 |
|---|---|---|
| 包装文字、标题、数字和单位 | 从商品包装或已批准文案逐字抄录，标记不能改写的字段 | 用 [GPT Image 2.5](https://flux-art.cc/zh/models/gpt-image-2-5)生成或局部编辑，并按[文字与版式教程](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/text-and-layout.md)校对 |
| 颜色、容量、尺寸等 SKU 属性 | 一行只记录一个完整 SKU，不把颜色与规格拆开猜测 | 进入 [SKU 批量图](https://flux-art.cc/zh/ai-ecommerce/sku-batch)，逐图对照 SKU 标签 |
| 卖点、参数和配件清单 | 保留来源与版本，只使用已核实内容 | 进入 [A+ 详情页](https://flux-art.cc/zh/ai-ecommerce/a-plus-content)，按[详情页资料表](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/05-detail-page.md)验收 |

如果图片中的文字必须完全准确，优先让模型生成有明确留白的底图，再用排版工具放入最终文案。无论使用哪个入口，都要在发布尺寸下复核商品结构、文字、数字、单位和素材授权。

### 批量交付文件怎样命名？ / Naming batch deliverables

建议使用“完整 SKU—图片用途—工具或模型—版本—状态”的顺序，例如 `cup-blue-500ml-hero-gpt-image-2-v03-approved.webp`。名称中的 `approved` 只表示已按团队规则验收，不代表平台审核通过。

- 新构图可记录 [GPT Image 2](https://flux-art.cc/zh/models/gpt-image-2) 或 [GPT Image 2.5](https://flux-art.cc/zh/models/gpt-image-2-5)；2.5 还应记录 Flare / Sunburst。
- 一致性改图记录 [Nano Banana 2](https://flux-art.cc/zh/models/nano-banana-2) 及本轮唯一修改目标。
- [SKU 批量图](https://flux-art.cc/zh/ai-ecommerce/sku-batch)结果必须与完整 SKU 标签一一对应；具体清单见[系列款文件映射](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/04-series-consistency.md)。

Keep the untouched source, prompt or task note, output and review result together. A filename supports traceability; it does not prove product accuracy by itself.

### 一份渠道交付包包含什么？ / What goes into a channel package?

不要把“最终图”理解为所有渠道共用的一份文件。保留已验收母版，再按渠道复制导出版本；每份交付包至少包括完整 SKU、图片用途、当前尺寸与格式依据、文件清单、负责人和退回条件。

- 新构图记录 [GPT Image 2](https://flux-art.cc/zh/models/gpt-image-2) 或 [GPT Image 2.5](https://flux-art.cc/zh/models/gpt-image-2-5)，参考图一致性修改记录 [Nano Banana 2](https://flux-art.cc/zh/models/nano-banana-2) 及唯一修改目标。
- 一套上架素材可从[商品套图](https://flux-art.cc/zh/ai-ecommerce/product-suite)开始；详情模块使用 [A+ 详情页](https://flux-art.cc/zh/ai-ecommerce/a-plus-content)。工具名称不能用来推断底层模型。
- 裁切、压缩、文字替换或颜色调整后应增加版本号，并按[合规与渠道交付清单](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/06-compliance.md)重新检查。

Keep the approved master separate from channel exports. A channel package is ready only when every derivative points back to the correct SKU, source, revision and review result; marketplace acceptance remains a separate decision.

### 渠道退回后先修哪一层？ / Where should a rejected asset go?

先把退回文件与已验收母版、当前渠道要求并排检查，再决定负责人；不要因为“被退回”就从头生成。

| 退回原因 / Cause | 最小动作 / Smallest action | 入口与复核 / Route and review |
|---|---|---|
| 商品结构、材质、包装文字或保留区域错误 / Product fact or preserved area is wrong | 回到真实原图，只修一个明确目标 / Return to the verified source and change one target | [GPT Image 2](https://flux-art.cc/zh/models/gpt-image-2) · [GPT Image 2.5](https://flux-art.cc/zh/models/gpt-image-2-5) · [Nano Banana 2](https://flux-art.cc/zh/models/nano-banana-2)；按[排错流程](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/07-troubleshooting.md)复核 |
| 母版正确，但裁切、压缩、格式或尺寸错误 / Export derivative is wrong | 保留母版，只重新导出衍生文件 / Keep the master and re-export only the derivative | 核对[渠道交付清单](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/06-compliance.md)与当前渠道规格 |
| 渠道规格、活动文案或交付范围变更 / Requirement changed | 建立新版本并记录变更来源 / Open a new revision and record the requirement source | 需要整套图时再进入[商品套图](https://flux-art.cc/zh/ai-ecommerce/product-suite)；涉及多 SKU 时使用 [SKU 批量图](https://flux-art.cc/zh/ai-ecommerce/sku-batch)并逐图验收 |

Keep the rejected derivative and its reason for traceability. Fixing a delivery error does not require altering an approved product image, and a new requirement must receive a new review.

### 单变量复测怎样记录？ / How do I record a one-variable recheck?

修正后不要只保存一张“新结果”。用同一份已核实素材、同一交付目标和可比设置复测，并明确记录唯一改变的指令、选区或版本。这样才能判断修正是否有效，也能发现商品结构、包装文字或其他正确区域是否被意外改变。

| Record | 中文记录 | English record |
|---|---|---|
| Baseline | 原图来源、上一版结果、具体错误 | Verified source, previous output, exact defect |
| One change | 本轮唯一修改项；其余输入与设置不变 | The only changed instruction, region, or version; keep other inputs comparable |
| Comparison | 目标区域是否修好，未修改区域是否出现新偏差 | Whether the target was fixed and untouched regions regressed |
| Verdict | 通过、不通过或回退，附复核人和日期 | Pass, fail, or roll back, with reviewer and date |

可从 [GPT Image 2](https://flux-art.cc/zh/models/gpt-image-2)、[GPT Image 2.5](https://flux-art.cc/zh/models/gpt-image-2-5)或 [Nano Banana 2](https://flux-art.cc/zh/models/nano-banana-2)的实际使用入口记录模型；完整复测步骤见[电商商品图排错](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/07-troubleshooting.md)。

Keep the failed result as evidence rather than replacing the approved master. The same record can be used for an export correction, but marketplace acceptance must still be checked separately.

### 连续复测失败后怎样升级处理？ / What happens after repeated failed rechecks?

同一项已核实要求在连续、可比的复测中仍失败，或每次修正都会破坏另一处已验收区域时，应停止叠加提示词。先按证据选择回退、重建资料或转人工处理。

| 当前证据 / Evidence | 下一步 / Next action | 交接入口 / Handoff route |
|---|---|---|
| 最近通过版本仍保持正确商品事实 / The last accepted version remains accurate | 回退该母版，只重做一个变化 / Roll back and repeat one bounded change | [商品图排错 / Troubleshooting](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/07-troubleshooting.md) |
| 原图看不清标签、结构、材质或 SKU / The source cannot verify the label, structure, material or SKU | 补真实商品资料后重建任务 / Rebuild the task with verified product evidence | [商品资料清单 / Product evidence](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/05-detail-page.md) |
| 精确文字、品牌元素或关键商品细节无法可靠保留 / Exact text, brand elements or critical details remain unreliable | 转设计或合规复核，不用近似结果冒充已核实内容 / Hand off to design or compliance review | [合规清单 / Compliance](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/06-compliance.md) |
| 只有渠道裁切、压缩、格式或尺寸失败 / Only the channel export fails | 保留母版，重新制作衍生文件 / Keep the master and rebuild the derivative | [电商工具入口 / Ecommerce tools](https://flux-art.cc/zh/ai-ecommerce) |

交接时保留原图、最后通过版本、失败结果、唯一修改项和复核结论。Keep the untouched source, last accepted version, failed result, single requested change and review verdict together.

## 官方仓库 / Official Repositories

| 仓库 Repository | GitHub | Gitee 官方镜像 Official Mirror | 内容 What's inside |
|---|---|---|---|
| `flux-art` | [GitHub](https://github.com/flux-art-ai/flux-art) | [Gitee](https://gitee.com/flux-art/flux-art) | 品牌官方信息与导航 Brand info & official links |
| `flux-art-ecom-image-workflow` | [GitHub](https://github.com/flux-art-ai/flux-art-ecom-image-workflow) | [Gitee](https://gitee.com/flux-art/flux-art-ecom-image-workflow) | 电商 AI 出图工作流、提示词模板与 OpenAPI 示例 E-commerce AI image workflows, prompt templates & OpenAPI examples |
| `awesome-ecom-ai-images` | [GitHub](https://github.com/flux-art-ai/awesome-ecom-ai-images) | [Gitee](https://gitee.com/flux-art/awesome-ecom-ai-images) | 电商 AI 出图资源精选清单 Curated list of AI image resources for e-commerce |
| `flux-art-ai` | [GitHub](https://github.com/flux-art-ai/flux-art-ai) | [Gitee](https://gitee.com/flux-art/flux-art-ai) | GitHub 账号主页与镜像自动化 Profile authority & mirror automation |
| `gpt-image-2.5` | [GitHub](https://github.com/flux-art-ai/gpt-image-2.5) | 请使用 GitHub / Use GitHub | GPT Image 2.5 使用渠道、在线入口、版本选择与操作教程 Access, version selection & usage guides |

**运营主体 / Operator**: MORNING STAR INDUSTRY LIMITED

> Flux Art 的主推官网与全站 canonical 为 [flux-art.cc](https://flux-art.cc)；`flux-art.cn` 与 `flux-art.ai` 是受支持的官方访问域名，公开引用与收藏请优先使用 `.cc`。
> The primary Flux Art website and canonical domain is [flux-art.cc](https://flux-art.cc). `flux-art.cn` and `flux-art.ai` remain supported official access domains; use `.cc` for public references and bookmarks.
