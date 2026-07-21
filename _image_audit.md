# AroundFire 报告站 · 全站配图审计（缺口清单）

审计日期：2026-07-21
审计范围：`summary.html` / `index.html` / `category.html` / `voc.html` / `ads.html` / `social.html` / `trends.html` / `seo.html` / `optimization.html`
（`competitors.html` / `meta.html` / `pricing.html` / `influencers.html` 由其他人并行处理，本次不碰）

判定标准：文字描述了某个页面元素、产品外观、界面现象、引用了某条评论/广告原文/视频，却没有配图或播放器。

审计前基线：

| 页面 | img | video | figure |
|---|---|---|---|
| summary.html | 0 | 0 | 0 |
| index.html | 0 | 0 | 0 |
| category.html | 39 | 0 | 1 |
| voc.html | 31 | 0 | 31 |
| ads.html | 37 | 40 | 0 |
| social.html | 21 | 0 | 21 |
| trends.html | 10 | 0 | 10 |
| seo.html | 4 | 0 | 4 |
| optimization.html | 63 | 0 | 47 |

素材池已全部复制进 `assets/`（295 个文件），审计前有 **18 个已下载但全站零引用**的素材。

---

## A. summary.html —— 全页零图（10 条核心结论）

| # | 缺口锚点 | 补什么 | 素材 | 状态 |
|---|---|---|---|---|
| A1 | §2 ① 「空位是真的」定位象限 | 品类定位坐标图 | `assets/products/positioning_chart.png` | ✅ 已有（原全站未用） |
| A2 | §2 ② 「Portable 打不过 NOMAD」 | NOMAD 广告素材实拍 + 关键词机会气泡图 | `assets/ads/nomadgrills/05_1338076138183777.jpg` + `assets/seo/01_keyword_opportunity_bubble.png` | ✅ 已有 |
| A3 | §2 ③ 「运费在结账第 4 区块才露出」 | 结账初始态（无运费）→ 填完地址后 $24.90 突现 | `assets/checkout/07_checkout_step1_initial.png` + `assets/checkout/08_checkout_us_shipping_2490.png` | ✅ 已有 |
| A4 | §2 ④ 关税悬崖 | 无对应截图素材（纯测算），表格已足够 | — | ⛔ 不补（无证据图，禁止编） |
| A5 | §2 ⑤ 「三种燃料旺季全部违法」 | 用户端禁火令证据 + 禁火州与热度州的地域重合 | `assets/evidence/reddit_firebans_wood_not_allowed.png` + `assets/trends/10_geo_subregion_lists.png` | ✅ 已有 |
| A6 | §2 ⑥ 「KBBQ 是证据最交叉的机会」 | KBBQ 词簇 + 5 年无季节性曲线 + $37 配件现状 | `assets/seo/03_kbbq_cluster.png` + `assets/trends/05_5y_kbbq.png` + `assets/products/AroundFire_KBBQ_Style_Grill_Grate.jpg` | ✅ 已有 |
| A7 | §2 ⑦ 「大众市场追问物理证据」 | 火网耐久负评统计 + 277 赞「无辐射热」原评 | `assets/evidence/amazon_fireside_mesh_durability_46pct_negative.png` + `assets/evidence/youtube_solostove_comment_no_radiant_heat.jpg` | ✅ 已有 |
| A8 | §2 ⑧ 「达人 UGC 跑赢自制混剪」 | 账户在投的达人 UGC 素材实貌 | `assets/ads/aroundfire/02_…_poster.jpg` + `01_…_poster.jpg`（可播 mp4） | ✅ 已有 |
| A9 | §2 ⑨ 「产品图 = 死路」 | 爆款母题账号 vs 产品图账号 vs 自家空阵地，三宫格 | `assets/social/gathergrills_ig_grid.jpg` + `biolite_ig_grid.jpg` + `aroundfire_ig_grid.jpg` | ✅ 已有 |
| A10 | §2 ⑩ 「渠道只有一条腿」 | Amazon 品类现状（Outland 家族） | `assets/trends/09_amazon_portable_fire_pit_reviewrank.png` + `assets/evidence/amazon_outland_rating_distribution.png` | ✅ 已有 |
| A11 | §3 P2「对比表从图片改回真 HTML 表格」 | 现状：整块对比表是一张 `alt=""` 图片 | `assets/ba/06_compare_before.png` | ✅ 已有 |

