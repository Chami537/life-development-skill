# 排查：备注里的文献链接 · 记录（2026-09-21）

任务来源：用户在检索页上读到第 2 节第 1 条（戒烟）的备注，里面嵌着一整串英文题录，说「这里怎么还有啊，读者都是中国人，你整个一长串这些放着」。

此前同一天已经处理过两条（第 2 节第 41 条夜班、第 6 节第 26 条早餐），当时只修了链接最多的两条，没做全书扫查。这一轮补齐。

## 判据与口径

- **文献链接一律进「来源」栏，备注不放。** 备注里至多留一个链接，且只能是指向 docs/ 长文的相对链接。
- 依据：CLAUDE.md 的通俗化规则明写「**来源栏除外**，文献题录和条款号照原样留着才能核对」——言下之意，英文题录的容身处就是来源栏。备注是给中国读者读的中文正文，塞进一串英文题名和 DOI 既读不懂也不该读。
- 扫描命令：`grep -c http` 扫全书所有 `- 备注：` 行。

## 处理前后

| | 处理前 | 处理后 |
|---|---|---|
| 备注里带链接的条目 | 19 条（其中 11 条是整串英文题录嵌在中文里） | **0 条** |
| 单条备注最多链接数 | 3 个 | 0 个 |
| 全书文献链接总数 | 1234 | **1234（未变）** |

链接总数不变是这轮的核心不变量：**题录是从备注挪到来源栏，不是删掉**。挪进来源时给每条加了一个中文小尾巴说明它撑的是哪个说法（「（争议方）」「（备注里那项高纯度处方鱼油试验）」之类），免得来源栏变成一串看不出用途的题录。

## 逐条清单

第 1 节：第 20 条（流感疫苗 Cochrane）、第 28 条（PrEP，Fonner 2016）、第 29 条（窗口期，广东疾控页面）。
第 2 节：第 1 条（二手烟 Oberg 2011）、第 9 条（低钠盐争议方 PURE）、第 19 条（加工肉争议方 NutriRECS 指南）、第 20 条（饮酒争议方 Di Castelnuovo 2006）、第 34 条（BMI 争议方 Flegal 2013）、第 41 条（夜班癌症两篇 + 光照 Czeisler，先一轮已处理）。
第 3 节：第 9 条（两篇争议方 Grubbs 2018、Prause & Pfaus 2015）。
第 5 节：第 17 条（指数基金争议方 Harvey & Liu 2022）。
第 6 节：第 1 条（复合维生素 Gaziano 2012）、第 2 条（鱼油 Bhatt 2019 REDUCE-IT）、第 26 条（早餐三篇，先一轮已处理）。
第 10 节：第 3 条（Perilloux & Kurzban 2015）、第 6 条（Dargie 2015）。
第 20 节：第 12 条（一般婴儿试验 EAT，Perkin 2016）。
第 29 节：第 4 条（Kristensen 2012）、第 9 条（Stroebe 2007）。

## 补全的题名

有 5 条原来在备注里是缩写形式（只有作者、年份、期刊），挪进来源栏要补题名。**没有凭记忆写**，逐条用 Crossref 按 DOI 取回：

| DOI | 取回的题名 |
|---|---|
| 10.1097/QAD.0000000000001145 | Effectiveness and safety of oral HIV preexposure prophylaxis for all populations（AIDS, 2016） |
| 10.1001/jama.2012.14641 | Multivitamins in the Prevention of Cancer in Men（JAMA, 2012） |
| 10.1056/NEJMoa1812792 | Cardiovascular Risk Reduction with Icosapent Ethyl for Hypertriglyceridemia（NEJM, 2019） |
| 10.1007/s10508-018-1248-x | Pornography Problems Due to Moral Incongruence: An Integrative Model with a Systematic Review and Meta-Analysis（Arch Sex Behav，**Crossref 记的年份是 2018 不是原文写的 2019**，已按 2018 写） |
| 10.1002/sm2.58 | Viewing Sexual Stimuli Associated with Greater Sexual Responsiveness, Not Erectile Dysfunction（Sexual Medicine, 2015） |

## 校验

- 全书 `- 备注：` 行含 http 的条数：**0**。
- 删除引文后扫了一遍标点，没有留下双句号、空括号或孤立的「。」。
- `node tools/check-refs.mjs --check`：454 处引用全部指向正确且带锚点，条数未变。
- `sync-stats.ps1`：条目 600、A 404、链接 1234，八处统计位一个没动。
