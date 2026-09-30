# 追加：勃起功能障碍两条 + 嫖娼一条 · 核实记录（2026-09-21）

任务来源：GitHub issue #21，标题「"性压抑"算不算这个时代下的一种健康问题」，正文空，无评论。

**原题没有直接写成条目。** 「算不算一种健康问题」是概念判断，既没有可量化的终点，也没有给读者的动作。按本书的规矩，这样的条目只能落在 C 级观点上，不写。改成从这个话题里挑出三件能量化、能给动作的事来写。

原有覆盖：全书搜「性」「勃起」「卖淫」「嫖娼」「性病」，性健康这一块只有第 1 节第 28、29 条（安全套、查艾滋，本轮之后改为第 30、31 条）和第 13 节第 38 条（72 小时阻断药）；勃起功能只在第 28 节第 3 条（合成代谢类固醇的副作用）里作为副作用出现过一次；卖淫嫖娼只在第 22 节第 4 条引娱乐场所条例时带过「禁止卖淫嫖娼的警示标志」。作为独立条目：零覆盖。

落点：
- 第 1 节新增第 28、29 条，插在第 27 条（肉眼血尿）后面。放这里是因为第 28 条和第 27 条是同一个形状——一个不疼不痒的信号，去查一次可能提前几年发现要命的病。**插入导致原第 28 至 34 条顺延为第 30 至 36 条**，跨节引用同步改了 8 处（第 6 节第 18 条、第 9 节第 22 条两处、第 13 节第 38 条、第 17 节第 8 条、第 29 节节首与第 13 条），节内引用改了 3 行 5 处。`docs/引用对照.md` 的 diff 逐行看过：所有变动行都是「条号变了、指向的条目不变」，没有出现条号未变而指向变了的行。`node tools/check-refs.mjs --check` 通过，引用总数 504 → 514（新增 10 处，与本轮实际新写的引用数对得上）。
- 第 9 节新增第 23 条（嫖娼），追加在末尾，不插队，不产生顺延。

刻意没写的：
- **性生活频率与死亡率**（Caerphilly 那一类队列）。单一队列、反向因果重（身体好的人性生活多），写进来要背一个说不清方向的「争议」，价值低于成本。
- **「性压抑有害」或者「无害」的任何断言**。本轮没有找到能逐字核对的量化证据。
- **网购「壮阳」保健品偷加西地那非**没有单开条目。放第 28 节不合适（那节是「为了外形」），单开又太窄，压成第 28 条备注里的一句，并引美国药品说明书库的禁忌原文。

## 文献（全部取回摘要逐字核对）

| 来源 | 复核 | 用到的原文数字 |
|---|---|---|
| Vlachopoulos CV 等 (2013). Prediction of cardiovascular events and all-cause mortality with erectile dysfunction. Circ Cardiovasc Qual Outcomes 6(1):99-109. <https://doi.org/10.1161/CIRCOUTCOMES.112.966903>（PMID 23300267） | 是（Europe PMC resultType=core 摘要全文） | 「Of the 14 studies included (92 757 participants; mean follow-up, 6.1 years…)」；「The pooled RRs for the above-mentioned end points were 1.44 (95% CI, 1.27-1.63), 1.19 (95% CI, 0.97-1.46), 1.62 (95% CI, 1.34-1.96), 1.39 (95% CI, 1.23-1.57), and 1.25 (95% CI, 1.12-1.39), respectively」，依次对应总心血管事件、心血管死亡、心梗、脑血管事件、全因死亡；「The RR was higher in intermediate- compared with high- or low-CV-risk populations and with younger age」；问卷判定 RR 1.61（1.38-1.86）对只问一句话 RR 1.27（1.18-1.37），P=0.006 |
| Gupta BP 等 (2011). The effect of lifestyle modification and cardiovascular risk factor reduction on erectile dysfunction. Arch Intern Med 171(20):1797-1803. <https://doi.org/10.1001/archinternmed.2011.440>（PMID 21911624） | 是（同上） | 「A total of 740 participants from 6 clinical trials in 4 countries」；「weighted mean difference, 2.66 (95% CI, 1.86-3.47)」；「If the trials with statin intervention (n = 143) are excluded, the remaining 4 trials of lifestyle modification interventions (n = 597)…weighted mean difference, 2.40 (95% CI, 1.19-3.61)」；纳入条件为随访至少 6 周的随机对照试验 |
| Rosen RC 等 (1999). Development and evaluation of an abridged, 5-item version of the IIEF (IIEF-5). Int J Impot Res 11(6):319-326. <https://doi.org/10.1038/sj.ijir.3900472>（PMID 10637462） | 是（同上） | 「a cutoff score of 21 (range of scores, 5-25)」；「ED was classified into five severity levels, ranging from none (22-25) through severe (5-7)」。只用来给读者一个刻度，不给诊断标准 |
| DailyMed（美国国立医学图书馆的药品说明书库）. VIAGRA (sildenafil citrate) tablet. <https://dailymed.nlm.nih.gov/dailymed/lookup.cfm?setid=d905dc8d-917f-4ea3-a4ee-a1ecf6967d4e> | 是（页面正文逐字抓取） | 「CONTRAINDICATIONS · Administration of VIAGRA to patients using nitric oxide donors, such as organic nitrates or organic nitrites in any form. VIAGRA was shown to potentiate the hypotensive effect of nitrates」 |