## B. index.html —— 12 张入口卡片全部无缩略图

| # | 卡片 | 缩略图 | 状态 |
|---|---|---|---|
| B1 | 执行摘要 | `assets/checkout/08_checkout_us_shipping_2490.png` | ✅ |
| B2 | 品类认知速成 | `assets/products/positioning_chart.png` | ✅ |
| B3 | 竞争格局 | ~~`assets/competitors/solostove_hero.png`~~ → **改用 `assets/competitors/breeo_hero.png`**（原图是 Cloudflare 验证页，见文末） | ✅ |
| B4 | 用户洞察 VOC | `assets/evidence/amazon_fireside_mesh_durability_46pct_negative.png` | ✅ |
| B5 | 广告情报 | `assets/ads/breeo/02_789668604211720.jpg` | ✅ |
| B6 | 社媒生态 | `assets/social/gathergrills_ig_grid.jpg` | ✅ |
| B7 | 市场趋势 | `assets/trends/01_5y_compare_5terms.png` | ✅ |
| B8 | SEO 关键词地图 | `assets/seo/01_keyword_opportunity_bubble.png` | ✅ |
| B9 | 网站诊断与优化 | `assets/ba/01_hero_after.jpg` | ✅ |
| B10 | 定价与商业模型 | `assets/checkout/20_checkout_qty2_us.png` | ✅ |
| B11 | Meta 投放诊断 | `assets/ads/aroundfire/07_…_poster.jpg` | ✅ |
| B12 | 达人库诊断 | `assets/ads/aroundfire/02_…_poster.jpg` | ✅ |

## C. category.html —— 39 张全是产品图，零证据图

| # | 锚点原文 | 补什么 | 素材 |
|---|---|---|---|
| C1 | `korean bbq table 的搜索曲线全年没有季节性` | KBBQ 5 年曲线 | `assets/trends/05_5y_kbbq.png` |
| C2 | `foldable korean bbq table 5 年搜索 +1,300% … Breakout` | Rising Queries 面板 | `assets/trends/07_rising_queries_panels.png` |
| C3 | `Reddit 里对这个品类的价格锚是 $20–30` | Reddit 价格锚原帖 + YouTube「$19 one on amazon」 | `assets/evidence/reddit_cheap_diy_alternatives_price_anchor.png` + `assets/evidence/youtube_tabletopfirepit_comment_price_vs_cheap.png` |
| C4 | `桌面不能被烧坏` / `太矮 28 次提及` | 两条原评截图 | `assets/evidence/youtube_mesa_comment_tabletop_heat_safety.png` + `assets/evidence/youtube_igt_table_comment_height_too_low.png` |
| C5 | `烧木柴——禁火令期违法` | 真实用户撞禁火令 | `assets/evidence/reddit_firebans_wood_not_allowed.png` |
| C6 | `丙烷…"不是真火"的心理折价` | 丙烷 vs 木柴辐射热讨论 | `assets/evidence/reddit_propane_vs_wood_radiant_heat.png` |
| C7 | `Amazon 品类销冠家族`（Outland） | 评分分布 + 品类排行 | `assets/evidence/amazon_outland_rating_distribution.png` |
| C8 | `AroundFire KBBQ 烤盘…埋在配件区` | 配件页现状 | `assets/shots/acc_desktop.png` |
| C9 | 术语黑话表搜索量列 | 关键词机会气泡图 | `assets/seo/01_keyword_opportunity_bubble.png` |
| C10 | 法条 blockquote（BLM / Mt. Hood 签署令） | 签署令原件截图 | ⛔ **无素材，未补**（需新截） |

