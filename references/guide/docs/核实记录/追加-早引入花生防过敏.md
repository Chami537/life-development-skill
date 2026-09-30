# 追加：早引入花生一条 · 核实记录（2026-09-21）

任务来源：用户看完生物钟长文后问「人体还有没有其他神奇的机制可以加的」。筛选口径不是「机制奇不奇」，是「知道了这个机制，读者的动作会不会变」。按这个筛出四条候选，用户选了先写第一条。

原有覆盖：全书搜「花生」零。「过敏」出现在第 6 节、第 13 节、第 20 节，但第 20 节那处只是说「所谓过敏性体质、家里人有过敏史、以前对食物药物过敏过，都不是疫苗禁忌」，讲的是接种，不是食物引入。本主题零覆盖。

落点：第 20 节第 12 条，追加在节末不动条号。

## 文献

| DOI | 复核 | 关键数字原文 |
|---|---|---|
| <https://doi.org/10.1056/NEJMoa1414850>（主证据，LEAP） | 是（Du Toit G, Roberts G, Sayre PH, 等. NEJM 2015;372(9):803-813，PMID 25705822） | 「We randomly assigned 640 infants with severe eczema, egg allergy, or both to consume or avoid peanuts until 60 months of age. Participants, who were at least 4 months but younger than 11 months of age at randomization, were assigned to separate study cohorts on the basis of preexisting sensitivity to peanut extract, which was determined with the use of a skin-prick test—one consisting of participants with no measurable wheal after testing and the other consisting of those with a wheal measuring 1 to 4 mm in diameter.」「Among the 530 infants in the intention-to-treat population who initially had negative results on the skin-prick test, the prevalence of peanut allergy at 60 months of age was 13.7% in the avoidance group and 1.9% in the consumption group (P<0.001). Among the 98 participants in the intention-to-treat population who initially had positive test results, the prevalence of peanut allergy was 35.3% in the avoidance group and 10.6% in the consumption group (P=0.004). There was no significant between-group difference in the incidence of serious adverse events.」 |
| <https://doi.org/10.1056/NEJMoa1514210>（备注·一般人群，EAT） | 是（Perkin MR, Logan K, Tseng A, 等. NEJM 2016;374(18):1733-1743，PMID 26943128） | 「In the intention-to-treat analysis, food allergy to one or more of the six intervention foods developed in 7.1% of the participants in the standard-introduction group (42 of 595 participants) and in 5.6% of those in the early-introduction group (32 of 567) (P=0.32). In the per-protocol analysis, the prevalence of any food allergy was significantly lower in the early-introduction group than in the standard-introduction group (2.4% vs. 7.3%, P=0.01), as was the prevalence of peanut allergy (0% vs. 2.5%, P=0.003) and egg allergy (1.4% vs. 5.5%, P=0.009)」「The early introduction of all six foods was not easily achieved but was safe.」「The trial did not show the efficacy of early introduction of allergenic foods in an intention-to-treat analysis.」 |
| <https://www.gov.cn/zhengce/zhengceku/2020-08/01/content_5531915.htm>（安全前提） | 是（国家卫生健康委办公厅《婴幼儿喂养健康教育核心信息》，2020-07-29 印发，从 gov.cn 政策文件库逐字抓取） | 「整粒花生、坚果、果冻等食物易吸入气管，引起窒息，婴幼儿应当避免食用。」 |

## 中国官方文件查了什么、查到什么

用国务院政策文件库 JSON 接口（`searchfield=title`）检索「婴幼儿喂养」，命中两份现行文件，都逐字抓下来做了关键词统计：

| 文件 | 过敏 | 致敏 | 回避 | 花生 |
|---|---|---|---|---|
| 《婴幼儿喂养健康教育核心信息》（2020） | 0 | 0 | 0 | 2（都是窒息警告） |
| 《婴幼儿营养喂养评估服务指南（试行）》（2025-02） | 2（都是「牛奶蛋白过敏影响铁吸收」的语境） | 0 | 0 | 0 |

**结论：中国官方喂养文件目前对「该早引入还是该回避易过敏食物」没有任何说法。** 正文备注里写明了这一点，并交代这条是按国际试验证据写的。《中国居民膳食指南》是中国营养学会的出版物、不是政府文件，本轮未取，也没引。

## 定级与取舍

- **定 A**：LEAP 是随机对照试验，按分组分析（ITT）就显著，两个队列都显著，数字可逐字核对。
- **收益定「大」**：13.7% 降到 1.9%，相对降幅约 86%，远超死亡率口径「≥20% 记大」的阈值。
- **成本定「钱=少」不是 0**：要买花生酱（几十元），加之前还要看一次医生。
- **三条安全边界必须写，缺一条这条就是危险的**：
  1. **绝不能给整粒花生**——卫健委明文，窒息。形式只能是花生酱调稀或花生粉拌辅食。备注里指向第 13 节第 28 条（有人噎住说不出话）。
  2. **必须先看医生评估，不许自己在家试**——LEAP 入组前每个孩子都做了皮试，**风团大于 4 毫米的被排除在试验之外**，试验从没让这些孩子吃过花生。摘要里「no measurable wheal」和「1 to 4 mm」两个队列就是证据。
  3. **只针对高危孩子**（重度湿疹或已有鸡蛋过敏），不是所有婴儿。
- **一般婴儿那一侧照实写弱**：EAT 试验按分组算不显著（5.6% 对 7.1%，P=0.32），只有符合方案分析才显著。备注写明「这种算法容易把效果说大，作者自己说按分组算没能证出效力」，同时保留「早引入是安全的」这一条作者原话。
- **没标「争议」**：LEAP 和 EAT 不是对立的两派，两者人群不同（高危 vs 一般），结论也不矛盾。按规矩只有对立证据才标争议，这里改为在备注里把适用范围划清。
- **处理了与第 20 节第 4 条的时间冲突**：LEAP 从 4 月龄起，中国是满 6 月龄加辅食。备注写明这个差异，落点交给医生，不替读者定。第 4 条备注也加了互指。
- 受益人：第②档（子女）。

## 同批候选里没写的三条

- **他汀肌痛多半是反安慰剂（SAMSON）**：NEJM 那篇是研究快报无摘要，完整版在 JACC 2021;78:1210-1222（DOI 10.1016/j.jacc.2021.07.022，Crossref 题录已核），本轮没拿到逐字数字，未写。
- **晕针晕血时绷紧肌肉防晕厥**：证据强度未查。
- **卧床老人口腔护理防吸入性肺炎**：证据强度未查，第 17 节现有 8 条无此条。
