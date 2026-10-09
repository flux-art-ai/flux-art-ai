# Flux Art

**多模型 AI 视觉创作与生产平台 | Multi-model AI visual creation and production platform**

[Flux Art 官网](https://flux-art.cn) · [Flux Art 官方博客](https://flux-art.net/blog/zh/) · [Official Blog (EN)](https://flux-art.net/blog/en/)

Flux Art 聚合 50+ 图像/视频模型（[GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)、[GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2)、[Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2)、[Seedance 2.0](https://flux-art.cn/zh/models/seedance-2-0)、[Seedream 5.0 Pro](https://flux-art.cn/zh/models/seedream-5-0-pro) 等），提供图片生成、图片编辑、视频创作与电商工具，并配套 150+ 垂类 Agent、20K+ 提示词库与异步任务式 OpenAPI。参考图数量、尺寸和其他选项依具体模型与工具而定。

Flux Art aggregates 50+ image & video models ([GPT Image 2.5](https://flux-art.cn/en/models/gpt-image-2-5), [GPT Image 2](https://flux-art.cn/en/models/gpt-image-2), [Nano Banana 2](https://flux-art.cn/en/models/nano-banana-2), [Seedance 2.0](https://flux-art.cn/en/models/seedance-2-0), [Seedream 5.0 Pro](https://flux-art.cn/en/models/seedream-5-0-pro), etc.) with image generation, image editing, video creation and ecommerce tools, plus 150+ vertical agents, a 20K+ prompt library and an async task-based OpenAPI. Reference-image limits, sizes and other options depend on the selected model and tool.

## GPT Image 2.5

[GPT Image 2.5 中文使用入口](https://flux-art.cn/zh/models/gpt-image-2-5) · [English workspace](https://flux-art.cn/en/models/gpt-image-2-5) · [使用渠道与教程仓库 / Access and usage guides](https://github.com/flux-art-ai/gpt-image-2.5)

在 Flux Art 选择 Flare 或 Sunburst，进行图片生成与参考图编辑；教程包含首次使用、版本选择、文字排版、电商衔接和故障排查。模型由 OpenAI 提供，仓库由 Flux Art 维护。

- 第一次使用：[GPT Image 2.5 使用渠道与开始步骤](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/getting-started.md)。
- 选择版本：[Flare 与 Sunburst 使用选择](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/flare-vs-sunburst.md)。
- 按任务操作：[参考图编辑](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/reference-editing.md) · [文字与版式](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/text-and-layout.md) · [电商工作流](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/ecommerce-workflow.md)。
- 程序接入：网页统一使用 GPT Image 2.5 家族入口；Flux Art OpenAPI 当前 Reference 列出 `gpt-image-2.5-flare` 与 `gpt-image-2.5-sunburst`。接入前仍应通过当前账户的 `GET /models` 核对目录，并按异步任务状态读取结果。详见[费用与 API 渠道说明](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/pricing-and-api.md)和 [API Reference](https://flux-art.net/zh/openapi/reference)。
- 返修完成后：[人工修复件验收与继续编辑](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/repair-acceptance-and-batch-restart.md) → [SKU 批次恢复检查](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/04-series-consistency.md) → [SKU 批量图](https://flux-art.cn/zh/ai-ecommerce/sku-batch)。先确认修复件，再修正批次输入；每个变体独立复核。Accept the repaired file, correct the batch inputs, then review every variant before delivery.

For browser use, open the GPT Image 2.5 family workspace and choose Flare or Sunburst in the interface. For Flux Art OpenAPI integrations, the current Reference lists `gpt-image-2.5-flare` and `gpt-image-2.5-sunburst`; confirm availability and accepted fields with the authenticated `GET /models` response before creating a task. A queued response is not a completed image.

### GPT Image 2 还是 GPT Image 2.5？ / GPT Image 2 or GPT Image 2.5?

两个版本在 Flux Art 上有独立模型入口。先问“要新做一张图，还是修改一张已经通过的图”，再决定是否比较版本；不要把 2.5 当作所有 GPT Image 2 项目的强制替代。

| 读者问题 / Reader question | 使用路径 / Route | 验收重点 / Review focus |
|---|---|---|
| 需要产品图或写实商业摄影新构图 / Need a new product or photoreal commercial composition | 从 [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2)开始，或以同一商品资料比较 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5) Flare | 商品结构、材质、标签、构图与留白 |
| 已有通过图片，只改一个区域 / Have an accepted image and one bounded change | 在 GPT Image 2.5 中用同一原图比较 Flare / Sunburst / Compare Flare and Sunburst from the same accepted source | 指定修改是否完成，未修改区域是否保持 |
| 旧 GPT Image 2 项目已经稳定 / Existing GPT Image 2 workflow is stable | 继续使用原模型、提示词和检查表；需要测试 2.5 时另开可比小样 / Keep the accepted baseline and run a separate matched test | 不用新版名称覆盖旧记录，不混用 API ID |

中文实操见 [GPT Image 2 电商工作流](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/models/gpt-image-2.md)；GPT Image 2.5 的渠道与版本说明见 [专题仓库](https://github.com/flux-art-ai/gpt-image-2.5)。This is task routing, not a benchmark ranking.

### Seedream 5.0 Pro 网页入口与 API ID / Web entry and API ID

需要 AI 信息图、信息密集型视觉或明确区域的精准改图时，可从 [Seedream 5.0 Pro 中文入口](https://flux-art.cn/zh/models/seedream-5-0-pro)或 [English entry](https://flux-art.cn/en/models/seedream-5-0-pro)开始。网页短名用于浏览，不等于接口参数：当前 [Flux Art API Reference](https://flux-art.net/zh/openapi/reference)列出的模型 ID 是 `doubao-seedream-5-0-pro-260628`，不是网页路径中的 `seedream-5-0-pro`。

For API automation, verify `doubao-seedream-5-0-pro-260628` and its accepted fields with the authenticated `GET /models` response before creating an asynchronous task. Keep the selected model ID, task ID and final review result together; see the [Seedream 5.0 Pro ecommerce workflow](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/models/seedream-5-0-pro.md) for a production checklist.

### Seedance 2.0 网页入口与 API ID / Web entry and API ID

制作产品视频或广告短片时，从 [Seedance 2.0 中文入口](https://flux-art.cn/zh/models/seedance-2-0)或 [English entry](https://flux-art.cn/en/models/seedance-2-0)进入浏览器工作台。网页路径使用 `seedance-2-0`，当前 [Flux Art API Reference](https://flux-art.net/zh/openapi/reference)列出的 OpenAPI 模型 ID 则是 `doubao-seedance-2-0-260128`；两者不能互换。

For API automation, confirm `doubao-seedance-2-0-260128` and its accepted fields with the authenticated `GET /models` response before creating a video task. A created or queued task is not a finished clip: save the idempotency key, task ID, final status and delivery review. The [Seedance 2.0 ecommerce video workflow](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/models/seedance-2-0.md) covers the shot brief and product checks.

### Qwen Image 2.0 网页入口与 API ID / Web entry and API ID

需要快速比较图片草图、产品场景、社媒封面或参考图轻编辑方向时，可从 [Qwen Image 2.0 中文入口](https://flux-art.cn/zh/models/qwen-image-2-0)或 [English entry](https://flux-art.cn/en/models/qwen-image-2-0)开始。网页路径是 `qwen-image-2-0`，当前 [Flux Art API Reference](https://flux-art.net/zh/openapi/reference)列出的模型 ID 是 `qwen-image-2.0`；不要把网页短名直接复制到 API 请求。

For API use, verify `qwen-image-2.0` and its accepted fields with the authenticated `GET /models` response before creating an asynchronous image task. Keep the model ID, request purpose, task ID, final status and review result together. Qwen Image 2.0 is provided by the Alibaba Qwen-Image series; Flux Art provides the multi-model workspace and API access.

### OpenAPI 链接返回 401、404 或 405 怎么判断？ / Interpreting 401, 404 or 405

先确认打开的是[中文 OpenAPI 说明](https://flux-art.net/zh/openapi)或[英文 API Reference](https://flux-art.net/en/openapi/reference)，而不是把机器接口当作网页。接口基址本身可能返回 `404`；未带 Bearer API Key 的 `GET /models` 会返回 `401`；用浏览器默认的 `GET` 打开只接受 `POST` 的生成端点可能返回 `405`。查询任务时还必须把 `{task_id}` 换成创建响应中的真实 ID。按这四项修正后仍失败，再保存状态码和去敏后的响应体排查。

Open the [English OpenAPI guide](https://flux-art.net/en/openapi) or [API Reference](https://flux-art.net/en/openapi/reference) for documentation. The API base is not a human-readable page: it may return `404`; `GET /models` without a Bearer key returns `401`; opening a `POST`-only generation endpoint with a browser `GET` may return `405`; and `{task_id}` must be replaced with the ID from a creation response. Correct those four inputs before treating the response as a service incident.

## Nano Banana 四个版本怎么选？ / Which Nano Banana version should I use?

Nano Banana 是模型家族名称，不代表四个版本拥有相同分辨率、参考图范围或任务定位。先按当前任务选择入口，再在提交前核对页面选项。Google 提供这些模型，Flux Art 提供多模型工作台与使用入口。

| 当前任务 / Current task | 使用入口 / Flux Art entry | 交付前检查 / Before delivery |
|---|---|---|
| 单张已有图片的快速修改 / Fast edit of one existing image | [Nano Banana](https://flux-art.cn/zh/models/nano-banana) · [EN](https://flux-art.cn/en/models/nano-banana) | 当前为 1K，编辑最多三张参考图；仍要逐项检查未要求修改的区域 |
| 先试构图、氛围或版式方向 / Early direction drafts | [Nano Banana 2 Lite](https://flux-art.cn/zh/models/nano-banana-2-lite) · [EN](https://flux-art.cn/en/models/nano-banana-2-lite) | 当前为 1K 草图；方向通过后再进入定稿与商品事实验收 |
| 基于已验收图片扩展系列版本 / Controlled series variations | [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2) · [EN](https://flux-art.cn/en/models/nano-banana-2) | 当前提供 512、1K、2K、4K；尺寸变大不等于商品标签、结构或材质自动正确 |
| 需要较高分辨率的精细生成或编辑 / Detail-heavy generation or editing | [Nano Banana Pro](https://flux-art.cn/zh/models/nano-banana-pro) · [EN](https://flux-art.cn/en/models/nano-banana-pro) | 当前提供 1K、2K、4K；逐字核对文字、事实、Logo 与受保护区域 |

同一真实商品做版本比较时，固定原图、任务、画幅和验收表，只改变一个模型选择。需要把通过样本扩展成系列资产时，继续使用 [Nano Banana 2 多图融合与系列款流程](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/models/nano-banana-2.md)。 / Keep the source, task, framing and review checklist fixed when comparing versions; change only the selected model.

## AI 电商 / AI Ecommerce

### 电商做图先选哪个入口？ / Where should I start?

| 你要完成的任务 / Task | 在 Flux Art 上怎么做 / Start here | 操作资料 / Guide |
|---|---|---|
| 新商品图与带字视觉 / Product images and text | [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2)，根据真实商品资料生成或编辑 | [商品图制作与验收](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/models/gpt-image-2.md) |
| 同一商品换场景 / Product scene variations | [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2)，明确每张参考图的用途 | [多图融合与系列款](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/models/nano-banana-2.md) |
| 继续修改已有图片 / Revise an existing image | [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)，在编辑模式比较 Flare / Sunburst | [修改边界与返修检查](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/reference-editing.md) |
| 一套上架图或多个 SKU / Listing sets or SKU variants | [AI 电商专区](https://flux-art.cn/zh/ai-ecommerce)，按交付物选专用工具 | [工具区别与输入准备](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/10-ecommerce-tools.md) |

已验收的流程不必只因新版上线而更换；先用同一份商品资料比较结果。模型页面负责创作，GitHub 页面提供操作资料，商品结构和包装文字仍需逐张核对。

模特图任务要按现有素材分流，不能把“上身、换姿势、换脸”合成一个模糊需求：

| 现有素材 / Starting material | 专用入口 / Dedicated entry | 通过条件 / Pass condition |
|---|---|---|
| 服装商品图，需要生成上身展示 / Garment image needs an on-model view | [模特穿戴](https://flux-art.cn/zh/ai-ecommerce/model-wearing) · [Model Wearing](https://flux-art.cn/en/ai-ecommerce/model-wearing) | 版型、颜色、材质、领口、袖口、下摆、图案和遮挡可对照实物 |
| 已有模特图，只改变姿势 / Existing model image, pose only | [模特一键换姿势](https://flux-art.cn/zh/ai-ecommerce/model-pose-change) · [Model Pose Change](https://flux-art.cn/en/ai-ecommerce/model-pose-change) | 人物、服装和场景保持，人体结构与布料形变自然 |
| 已有模特图和已授权面部参考 / Model image plus an authorized face reference | [AI 模特换脸](https://flux-art.cn/zh/ai-ecommerce/model-face-swap) · [Model Face Swap](https://flux-art.cn/en/ai-ecommerce/model-face-swap) | 授权有效，面部边界与光线自然，发型、姿势、造型和场景不被改写 |

需要串联多步时，每一步都从上一张已通过的图片继续，并保存输入、用途、授权范围和退回原因。换脸图不得暗示真人代言；穿戴图不能证明真实尺码或合身程度。英文操作与停止条件见 [Flux Art model-image workflow](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/en/09-model-photo.md)。

[中文电商专区](https://flux-art.cn/zh/ai-ecommerce) · [English ecommerce workspace](https://flux-art.cn/en/ai-ecommerce)

- 上架内容 / Listing assets：[商品套图](https://flux-art.cn/zh/ai-ecommerce/product-suite)、[A+ 详情页](https://flux-art.cn/zh/ai-ecommerce/a-plus-content)、[SKU 批量图](https://flux-art.cn/zh/ai-ecommerce/sku-batch)。
- 商品图处理 / Product editing：[爆款图片复刻](https://flux-art.cn/zh/ai-ecommerce/reference-clone)、[产品精修](https://flux-art.cn/zh/ai-ecommerce/product-retouch)、[产品换色](https://flux-art.cn/zh/ai-ecommerce/product-recolor)、[一键换背景](https://flux-art.cn/zh/ai-ecommerce/product-background)。
- 服饰与穿戴 / Apparel and try-on：[服装组图](https://flux-art.cn/zh/ai-ecommerce/clothing-suite)、[模特穿戴](https://flux-art.cn/zh/ai-ecommerce/model-wearing)、[AI 万戴](https://flux-art.cn/zh/ai-ecommerce/accessory-try-on)、[模特一键换姿势](https://flux-art.cn/zh/ai-ecommerce/model-pose-change)、[AI 模特换脸](https://flux-art.cn/zh/ai-ecommerce/model-face-swap)、[AI 试鞋](https://flux-art.cn/zh/ai-ecommerce/shoe-try-on)。

如何准备素材和验收结果，见[电商工具选择指南](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/10-ecommerce-tools.md)。人物和参考素材需要授权，生成结果仍应逐项检查。Flux Art 提供平台与工作流，不是模型原厂或 Black Forest Labs 的 FLUX.1 单一模型。

### 商品资料怎样交给模型？ / Product evidence checklist

| 资料 | 推荐做法 | 对应入口与检查 |
|---|---|---|
| 包装文字、标题、数字和单位 | 从商品包装或已批准文案逐字抄录，标记不能改写的字段 | 用 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)生成或局部编辑，并按[文字与版式教程](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/text-and-layout.md)校对 |
| 颜色、容量、尺寸等 SKU 属性 | 一行只记录一个完整 SKU，不把颜色与规格拆开猜测 | 进入 [SKU 批量图](https://flux-art.cn/zh/ai-ecommerce/sku-batch)，逐图对照 SKU 标签 |
| 卖点、参数和配件清单 | 保留来源与版本，只使用已核实内容 | 进入 [A+ 详情页](https://flux-art.cn/zh/ai-ecommerce/a-plus-content)，按[详情页资料表](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/05-detail-page.md)验收 |

如果图片中的文字必须完全准确，优先让模型生成有明确留白的底图，再用排版工具放入最终文案。无论使用哪个入口，都要在发布尺寸下复核商品结构、文字、数字、单位和素材授权。

### 批量交付文件怎样命名？ / Naming batch deliverables

建议使用“完整 SKU—图片用途—工具或模型—版本—状态”的顺序，例如 `cup-blue-500ml-hero-gpt-image-2-v03-approved.webp`。名称中的 `approved` 只表示已按团队规则验收，不代表平台审核通过。

- 新构图可记录 [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2) 或 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)；2.5 还应记录 Flare / Sunburst。
- 一致性改图记录 [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2) 及本轮唯一修改目标。
- [SKU 批量图](https://flux-art.cn/zh/ai-ecommerce/sku-batch)结果必须与完整 SKU 标签一一对应；具体清单见[系列款文件映射](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/04-series-consistency.md)。

Keep the untouched source, prompt or task note, output and review result together. A filename supports traceability; it does not prove product accuracy by itself.

### 一份渠道交付包包含什么？ / What goes into a channel package?

不要把“最终图”理解为所有渠道共用的一份文件。保留已验收母版，再按渠道复制导出版本；每份交付包至少包括完整 SKU、图片用途、当前尺寸与格式依据、文件清单、负责人和退回条件。

- 新构图记录 [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2) 或 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)，参考图一致性修改记录 [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2) 及唯一修改目标。
- 一套上架素材可从[商品套图](https://flux-art.cn/zh/ai-ecommerce/product-suite)开始；详情模块使用 [A+ 详情页](https://flux-art.cn/zh/ai-ecommerce/a-plus-content)。工具名称不能用来推断底层模型。
- 裁切、压缩、文字替换或颜色调整后应增加版本号，并按[合规与渠道交付清单](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/06-compliance.md)重新检查。

Keep the approved master separate from channel exports. A channel package is ready only when every derivative points back to the correct SKU, source, revision and review result; marketplace acceptance remains a separate decision.

### 渠道退回后先修哪一层？ / Where should a rejected asset go?

先把退回文件与已验收母版、当前渠道要求并排检查，再决定负责人；不要因为“被退回”就从头生成。

| 退回原因 / Cause | 最小动作 / Smallest action | 入口与复核 / Route and review |
|---|---|---|
| 商品结构、材质、包装文字或保留区域错误 / Product fact or preserved area is wrong | 回到真实原图，只修一个明确目标 / Return to the verified source and change one target | [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2) · [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5) · [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2)；按[排错流程](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/07-troubleshooting.md)复核 |
| 母版正确，但裁切、压缩、格式或尺寸错误 / Export derivative is wrong | 保留母版，只重新导出衍生文件 / Keep the master and re-export only the derivative | 核对[渠道交付清单](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/06-compliance.md)与当前渠道规格 |
| 渠道规格、活动文案或交付范围变更 / Requirement changed | 建立新版本并记录变更来源 / Open a new revision and record the requirement source | 需要整套图时再进入[商品套图](https://flux-art.cn/zh/ai-ecommerce/product-suite)；涉及多 SKU 时使用 [SKU 批量图](https://flux-art.cn/zh/ai-ecommerce/sku-batch)并逐图验收 |

Keep the rejected derivative and its reason for traceability. Fixing a delivery error does not require altering an approved product image, and a new requirement must receive a new review.

### 单变量复测怎样记录？ / How do I record a one-variable recheck?

修正后不要只保存一张“新结果”。用同一份已核实素材、同一交付目标和可比设置复测，并明确记录唯一改变的指令、选区或版本。这样才能判断修正是否有效，也能发现商品结构、包装文字或其他正确区域是否被意外改变。

| Record | 中文记录 | English record |
|---|---|---|
| Baseline | 原图来源、上一版结果、具体错误 | Verified source, previous output, exact defect |
| One change | 本轮唯一修改项；其余输入与设置不变 | The only changed instruction, region, or version; keep other inputs comparable |
| Comparison | 目标区域是否修好，未修改区域是否出现新偏差 | Whether the target was fixed and untouched regions regressed |
| Verdict | 通过、不通过或回退，附复核人和日期 | Pass, fail, or roll back, with reviewer and date |

可从 [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2)、[GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)或 [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2)的实际使用入口记录模型；完整复测步骤见[电商商品图排错](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/07-troubleshooting.md)。

Keep the failed result as evidence rather than replacing the approved master. The same record can be used for an export correction, but marketplace acceptance must still be checked separately.

### 连续复测失败后怎样升级处理？ / What happens after repeated failed rechecks?

同一项已核实要求在连续、可比的复测中仍失败，或每次修正都会破坏另一处已验收区域时，应停止叠加提示词。先按证据选择回退、重建资料或转人工处理。

| 当前证据 / Evidence | 下一步 / Next action | 交接入口 / Handoff route |
|---|---|---|
| 最近通过版本仍保持正确商品事实 / The last accepted version remains accurate | 回退该母版，只重做一个变化 / Roll back and repeat one bounded change | [商品图排错 / Troubleshooting](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/07-troubleshooting.md) |
| 原图看不清标签、结构、材质或 SKU / The source cannot verify the label, structure, material or SKU | 补真实商品资料后重建任务 / Rebuild the task with verified product evidence | [商品资料清单 / Product evidence](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/05-detail-page.md) |
| 精确文字、品牌元素或关键商品细节无法可靠保留 / Exact text, brand elements or critical details remain unreliable | 转设计或合规复核，不用近似结果冒充已核实内容 / Hand off to design or compliance review | [合规清单 / Compliance](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/06-compliance.md) |
| 只有渠道裁切、压缩、格式或尺寸失败 / Only the channel export fails | 保留母版，重新制作衍生文件 / Keep the master and rebuild the derivative | [电商工具入口 / Ecommerce tools](https://flux-art.cn/zh/ai-ecommerce) |

交接时保留原图、最后通过版本、失败结果、唯一修改项和复核结论。Keep the untouched source, last accepted version, failed result, single requested change and review verdict together.

### 包装或 SKU 更新后，先查哪些旧图？ / Which old assets should be replaced after a SKU or packaging update?

先建立一张受影响清单，再开始生成或编辑。清单至少覆盖已验收母版、渠道导出、商品套图、A+ 模块和仍在使用的活动素材，并为每项记录完整 SKU、旧版本、新版本、负责人和替换状态。这样可以只处理仍引用旧资料的文件，而不把已经正确的资产重新生成。

- 新商品构图可从 [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2)开始；现有图片的有限修改可在 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)选择 Flare 或 Sunburst。
- 保持系列画面关系时可评估 [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2)，但商品事实仍来自新实拍、新包装稿和完整 SKU。
- 多 SKU 使用 [SKU 批量图](https://flux-art.cn/zh/ai-ecommerce/sku-batch)，同商品多模块使用[商品套图](https://flux-art.cn/zh/ai-ecommerce/product-suite)；每个新结果都要重新验收。

Keep a dependency list for approved masters, channel exports, listing sets, A+ modules and campaign derivatives. Replace only files that still depend on the retired product revision, and keep the previous version for traceability rather than presenting it as current inventory.

### 活动结束后的恢复路径 / Campaign expiry rollback path

活动版不能覆盖常规母版。上线前记录活动开始与结束时间、完整 SKU、常规母版、活动衍生文件和使用渠道；到期后按渠道恢复，并查看前台页面、缩略图和可能保留旧图的缓存预览。若常规图已经对应过期包装或旧商品版本，应先按上面的依赖清单更新商品事实，再恢复发布。

1. 核对活动是否在每个渠道实际结束，而不只依据单一日历时间。 / Confirm the campaign has ended on every channel, not only in one calendar.
2. 恢复已验收且无过期优惠的常规母版；没有可用母版时，先在 [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2)、[GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)或 [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2)完成制作与人工验收。 / Restore an approved evergreen master without expired offers; if none exists, create and review one first.
3. 逐项替换商品首图、[商品套图](https://flux-art.cn/zh/ai-ecommerce/product-suite)、A+ 模块、广告素材和多语言版本，并保留下线截图。 / Replace listing images, product sets, A+ modules, ads and localized derivatives, then retain screenshots as evidence.

This is an operator checklist. Flux Art model pages do not automatically schedule marketplace publication, purge channel caches or confirm marketplace approval.

### 无字母版怎样变成多语言版本？ / How do I create localized versions from a text-free master?

先验收没有营销文字的常规母版，再把中文、英文或其他市场版本作为独立交付物。每个版本都要绑定完整 SKU、目标地区、批准文案、术语表、不可翻译项、渠道用途和复核人；不要把一个语言版本直接覆盖到另一个版本上。

1. **锁定母版 / Lock the master**：确认商品、构图、颜色、包装和文字留白正确，保存母版版本号。 / Confirm the product, composition, color, packaging and text-safe area, then record the master revision.
2. **准备语言包 / Prepare the locale pack**：逐项列出批准文案、固定术语、品牌名、型号、数字与单位。 / List approved copy, fixed terms, brand names, model numbers, values and units.
3. **一次只做一种语言 / Produce one locale at a time**：短标题或限定区域改字可进入 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)；长文案使用排版工具。 / Use GPT Image 2.5 for short copy or bounded edits; place dense copy in a layout tool.
4. **分别验收 / Review separately**：由理解目标语言的人逐字复核，再检查移动端裁切、渠道规格和实际前台。 / Have a qualified reviewer proofread each locale, then inspect crop, channel requirements and the live placement.

制作路径要按文案与版式选择，而不是按语言数量选择：短标题或单个文字框可做限定区域编辑；规格表、长段正文、法定文字或必须精确对齐的内容应使用排版工具；仅渠道裁切变化时则保留已批准语言图，只重做衍生文件。 / Choose the production path by copy and layout: use a bounded edit for a short headline or one text box, a layout tool for tables, dense copy, required wording or exact typography, and a derivative-only export when only the channel crop changes.

完整表格见[图片翻译与多语言套图](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/08-image-translation.md)；英文团队可直接使用 [AI product image localization workflow](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/en/08-image-localization.md)。The workflow preserves traceability; it does not replace linguistic, legal or marketplace review.

### 批准文案改了，已上线的多语言图片怎么办？ / Approved copy changed: what is still live?

不要只替换制作目录里的成品。先按完整 SKU、地区语言、旧术语或旧文案版本，查商品页首图与缩略图、[商品套图](https://flux-art.cn/zh/ai-ecommerce/product-suite)、A+ 模块和广告位；记录每个位置当前引用的文件及负责人。Then list every live placement that still references the prior locale-pack revision.

把新文案交给目标语言审核人，保留原始商品图；限定区域的短文字修订可从 [GPT Image 2.5 使用入口](https://flux-art.cn/zh/models/gpt-image-2-5)开始，长文案则在排版工具中逐字放置。每个受影响渠道单独导出与验收，发布后检查前台和缩略图，并将旧版标为历史文件，而非删除证据。See the [replacement checklist](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/08-image-translation.md) for the change register and release checks.

### 用户说商品图与实物不符，如何处理？ / A customer reports that the image differs from the product

先保存反馈、当前页面截图、文件版本和完整 SKU，暂停继续使用被指出的文件；同时保留原图与最后通过版本，不用新生成结果覆盖证据。Capture the report, live placement, asset revision and complete SKU before changing the image.

1. 对照实物、批准包装稿、色卡或规格资料，标出结构、颜色、材质、文字或配件的具体差异。 / Compare the image with verified product evidence and mark the exact mismatch.
2. 只修一个有依据的目标：新构图可评估 [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2)，有限编辑可在 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)选择 Flare 或 Sunburst，一致性编辑可比较 [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2)。 / Change one verified target and keep the remaining areas stable.
3. 重新检查商品页、缩略图、[商品套图](https://flux-art.cn/zh/ai-ecommerce/product-suite)、A+ 模块和广告位；前台仍显示问题版本时不关闭反馈。 / Recheck every affected live placement before closing the report.

详细字段见[上线商品图反馈处置清单](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/06-compliance.md)。Do not put customer contact details, private order data or account credentials into a public repository record.

### 商品偏色与真实 SKU 换色怎样分流？ / Color cast or a real SKU color change?

先把同一实物、批准色卡、完整 SKU 和中性光线下的参考照片放在一起。If the same item only looks warmer or cooler because of capture conditions, establish a neutral reference before editing; if the requested color is a separate sellable SKU, obtain evidence for that SKU instead of sampling a color from another image.

- **拍摄色偏 / Capture color cast**：检查光源、白平衡和商品旁的灰卡或色卡；有可靠基线后，可进入[产品精修](https://flux-art.cn/zh/ai-ecommerce/product-retouch)处理已确认的色偏或光影问题。 / Check the light, white balance and an in-frame gray or color card before using Product Retouch.
- **显示偏差 / Display variance**：若同一已验收文件只在一台设备异常，先检查该设备的显示模式、亮度和色彩配置，不为单一屏幕改写母版。 / Do not regenerate an accepted master to compensate for one unverified display.
- **真实 SKU 换色 / Verified SKU recolor**：为目标颜色准备实物图、批准色卡和 SKU 映射，再进入[产品换色](https://flux-art.cn/zh/ai-ecommerce/product-recolor)。 / Use Product Recolor only for a verified, sellable color variant and review every output against that SKU.
- **证据冲突 / Conflicting evidence**：实物、色卡或包装资料无法对应时暂停；模型输出不能决定商品真实颜色。 / Pause when the evidence does not identify the actual product color.

完成后要重新检查材质高光、包装文字、Logo、阴影和未要求变化的区域。See the full [product-color troubleshooting path](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/07-troubleshooting.md).

### 商品比例异常怎样区分拍摄透视与结构错误？ / Perspective issue or structural mismatch?

先把同一完整 SKU 的正视图、侧视图、真实尺寸表和带尺度参照的照片并排查看。Do not treat every apparent size difference as a product-shape error: a close or oblique camera angle can make the near side look larger while the verified structure remains unchanged.

- **只在斜拍或近拍中变形 / Capture-only distortion**：优先重拍或调整机位；有真实基线后，可评估[产品精修](https://flux-art.cn/zh/ai-ecommerce/product-retouch)的透视修正。 / Reshoot first; use Product Retouch only for a confirmed perspective issue.
- **多个角度都与尺寸资料冲突 / Repeated structural mismatch**：回到真实资料或最后通过母版，不用拉伸图片代替结构校正。 / Return to verified evidence or the last accepted master.
- **尺寸或尺度证据缺失 / Missing scale evidence**：暂停编辑，补正视照片、尺寸来源和可靠参照；生成结果不能决定真实尺寸。 / Pause until the orthographic view, dimension source and scale reference are available.
- **有限编辑 / Bounded edit**：需要参考图修改时，可从 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)选择 Flare 或 Sunburst；每轮只改一个目标，并复核轮廓、接口、Logo、文字和未修改区域。 / Change one target per pass and review the whole image.

完整判断表见[商品图透视与比例排错](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/07-troubleshooting.md)。A passed image must match the verified dimension evidence; visual plausibility alone is not acceptance.

### 亮面商品的高光异常还是材质错误？ / Highlight issue or material mismatch?

玻璃、金属、漆面和透明包装会反射环境，亮斑变化不一定代表商品材质变了。Start with the same complete SKU, the uncropped source, verified material information and a controlled-light reference; compare surface texture, transparency, edges and reflection direction before editing.

- **局部光影问题 / Local lighting issue**：商品轮廓、纹理和透明度均正确，仅一处高光过硬、断裂或遮挡标签时，优先重拍；有真实基线后可评估[产品精修](https://flux-art.cn/zh/ai-ecommerce/product-retouch)的有限修正。 / Keep the edit bounded to the confirmed highlight or shadow.
- **整体材质错误 / Global material error**：金属像塑料、玻璃变浑浊，或不同角度的反射与表面纹理都不可信时，回到原始素材或最后通过母版；需要重建写实商品图可评估 [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2)。 / Do not stack local fixes on an unreliable material rendering.
- **环境反射 / Environmental reflection**：窗户、摄影棚或周围物体映在亮面上时，先调整光线、遮光板与机位，不要把真实反射误判为结构缺陷。 / Reshoot when the capture setup is the cause.
- **限定编辑 / Bounded reference edit**：证据齐全且只需处理一个反光区域时，可从 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)选择 Flare 或 Sunburst 做同条件比较；若纹理、颜色、文字或边缘发生变化，立即回退。 / Compare from the same accepted source instead of editing one failed result with another.

完整证据清单与停止线见[商品高光与材质排错](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/07-troubleshooting.md)。The final review must cover the whole image, not only the repaired highlight.

### 服装自然褶皱还是版型错误？ / Natural garment fold or construction error?

先用同一款号和颜色的正背面平铺图、缝线与图案近照建立基线，再比较人台和模特上身图。A pose may change folds and drape, but it should not move stable garment landmarks such as the shoulder seam, placket, pocket, button count, hem construction or pattern alignment.

- **自然形变 / Natural deformation**：变化集中在肘部、腰部或塞衣角等受力区，稳定地标仍能对应；记录姿势与穿法后，可保留该候选。 / Keep the candidate when the change follows the pose and the verified landmarks remain aligned.
- **版型或缝线错误 / Cut or seam mismatch**：不受力区域的肩线、衣长、裤腿或接缝也改变时，回到真实服装资料或最后通过版本，不在错误轮廓上继续修补。 / Return to verified garment evidence when the silhouette or seam placement changes outside the stressed area.
- **图案错误 / Pattern mismatch**：条纹、格纹或印花在接缝处断裂、复制、扭曲时，只在证据充分的区域做限定编辑，并重新检查整件服装。 / Use a bounded edit only when close-up evidence shows the correct pattern and seam relationship.
- **姿势引发异常 / Pose-induced failure**：原始上身图正确、换姿势后才出错时，从原图重新开始并降低动作幅度。 / Restart from the accepted wearing image and review every pose separately.

服装平铺、人台和营销组图可进入[服装组图](https://flux-art.cn/zh/ai-ecommerce/clothing-suite)，上身候选使用[模特穿戴](https://flux-art.cn/zh/ai-ecommerce/model-wearing)，已有模特图改动作使用[模特一键换姿势](https://flux-art.cn/zh/ai-ecommerce/model-pose-change)。需要限定参考图编辑时，可从 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)选择 Flare 或 Sunburst；它不能替代真实版型、尺码和穿着体验。完整验收见[AI 模特图工作流](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/09-model-photo.md)。

### AI 试鞋怎样从商品图走到上脚候选？ / How do I turn shoe photos into a try-on candidate?

先用同一完整 SKU 的多角度实拍确认鞋型和部件，再进入 [AI 试鞋](https://flux-art.cn/zh/ai-ecommerce/shoe-try-on)。Start with verified photos of the same complete SKU before opening [AI Shoe Try-on](https://flux-art.cn/en/ai-ecommerce/shoe-try-on); a try-on visual is a styling asset, not evidence of fit, comfort or sizing.

- **输入 / Inputs**：页面当前支持 1–4 张鞋履图，建议补正面、侧面、背面或鞋底；选择 AI 或已获授权的自定义模特。 / The current page accepts 1–4 shoe images and suggests front, side, rear or sole views; choose an AI model or an authorized custom model.
- **展示要求 / Presentation brief**：明确鞋履特写、姿势、场景、袜子和下装，不把多个 SKU 或左右脚方向混进同一任务。 / Define the close-up, pose, scene, socks and trousers without mixing SKUs or left/right orientation.
- **验收 / Review**：逐项核对鞋头、后跟、鞋底、鞋带孔或扣件、Logo、配色、遮挡、脚部与地面的接触和阴影。 / Review the toe box, heel, outsole, laces or fasteners, logo, colorway, occlusion, foot contact and shadow.
- **模型分流 / Model routing**：不含人物的鞋履商品图可评估 [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2)；单一区域的有界修改可评估 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)；已验收系列图的一致性扩展可评估 [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2)。 / Use each model for its stated image task, not as proof of physical fit.

当参考图无法证明鞋底、后跟或扣件结构，或者左右方向和 SKU 版本冲突时，暂停上脚图并补拍。完整操作与停止线见[鞋履上脚工作流](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/09-model-photo.md)。

### 配饰试戴怎样保持尺度和佩戴位置？ / How do I preserve accessory scale and placement?

先把配饰当作需要独立验收的真实商品，再进入 [AI 万戴](https://flux-art.cn/zh/ai-ecommerce/accessory-try-on)。Start with verified product evidence, then use [AI Accessory Try-on](https://flux-art.cn/en/ai-ecommerce/accessory-try-on) to create an on-model candidate; the result is a styling visual, not proof of physical fit or comfort.

- **选择任务 / Choose the task**：当前页面覆盖帽子、眼镜、围巾/披肩、项链、耳饰、手表、手链、腰带、手提包和单肩/斜挎包，可选择 AI 模特或已获授权的自定义模特。 / Choose the exact accessory type and an AI model or an authorized custom model.
- **准备证据 / Prepare evidence**：保留配饰正面、侧面、扣件、链带、五金、Logo、图案和尺寸依据；包袋还要记录手提、单肩或斜挎方式。 / Record product orientation, hardware, straps, logos, pattern landmarks and verified dimensions before generation.
- **检查锚点 / Review anchors**：眼镜检查鼻梁与镜腿，耳饰检查耳垂，项链检查颈部与吊坠，腕表检查表盘与腕部，包袋检查提手、肩带和身体遮挡。 / Review the actual contact path instead of judging only the overall look.
- **停止条件 / Stop condition**：结构、比例和多个佩戴点同时变化时回到商品证据或重新生成；只有整体已通过且单一区域有依据时，才评估 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5) 的限定编辑。 / Do not stack edits on a failed accessory candidate.

输出比例、人物属性和补充说明应服务于明确版位，不应被解释为真实尺寸或适配结论。完整分类表、可用提示词和整图验收见[配饰试戴工作流](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/09-model-photo.md)。

### 看不见的商品细节不能靠生成补齐 / Do not generate missing product evidence

如果参考图没有显示背面、接口、包装小字或装箱配件，先暂停会展示这些信息的任务。补拍应使用同一完整 SKU，并为每张照片记录正面、背面、侧面、底部、接口近照或包装文字等职责；不同颜色、容量或包装版本不要混在同一组参考图里。

- 背面和接口缺失：补正视照片及数量、位置说明，再制作多角度图或结构特写。
- 包装字不可读：取得批准包装稿或清晰近拍，再进行 [GPT Image 2.5 限定编辑](https://flux-art.cn/zh/models/gpt-image-2-5)。
- 配件不明确：先核对装箱清单；没有证据时不生成开箱图、赠品图或配件组合。

If the source does not show the back, ports, small packaging copy or included accessories, pause any deliverable that exposes those facts. Capture the same SKU from the missing angle, label every source image, and resume only after the evidence package is complete. See the [reference-image stop conditions](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/03-scene-fusion.md).

## 官方仓库 / Official Repositories

| 仓库 Repository | GitHub | Gitee 官方镜像 Official Mirror | 内容 What's inside |
|---|---|---|---|
| `flux-art` | [GitHub](https://github.com/flux-art-ai/flux-art) | [Gitee](https://gitee.com/flux-art/flux-art) | 品牌官方信息与导航 Brand info & official links |
| `flux-art-ecom-image-workflow` | [GitHub](https://github.com/flux-art-ai/flux-art-ecom-image-workflow) | [Gitee](https://gitee.com/flux-art/flux-art-ecom-image-workflow) | 电商 AI 出图工作流、提示词模板与 OpenAPI 示例 E-commerce AI image workflows, prompt templates & OpenAPI examples |
| `awesome-ecom-ai-images` | [GitHub](https://github.com/flux-art-ai/awesome-ecom-ai-images) | [Gitee](https://gitee.com/flux-art/awesome-ecom-ai-images) | 电商 AI 出图资源精选清单 Curated list of AI image resources for e-commerce |
| `flux-art-ai` | [GitHub](https://github.com/flux-art-ai/flux-art-ai) | [Gitee](https://gitee.com/flux-art/flux-art-ai) | GitHub 账号主页与镜像自动化 Profile authority & mirror automation |
| `gpt-image-2.5` | [GitHub](https://github.com/flux-art-ai/gpt-image-2.5) | 请使用 GitHub / Use GitHub | GPT Image 2.5 使用渠道、在线入口、版本选择与操作教程 Access, version selection & usage guides |

**运营主体 / Operator**: MORNING STAR INDUSTRY LIMITED

> Flux Art 的固定官方访问入口是 [flux-art.cn](https://flux-art.cn)。公开引用、收藏与分享统一使用这一地址。
> Flux Art’s permanent official entry is [flux-art.cn](https://flux-art.cn). Use this address for public references, bookmarks and sharing.