## D. optimization.html —— 已有 63 图，但仍有 9 处实测事实无图（且 12 个已下载素材零引用）

| # | 锚点原文 | 补什么 | 素材 |
|---|---|---|---|
| D1 | `Loved By Our Customers 卡片…滚动进视口后复测…清晰` | 复测清晰的实拍 | `assets/shots/home_loved_section.jpg`（原零引用） |
| D2 | `页脚出现 UnionPay（银联）支付图标` | 页脚支付图标条 | `assets/shots/pdp_lite_compare.png`（**文件名有误导，实为页脚截图**，原零引用） |
| D3 | `Warm- 后面直接换行，是一个悬挂连字符` | 移动端首屏（悬挂连字符最明显） | `assets/shots/home_mobile_fold.png`（原零引用） |
| D12 | `竞品的信任资产密度是 Breeo The Original / Since 2011 / American Made…` | 竞品首屏原件 | `assets/competitors/breeo_hero.png` |
| D4 | `全部埋在默认收起的 Specifications 折叠块` / 火网 50 次 | PDP 右栏描述区 | `assets/shots/pdp_lite_y1400.png`（原零引用） |
| D5 | `必填字段数：9 个` / `没有 Klarna / Affirm / Afterpay` | 移动端结账整页（一图证 9 字段 + 无 BNPL + 小费 + 折扣码） | `assets/checkout/12_checkout_mobile.png`（原零引用） |
| D6 | 结账流程图组缺 ATC → 购物车这一步 | 加购抽屉（桌面 + 移动） | `assets/checkout/05_atc_drawer.png` + `assets/checkout/14_mobile_after_atc.png`（原零引用） |
| D7 | `空车状态：Your cart is empty` | 移动端空车 + 有货购物车的推荐位 | `assets/checkout/15_mobile_cart.png` + `assets/checkout/07_checkout_step1.png`（**实为带货购物车页**，原零引用） |
| D8 | `主 ATC 在 top=1163px（首屏之下 1.4 屏）` | 移动端 PDP 整页 | `assets/checkout/13_mobile_pdp.jpg`（原零引用） |
| D9 | `首页模块标题 3-in-1 Functionality / Patented 3-in-1 Technology` | 首页 3-in-1 模块 | `assets/shots/_hs2.png` + `assets/shots/_hs0.png`（原零引用） |
| D10 | `Hero 背景视频源分辨率 882×480…拉伸铺满` | Hero 1:1 裁切特写 | ⛔ **无素材，未补** |
| D11 | PDP FAQ 7 条原文引用 | FAQ 区截图 | ⛔ **无素材，未补** |

## E. ads.html —— 分析段（46–170 行）引用了 ~15 条素材，第一张图要到 202 行才出现

| # | 锚点原文 | 补什么 | 素材 |
|---|---|---|---|
| E1 | Q1 五家品牌的 headline 原文（`Bring Your Backyard Vision to Life` 等） | 五品牌代表素材缩略条 | `assets/ads/breeo/01_…jpg` / `solostove/03_…jpg` / `nomadgrills/02_…jpg` / `biolite/01_…jpg` / `kbbqbros/04_…jpg` |
| E2 | Q2 对照组：`Breeo 人物出现时全部是坐着的；Solo Stove 唯一一条是海滩上弹琴烤棉花糖` | 反例三宫格 + AroundFire 正例 | `assets/ads/breeo/02_…jpg` / `solostove/03_…jpg` / `kbbqbros/07_…jpg` / `aroundfire/03_…_poster.jpg` |
| E3 | Q3 `[159 天]` / `[144 天]` 两条最长在投 KBBQ 素材（blockquote 原文，无播放器） | 两条视频就地可播 | `assets/ads/kbbqbros/01_934579802442425.mp4` + `02_1250177180513838.mp4` |
| E4 | 差距 6 Breeo 点名打 Solo Stove 的证言素材 | Breeo 长青三条 | `assets/ads/breeo/01/02/03_…jpg` |
| E5 | 差距 1 `素材形式 100% 视频，零静态图` | 竞品静态图长什么样 | `assets/ads/breeo/05_…jpg` / `nomadgrills/05_…jpg` / `solostove/07_…jpg` |
| E6 | `Gather Grills 页面返回 "No ads match your search criteria"` | Ad Library 空结果页 | ⛔ **无素材，未补** |

