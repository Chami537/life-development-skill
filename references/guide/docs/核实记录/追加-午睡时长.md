# 追加：午睡时长一条 · 核实记录（2026-09-21）

任务来源：用户问「有没有午睡相关的内容，推不推荐加」。

原有覆盖：全书搜「午睡」「小睡」「打盹」「午休」，只有第 3 节第 11 条（下午困了就睡 10 分钟，不要睡半小时），口径是时间与精力，只讲提神效果和睡眠惰性，不涉及死亡率。第 2 节第 13 条（每晚睡 7 小时左右）备注里提了「睡得长风险高多半是因果反过来」，但说的是夜间睡眠，没提午睡。午睡时长与死亡率、心血管：零覆盖。

落点：第 2 节第 39 条，追加在节末。追加而不是插在第 13 条（每晚睡 7 小时）后面，是为了不触发条号顺延——第 2 节有 38 条、被别节引用多处，插入要整体重编号并逐处核对引用，收益不值这个风险。口径记死亡率。

## 文献（三篇，数字取自 Europe PMC core 记录与 PMC 全文原文）

| DOI | 复核 | 关键数字原文 |
|---|---|---|
| <https://doi.org/10.3389/phrs.2026.1609013> | 是（Du P, Li J, Hua Z, Sun Y, Song S, Liao Y, Cheng S, Li X. Public Health Reviews 2026;47:1609013，PMID 41710553） | 「This umbrella review identified 16 meta-analyses encompassing 244 health-related outcomes.」「Napping for <60 min maximizes cognitive enhancement (SMD = 0.69, 95% CI: 0.37-1.00) and reduces fatigue, while minimizing the risk of all-cause mortality and chronic diseases.」「Napping for >60 min correlates with a 30% higher risk of coronary heart disease and a 20% increased risk of diabetes and obesity; short naps (20-30 min) improve athletic performance (SMD = 0.99, 95% CI: 0.67-1.31)」 |
| <https://doi.org/10.1001/jamanetworkopen.2026.7938> | 是（Gao C, Cai R, Zheng X, Gaba A, Yu L, Buchman AS, Bennett DA, Gao L, Hu K, Li P. JAMA Netw Open 2026;9:e267938，PMID 42008265） | 「community-dwelling adults aged 56 years or older」「Daytime napping, defined as sleeping between 9 am and 7 pm and assessed by up to 14 days of actigraphy data.」「Among 1338 participants over a mean (SD) follow-up of 8.30 (4.78) years ... 926 (69.2%) died」「longer daytime nap duration (adjusted hazard ratio [AHR] per 1-hour increase, 1.13; 95% CI, 1.04-1.23; P = .005) and higher nap frequency (AHR per additional daily nap, 1.07; 95% CI, 1.02-1.13; P = .003) at baseline were associated with increased mortality. Morning nappers had higher mortality risk compared with early afternoon nappers (AHR, 1.30; 95% CI, 1.03-1.64; P = .03).」 |
| <https://doi.org/10.1038/s41467-020-20585-3> | 是（Dashti HS et al. Nat Commun 2021;12:900，PMID 33568662，PMC7876146 全文 XML 逐字抓取） | 摘要：「a genome-wide association study of self-reported daytime napping in the UK Biobank (n = 452,633) and identify 123 loci of which 61 replicate in the 23andMe research cohort (n = 541,333)」「Mendelian randomization shows potential causal links between more frequent daytime napping and higher blood pressure and waist circumference.」正文：「We observed a potentially causal effect of more frequent daytime napping on higher diastolic blood pressure (DBP; 0.25 standard deviation (SD) unit increase per category increase in daytime napping, 95% CI [0.15, 0.34], P = 2.99 × 10−7), systolic blood pressure (SBP; 0.18 SD units, [0.09, 0.27], P = 5.15 × 10−5), and waist circumference (0.28 SD units, [0.11, 0.45], P = 1.3 × 10−3)」；另「This analysis revealed no associations of the variants with cardiovascular outcomes」，1402 个 ICD 表型的无假设扫描「found no variant-disease associations」 |

## 定级与取舍

- **定 B，不定 A**：两项主证据都是只记录、不分组的观察研究，反向因果重（睡眠呼吸暂停、贫血、甲减、抑郁、慢性病都会让人白天长睡）。伞形综述本身汇总的也是观察性荟萃，AMSTAR-2/GRADE 在摘要里没给逐个结局的等级，不能按 A 级的「可量化且设计硬」算。
- **收益定「中」，没按阈值定「大」**：死亡率口径的阈值是相对降幅 ≥20% 记「大」，冠心病 30%、死亡风险每小时 13% 按字面够得上「大」。压到「中」的理由是这些是关联不是干预效果，而 MR 这一侧只支持血压和腰围的弱因果、查不到对冠心病和糖尿病的因果影响，读者照做能拿到的实际折扣远小于字面数字。属于「数字不足以判定时用判断」，按规矩在这里写明。
- **标了「争议」**：正反两侧确实对立——观察性证据说长午睡和死亡、冠心病连在一起，基因证据说这条因果链查不到。两边都写进备注。
- **Dashti 的 SD 单位没换算成 mmHg**：论文用 UK Biobank 的样本标准差（SBP 11.25 mmHg、DBP 20.65 mmHg）做标准化，DBP 的 SD 明显偏大、SBP 偏小，换算出来的毫米汞柱数不可靠。正文只写方向「血压和腰围越高一点」，不给数字。
- **「去查原因」那半是 C 级**：夜间睡眠呼吸暂停、贫血、甲减、抑郁会造成白天长睡，这是临床常识，但「查了能降多少死亡率」没有可引的干预证据。已在备注里标明属于作者建议。
- **没写的**：午睡能不能补回前一晚缺的觉——实验室 RCT 只有短期替代终点，且与第 3 节第 11 条重复，未收。希腊 EPIC 队列（Naska 2007）说午睡降冠心病死亡、Häusler 2019 说每周 1 到 2 次午睡风险低，方向相反且样本小，已被伞形综述涵盖，未单列。
- 受益人：第①档（你自己）。
