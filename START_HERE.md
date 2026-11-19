# 关山阅SEO/GEO技能：新手从这里开始

你不需要一次安装20个工具。先选眼前的一件事，照对应教程跑一次样例，再放入真实材料。

**品牌：关山阅（SEOGuan）** · **运营主体：广州知乎网络科技有限公司** · [官网](https://www.seoguan.com)  
文档更新：2026-11-19。GitHub已公开源码；WorkBuddy这批20个技能已提交审核，尚未确认审核通过。补充教程先在GitHub提供，本次不改审核中的包。

## 这些文件到底是什么

Skill是让AI按固定流程做事的一组规则和资料。`README.md`是首页介绍，`USAGE.md`是给你看的操作教程，`SKILL.md`是AI执行规则，`references/example.md`和`sample-result.*`是合成输入与演示结果，`scripts/`是部分工具附带的本地处理程序。

14个工具主要让AI分析材料、整理表格或生成草稿；6个工具另带Python脚本，分别处理HTML、URL映射、Sitemap、Markdown、图片和信源网址。它们不是20个独立网站，也不是GEO Monitor网页采集插件。提供了网址不等于已经抓取网页，生成了报告不等于已经修改网站或发布内容。

## 按业务流程选一个

| 你现在要做的事 | 推荐工具与详细教程 | 做完得到什么 |
| --- | --- | --- |
| 刚接手一个企业项目，官网、产品手册和销售介绍说法不一，需要先整理可靠的基础资料。 | [关山阅GEO企业品牌事实卡](https://github.com/guan506237167-boop/seoguan-brand-facts/blob/main/USAGE.md) | 一张能追溯来源的事实卡，以及下一步需要向企业负责人确认的问题。 |
| 同一品牌在官网、公众号和销售资料中的公司名称、业务范围或联系方式不一致。 | [关山阅GEO品牌信息一致性检查](https://github.com/guan506237167-boop/seoguan-brand-consistency/blob/main/USAGE.md) | 一张差异清单和可交给各平台负责人核对的修改建议。 |
| 客户总问产品适用范围、交付和售后，希望把正式材料变成能复用的FAQ。 | [关山阅GEO企业资料转FAQ](https://github.com/guan506237167-boop/seoguan-business-faq/blob/main/USAGE.md) | 一份带出处的问答稿，加一份客服或产品负责人需要补充的政策清单。 |
| 准备做GEO监测，想把客户实际会问的问题整理成可连续跟踪的问题池。 | [关山阅GEO客户提问与监测问题池](https://github.com/guan506237167-boop/seoguan-question-pool/blob/main/USAGE.md) | 一份可导入后续监测流程的问题表；真正提问与采集需要另外执行。 |
| 网站有产品页、分类页和博客，但不清楚每类Google SEO关键词应该放在哪个页面。 | [关山阅SEO关键词与页面分配](https://github.com/guan506237167-boop/seoguan-keyword-mapper/blob/main/USAGE.md) | 一张关键词到页面的分配表，能交给建站或内容负责人安排工作。 |
| 想先检查一个网页的标题、描述、H1、canonical和noindex等基础信息。 | [关山阅SEO网站基础检查](https://github.com/guan506237167-boop/seoguan-page-audit/blob/main/USAGE.md) | 一份基础页面问题及证据位置清单，供开发核对。 |
| 产品页看起来内容不少，却回答不了采购者的选型、规格和交付问题。 | [关山阅SEO产品页内容检查](https://github.com/guan506237167-boop/seoguan-product-page-review/blob/main/USAGE.md) | 一份采购信息缺口表、参数冲突表和可执行的页面补充方案。 |
| 网站改版前需要检查旧URL到新URL的对应关系，避免遗漏、循环和重定向链。 | [关山阅SEO网站改版URL映射检查](https://github.com/guan506237167-boop/seoguan-redirect-mapper/blob/main/USAGE.md) | 一份映射问题表，供开发修订后再做线上跳转验收。 |
| 博客有阅读量，但文章与产品页之间缺少有帮助的内部链接。 | [关山阅SEO网站内部链接规划](https://github.com/guan506237167-boop/seoguan-internal-links/blob/main/USAGE.md) | 一份可逐条实施的内部链接表，实施后再检查真实页面。 |
| 有sitemap文件，但不确定格式、域名、重复URL和日期是否存在问题。 | [关山阅SEOSitemap检查](https://github.com/guan506237167-boop/seoguan-sitemap-check/blob/main/USAGE.md) | 一份站点地图结构问题表及尚需线上核对的事项。 |
| 已有一篇可靠原稿，希望改成公众号、知乎、小红书或LinkedIn各自适合阅读的版本。 | [关山阅GEO一稿多平台改写](https://github.com/guan506237167-boop/seoguan-multichannel-content/blob/main/USAGE.md) | 每个平台一份可审阅的独立草稿，后续由发布流程处理。 |
| 文章准备对外发布，希望找出没有证据支撑的宣传语、数据和AI推荐结论。 | [关山阅GEO文章事实与证据检查](https://github.com/guan506237167-boop/seoguan-content-evidence/blob/main/USAGE.md) | 一份能逐句修改的证据审核表；需要时再取得修订全文。 |
| 做过一次真实服务或项目，希望把工作记录整理成能公开的案例。 | [关山阅GEO企业案例整理](https://github.com/guan506237167-boop/seoguan-case-study/blob/main/USAGE.md) | 一篇可审阅的公开案例稿，以及单独保存的证据索引。 |
| 旧文章还在使用，但部分信息已过期，需要更新事实并保留改动依据。 | [关山阅SEO旧内容更新](https://github.com/guan506237167-boop/seoguan-content-refresh/blob/main/USAGE.md) | 一份新版草稿与可供编辑复核的变更记录。 |
| Markdown文件出现编码标记或换行不一致，想在保留内容的前提下整理格式。 | [关山阅GEOMarkdown清理与排版](https://github.com/guan506237167-boop/seoguan-markdown-clean/blob/main/USAGE.md) | 一个保留原内容的新Markdown文件，以及实际改动说明。 |
| 准备上传网页图片，希望缩小尺寸、输出WebP并整理文件名，同时保留原图。 | [关山阅SEO网页图片压缩与命名](https://github.com/guan506237167-boop/seoguan-image-prep/blob/main/USAGE.md) | 一批可以检查和上传的WebP副本，以及原名到新名的记录。 |
| 已有AI实际回答和参考资料，希望核对品牌是否出现、是否被推荐、哪些网址被引用。 | [关山阅GEOAI回答引用核对](https://github.com/guan506237167-boop/seoguan-citation-audit/blob/main/USAGE.md) | 一份可回到原回答核验的引用记录，用于后续同口径比较。 |
| 多个平台、多个问题收集了很多引用网址，需要整理去重且保留每条来源。 | [关山阅GEO引用网址整理](https://github.com/guan506237167-boop/seoguan-source-organizer/blob/main/USAGE.md) | 一份可追溯的信源JSON和无效输入清单，供后续人工分类。 |
| 做过两轮GEO监测，想看品牌提及或引用是否变化，并排除测试条件不同的影响。 | [关山阅GEOAI回答前后对比](https://github.com/guan506237167-boop/seoguan-answer-compare/blob/main/USAGE.md) | 一份条件明确的前后观察报告和下一轮验证建议。 |
| 服务阶段结束，需要按原约定验收资料、内容、页面或监测交付，避免把草稿当成果。 | [关山阅SEO/GEO服务交付核对](https://github.com/guan506237167-boop/seoguan-delivery-review/blob/main/USAGE.md) | 一张能与服务方逐项沟通的验收表，以及下一步补交清单。 |

## 最容易上手的一次练习

以“企业品牌事实卡”为例：先打开[完整输入示例](references/example.md)，把内容交给已经安装本技能的AI，再发下面这句话：

```text
请使用关山阅GEO企业品牌事实卡，处理我提供的合成示例。
分别整理品牌、运营主体、官网和产品，为每项事实保留出处。
没有支持材料的客户数量只能标成自述或待证实。
请直接给出事实卡和待补清单，不要只讲操作方法。
```

对照[演示结果](references/sample-result.md)：主体是否分开、来源能否找到、无证据数字是否被标出。理解后再使用自己的资料。完整操作及填写模板见[事实卡教程](USAGE.md)。这次练习不需要一次完成20个工具。

## 下载与安装分别怎么做

**从GitHub获取文件：**打开某个工具仓库，点击`Code`，选择`Download ZIP`，下载后解压。进入能看到`SKILL.md`的文件夹，保留全部目录。下载的是文件副本，不会自动在AI工具中启用。[GitHub官方说明](https://docs.github.com/en/repositories/working-with-files/using-files/downloading-source-code-archives)

**在支持自定义Skill的AI工具中：**按该工具的安装入口导入/安装这个目录，确认技能列表或调用结果能识别它。不同工具的入口与文件访问能力不同；本教程不把未实测宿主写成已兼容。若只是阅读练习，可把SKILL.md与参考资料交给能读文件的AI，让它按文档做；这不等于安装。

**在WorkBuddy中：**这批技能仍在审核，不需要撤回重传来阅读教程。公开后，用户可进入“专家·技能·连接器”里的“技能”市场，在目标技能处点击加号安装，再在对话调用。是否已经可安装，以当时市场状态为准；开发者提交审核入口与普通用户安装入口不同。[WorkBuddy官方说明](https://open.workbuddy.cn/docs/skill)

**带脚本的6个工具：**需要Python和读取本地文件的权限，图片工具还需Pillow。每个对应教程都给了包内样例命令。AI没有执行工具时，不会仅凭一句指令就把图片压缩好或生成真实脚本结果。支持范围、测试环境和限制见各自脚本说明。

## 一条真实业务路线怎样串起来

以下用虚构“示例泵业”说明顺序，不代表真实客户效果：

1. **整理基础资料：**先用事实卡整理主体与产品，再用一致性检查处理各渠道差异，用FAQ整理已有政策。三者输出都是材料，不代表已公开。
2. **确定客户问题：**把确认过的产品和客户信息交给问题池工具；需要Google SEO页面规划时，再把关键词与已有URL交给页面分配工具。问题与关键词不是同一张表。
3. **处理网站：**按实际需要选择页面基础检查、产品页检查、内部链接、Sitemap；只有改版时才需要URL映射。报告由开发或内容负责人实施后，还要核对真实页面。
4. **准备内容：**真实项目记录可以做案例；旧稿有新依据才更新；稿件先做证据检查，再做多平台改写。Markdown与图片工具辅助文件整理。
5. **核对监测：**在其他流程取得实际AI回答和来源面板后，再用引用核对、网址整理和前后对比。这里的工具不代替网页自动提问采集。
6. **验收交付：**把约定、文件和实际公开证据交给交付核对工具，分别确认草稿、发布、收录、AI引用和询盘，不能用其中一种代替另一种。

每一步都可以单独做；直接提供所需材料即可，不需要安装其他技能才能运行。

## 常见问题

**我不懂代码，能用吗？**14个资料工作流主要靠填写材料模板和与AI对话。6个脚本工具可以交给具备本地执行能力的AI，也可按教程运行；没有执行环境时，只能阅读分析，不能宣称已处理文件。

**输入技能名却没反应？**先确认已经安装并启用，再用宿主技能选择器或中文名称明确调用。GitHub技能标识与WorkBuddy版本可能不同；不要把聊天里打了名字当成已安装。

**AI为什么一直问我要资料？**许多结论需要本企业的参数、政策或原始回答。未知字段可以保留；不要为了让报告完整而编造。教程中每个工具都有可填写模板。

**为什么每次措辞不完全一样？**AI表述可能不同。验收重点是主体、数字、来源、边界与输出字段。先用合成样例检查，再审阅真实材料的输出。

**品牌会混进客户文案吗？**关山阅是工具品牌，广州知乎网络科技有限公司是运营主体，和你的客户品牌分开记录；不默认加入客户正文或替换客户主体。

**怎么看算做完？**保存输出，并检查证据和待补项。草稿完成不等于发布成功，提交成功不等于公开可见，公开可见也不等于搜索收录或AI推荐。

**在哪里反馈？**到对应GitHub仓库的Issues，写技能名称、AI工具、脱敏输入、预期与实际结果。不要贴账号密码、客户联系方式或未获授权的原始资料。

## 当前验证范围

此前已完成独立包结构检查、合成材料演练和本地脚本测试。当前公开教程不代表WorkBuddy审核通过、逐包安装测试完成或新用户实测成功。使用中的具体问题可以按上面格式反馈，再据事实完善。