## F. seo.html

| # | 锚点原文 | 补什么 | 素材 |
|---|---|---|---|
| F1 | `实测 <h1> 标签数 = 0` | 首页首屏（标题不是 H1） | `assets/shots/_hs0.png` |
| F2 | `title 仅 Accessories – AroundFire，无任何关键词` | 配件页 | `assets/shots/acc_desktop.png` |
| F3 | `集合页 仅 3 个` | 集合页现状 | `assets/shots/coll_desktop.png` |
| F4 | `全站唯一 KBBQ 资产是 $37 配件页` | 配件区实拍 | `assets/shots/acc_desktop.png` |
| F5 | `Breeo hero 直接写 Built for the Backyard、Solo Stove 首屏写…` | 竞品首屏原件 | **`assets/competitors/breeo_hero.png`**（Solo Stove 首屏未取得，图注已声明） |
| F6 | `Add a short description for your blog.`（博客占位文案） | `/blogs/news` 截图 | ⛔ **无素材，未补** |
| F7 | SERP 形态表（97% 视频位 / 89% Popular products） | 一张带标注的 SERP | ⛔ **无素材，未补** |

## G. trends.html

| # | 锚点原文 | 补什么 | 素材 |
|---|---|---|---|
| G1 | `一个 $33 的 Camping Stove 配件形式埋在配件区` | 配件页现状 | `assets/shots/acc_desktop.png` |
| G2 | `Gather Lite From $189（站内 57 条评价 4.91★）` | 官网 PDP 首屏 | `assets/shots/pdp_lite_desktop_fold.png` |
| G3 | `Ignik FireCan 能在 portable fire pit 的 5 年 Rising Queries 里排第一` | 产品形态（丙烷罐式） | `assets/products/Ignik_FireCan_Deluxe_Fire_Pit.jpg` |
| G4 | `信号 C · 玩家结构 —— 三个价格层` | 定位坐标图 | `assets/products/positioning_chart.png` |
| G5 | `Dealers & Distributors 页实测为纯招募表单` | 招商页截图 | ⛔ **无素材，未补** |
| G6 | `没有一个是「火盆+烤架+桌面」一体化产品` | 该词 SERP 截图 | ⛔ **无素材，未补** |
| G7 | 禁火令三条 .gov 法条原文引用 | 签署令原件 | ⛔ **无素材，未补** |

## H. voc.html

| # | 锚点原文 | 补什么 | 素材 |
|---|---|---|---|
| H1 | §1.1 对标 SKU 表（11 行，形态是分析重点） | 四款对标品形态图 | `assets/products/OutlandLiving_Standard_Propane_Fire_Pit.jpg` / `FiresideOutdoor_Trailblazer_Pop_Up_Fire_Pit.jpg` / `Blackstone_Camping_Griddle_20x14.jpg` / `SoloStove_Bonfire_2_0_Smokeless_Fire_Pit.jpg` |
| H2 | `比价对象是三层，不是一层` | 定位坐标图 | `assets/products/positioning_chart.png` |
| H3 | `Korean BBQ is my favorite way to eat, period.`（168 赞） | 原帖截图 | ⛔ **无素材，未补** |
| H4 | 300g 火网特写 | 火网结构特写 | ⛔ **无素材，未补** |

## I. social.html