两处刻意的取舍：① **没有引 ACC/AHA 1999 年那份西地那非与心血管病的专家共识**（Cheitlin MD 等，JACC 33:273-282 / Circulation 99:168-177）。Europe PMC 只有题录、没有摘要，禁忌那句话逐字核不了，所以改引能逐字核对的说明书原文。② **没有引 Ishikura 2000 那篇 Circulation**（西地那非合用硝酸酯的血流动力学研究）——受试者是比格犬，不是人。

## 法条（逐字核对）

| URL | 复核 | 原文引句 |
|---|---|---|
| <https://www.spp.gov.cn/spp/fl/202506/t20250627_699863.shtml> | 是（最高检转载全文，逐字抓取） | 《治安管理处罚法》（2025 年修订）第七十八条：「卖淫、嫖娼的，处十日以上十五日以下拘留，可以并处五千元以下罚款；情节较轻的，处五日以下拘留或者一千元以下罚款。在公共场所拉客招嫖的，处五日以下拘留或者一千元以下罚款。」第七十九条：「引诱、容留、介绍他人卖淫的，处十日以上十五日以下拘留，可以并处五千元以下罚款；情节较轻的，处五日以下拘留或者一千元以上二千元以下罚款。」第八十七条：「旅馆业、饮食服务业、文化娱乐业、出租汽车业等单位的人员，在公安机关查处吸毒、赌博、卖淫、嫖娼活动时，为违法犯罪行为人通风报信的，或者以其他方式为上述活动提供条件的，处十日以上十五日以下拘留……」 |
| <https://jtgl.beijing.gov.cn/jgj/jgxx/flfg/fl/11033925/index.html> | 是（北京市公安交管局转载的整合文本，经刑法修正案十一修正） | 「第三百六十条 【传播性病罪】明知自己患有梅毒、淋病等严重性病卖淫、嫖娼的，处五年以下有期徒刑、拘役或者管制，并处罚金。」整合文本里第三百六十条**只有一款** |
| <https://www.spp.gov.cn/spp/fl/201802/t20180205_364562.shtml> | 是（最高检转载全文） | 刑法修正案（九）「四十三、删去刑法第三百六十条第二款。」被删的就是嫖宿幼女罪 |

一处必须注意的版本坑：最高检那份刑法全文（`t20180206_364975.shtml`）是 **1997 年原始文本**，第三百六十条还带着第二款「嫖宿不满十四周岁的幼女的，处五年以上有期徒刑，并处罚金」。正文引的是整合文本 + 修正案九，两处都给了链接。这一点和本仓库既有的做法一致。

## 量级与口径怎么定的

- 第 1 节第 28 条（勃起功能障碍去查心血管）：口径死亡率，收益记「中」。44% 是两群人的风险差距，不是「去查一次能降多少死亡」，所以不按 ≥20% 的阈值机械记「大」；但它也不同于第 27 条（肉眼血尿）那种只有检出率的信号——这里查出来的高血压、糖尿病、血脂异常都有现成的治疗办法，所以不记「小」。理由已写进备注。
- 第 1 节第 29 条（改生活方式）：口径死亡率，收益记「小」。终点只有 IIEF-5 问卷评分这个替代终点，按阈值就是「小」。硬终点在第 2 节第 1、33 条和第 1 节第 7 条，备注里指过去了。
- 第 9 节第 23 条（嫖娼）：口径自由，收益记「中」。按自由口径的阈值，避免的是行政拘留，就是「中」；传播性病罪那一档才够「大」，但那一档有「明知自己患有严重性病」这个前提，不是默认情形，所以按默认档记。