| # | 锚点原文 | 补什么 | 素材 |
|---|---|---|---|
| I1 | Breeo / NOMAD / Snow Peak 三家 `IG 主页网格截图未取得`（视觉风格段落无图） | 用已抓到的广告静帧 / 产品图作替代（并注明是替代） | `assets/ads/breeo/02_…jpg` / `assets/ads/nomadgrills/05_…jpg` / `assets/products/SnowPeak_Collapsible_IGT_4_Unit_Set.jpg` |
| I2 | `自制"NEW FAVORITE OUTDOOR"黄字贴纸那条` / `两套调性混在一个网格里` | AroundFire 两种调性素材并排 | `assets/ads/aroundfire/06_…_poster.jpg` + `02_…_poster.jpg` |
| I3 | `IGT-maxxing all summer long`（Snow Peak 模块化叙事） | IGT 模块化产品图 | `assets/products/SnowPeak_Collapsible_IGT_4_Unit_Set.jpg` |
| I4 | Gather Grills 287 万播放那条 Reel / KBBQ Bros 6.9 万赞那条 / Breeo 25.8 万播放科普片 | 原帖封面帧 | ⛔ **无素材，未补**（IG/TikTok 对本机 IP 限流，缩略图未加载） |

---

## 汇总（执行完毕）

| 页面 | 补图前 img / video | 补图后 img / video | 净增 |
|---|---|---|---|
| summary.html | 0 / 0 | **18 / 2** | +20 |
| index.html | 0 / 0 | **12 / 0** | +12 |
| category.html | 39 / 0 | 51 / 0 | +12 |
| optimization.html | 63 / 0 | 76 / 0 | +13 |
| ads.html | 37 / 40 | 50 / 43 | +16 |
| voc.html | 31 / 0 | 36 / 0 | +5 |
| social.html | 21 / 0 | 26 / 0 | +5 |
| trends.html | 10 / 0 | 14 / 0 | +4 |
| seo.html | 4 / 0 | 8 / 0 | +4 |
| **合计** | | | **+91** |

- 缺口条目合计 **58 条**（A 11 / B 12 / C 10 / D 11 / E 6 / F 7 / G 7 / H 4 / I 4，扣除跨页重复计数）
- **44 条已补**（对应上表 91 张图/视频，部分条目一条配多图）
- **14 条无现成素材、未补**：C10（禁火令签署令原件）、D10（Hero 视频分辨率特写）、D11（PDP FAQ 区截图）、E6（Gather Grills Ad Library 空结果页）、F6（`/blogs/news` 占位文案）、F7（SERP 形态截图）、G5（招商页）、G6（`fire pit grill table portable` SERP）、G7（三条 .gov 法条原件）、H3（Reddit 168 赞 KBBQ 原帖）、H4（火网特写）、I4×3（Gather Grills 287 万播放 Reel / KBBQ Bros 6.9 万赞 Reel / AroundFire 自有最佳帖封面帧）
  - 均为需重新访问外站或官网新截的「说明性」缺口，非结论性缺口
  - **所有相关文字结论保持原样，未因缺图删改，也未新增任何无数据支撑的结论**；"未取得 / 未查证"声明全部原样保留
- 原「已下载但零引用」的 18 个素材，本次消化 16 个
  - `shots/_hs3.png` 未用：内容是懒加载未触发的 Instagram 占位块，属取证伪影，用了会误导
  - `checkout/14_mobile_cart_drawer.png` 未用：与 `14_mobile_after_atc.png` 内容重复，取其一

---

## 本次顺带发现的两个素材问题（需知会）

1. **`assets/competitors/solostove_hero.png` 不是 Solo Stove 首屏**，实际内容是 Cloudflare 的 `Managed Challenge / Your connection is being verified` 验证页（文件仅 36 KB）。
   - 本次在 index.html 与 seo.html 里**已改用 `assets/competitors/breeo_hero.png`**（内容正确：`THE ORIGINAL SMOKELESS FIRE PIT` + 副标 `Hand Crafted, American Made Fire Pits Built for the Backyard`，正是报告引用的原文）
   - seo.html 图注已如实写明「Solo Stove 首屏截图本次未取得——抓取返回 Cloudflare 验证页，未以该页冒充首屏」
   - ⚠️ **competitors.html 若引用了这张图，需要换掉**（该文件由另一人负责，本次未碰）
2. **`assets/competitors/` 下 4 个文件超过 800 KB**：`nomad_hero.png` 1,499 KB、`snowpeak_hero.png` 1,739 KB、`gather_hero.png` 1,074 KB、`ignik_hero.png` 837 KB。
   - 这批是他人新增的素材，本次未压缩也未引用（除 `breeo_hero.png` 680 KB，未超线）
   - 建议由 competitors.html 负责人统一压到 800 KB 以内

## 本次做的一处事实性收窄（有截图支撑，非改结论）

`optimization.html` P2-16 原文写「购物车页**无加购推荐**、无免邮进度条」。
调阅 `assets/checkout/07_checkout_step1.png`（文件名误导，实际拍的是**有货状态的购物车页**）后确认：**有货购物车是有 `You may also like` 推荐位的**，4 张配件卡（KBBQ 烤盘 $37 / Gather Grande / Light Stand $33 / Camping Stove $33）各带 Add to cart。
因此把标题与实测事实**收窄到「空车态无推荐」**，并把这张图连同 `15_mobile_cart.png` 一起补进证据组，图注写明「复测更正」。**免邮进度条 / 信任徽章缺失这两条结论未变**，另据图补了一条同样有截图支撑的事实：推荐位副标题仍是 Shopify 默认占位文案 `Describe your featured collection here`。

## 汇总

- 缺口条目合计 **58 条**（A 11 / B 12 / C 10 / D 11 / E 6 / F 7 / G 7 / H 4 / I 4 —— 去掉重复统计口径后按下表执行）
- 其中 **44 条有现成素材、本次已补**
- **14 条无现成素材、本次未补**（C10 / D10 / D11 / E6 / F6 / F7 / G5 / G6 / G7 / H3 / H4 / I4×3），原因均为：证据需重新访问外站或官网新截，且属于「说明性」而非「结论性」缺口；所有相关文字结论保持原样，未因缺图删改，也未新增任何无数据支撑的结论。
- 原「已下载但零引用」的 18 个素材，本次消化 16 个（`shots/_hs3.png` 为懒加载捕获伪影不用；`checkout/14_mobile_cart_drawer.png` 与 `14_mobile_after_atc.png` 重复，取其一）。

## 硬性约束执行情况（已逐条验证）

- **单张图片 > 800KB**：全量扫描 `assets/`，本次**引用到的图片没有一张超过 800 KB**（超线的 4 个文件在 `assets/competitors/`，非本次引用，已在上方列出待处理）。视频统一 `preload="none"` + poster，不影响首屏
- **alt + 图注**：脚本校验全站 **0 张 `<img>` 缺 `alt`**；本次新增的每一张图都在 `<figcaption>` 里写明「这张图证明了什么」
- **长截图容器内滚动**：统一套站内既有的 `.tall` / `.tall.short`（`max-height + overflow-y:auto`），未新造类
- **视频**：统一 `<video controls preload="none" playsinline poster="…">`
- **窄屏不横向滚动**：Playwright 在 **390px 与 1280px 两个视口逐页实测 9 个页面**，`document.documentElement.scrollWidth > innerWidth` 全部为 false
- **沿用站内 CSS 令牌与卡片样式**：未改动 `assets/site.css`（避免与并行改动冲突）。index.html 新增的缩略图样式写在该页 `<style>` 内，只有 3 条规则，颜色/圆角全部取自既有 `--line` / `--r` / `--sand2` / `--ink3`
- **引用完整性**：脚本校验全站 **394 处 `src` / `poster` 引用，文件全部真实存在**
- **HTML 结构**：9 个改动页面逐页做标签配平检查，**无未闭合、无错配**
