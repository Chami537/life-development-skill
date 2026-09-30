# 第 5 节追加：处置效应与暴涨暴跌期的主动交易（2026-09-22）

任务来源：GitHub issue #24（wangchao732）。原文是「劝大家别炒 A 股，90% 的散户被套进去。套进去了又不肯割肉，短时间 1 年想出来几乎不可能。还想着越低越补，即伤命又伤财」。

原有覆盖：第 5 节已经有一组投资条目——第 15 条（不频繁交易股票，Barber-Odean 2000，换手最高组年化 11.4% 对市场 17.9%）、第 16 条（不借钱不加杠杆）、第 17 条（宽基指数基金替代主动基金）、第 18 条（同类基金选费率低的）、第 19 条（不押单一标的）、第 27 条（先存应急金）。也就是说「别频繁买卖、别借钱、别押一只」这三件事已经写了。

issue 里真正没被覆盖的是两件：① **卖出决策的偏差**（赚了就卖、亏了死扛、还往下补仓），全书零覆盖；② **暴涨暴跌期的主动交易账**，第 15 条讲的是长期换手成本，没有讲「行情疯的时候动手」这一段，而且它引的是美国 1990 年代数据，没有中国的量。

落点：第 5 节节末新增第 37、38 条，不插在第 15 到 19 条的投资簇中间。理由是插入会让第 20 到 36 条整体顺延，全书指向第 5 节的 7 处跨节引用和本节十几处自引都要跟着改，而按 CLAUDE.md 的口径这类顺延撞歪对照表 diff 也不一定看得出来。节末追加零风险，检索页本来就按性价比重排，读者不靠纸面顺序找条目。第 36 条（散装食品）也是这么追加的。

## 没有采纳 issue 的结论口径

**不写「别炒 A 股」。** 按 CLAUDE.md「只拆账不给结论」和「判断一条只给禁止不给出路之前先确认当事人是不是真的没得选」两条：第 17 条已经给了「拿钱进股市」的低成本走法（宽基指数基金），再写一条「一律别买」会和它直接冲突。所以这两条写的都是动作层面的差别——同一笔钱、同一段行情，卖出规则怎么定、行情最热时动手多少，而不是「进不进场」。

**不写「90% 的散户亏钱」。** 这个数字在网上流传很广，但查不到可逐字核对的官方统计：上交所、深交所的统计年鉴和投资者状况调查报告没有给出「亏损账户占比」这一项的公开时间序列，本轮也没有找到可引的原始文献。按项目规则「不确定的数字宁可不写」，第 38 条备注里明说了这个数字不用，并给出能核对的替代——同一批账户里账户最小的 85% 相对「一直持有不动」的亏损额。

**「1 年想出来几乎不可能」没写。** 这是回本时间的问题，需要按买入点分布算持有期收益，本轮没有找到可引的原始测算，不凭印象写。

## 逐条来源

| URL | 复核 | 原文要点 |
|---|---|---|
| <https://doi.org/10.1111/0022-1082.00072>（Odean T, 1998, The Journal of Finance 53(5):1775-1798；全文 PDF 取自作者主页 faculty.haas.berkeley.edu/odean/Papers current versions/AreInvestorsReluctant.pdf，pdftotext 逐字核对） | 是 | 数据为一家折扣券商 10,000 个账户 1987–1993 年全部交易记录。Table I：全年 PGR = 0.148，PLR = 0.098，差 −0.050，t = −35（13,883 realized gains / 79,658 paper gains / 11,930 realized losses / 110,348 paper losses）。正文：「the ratio of PGR to PLR for the entire year is a little over 1.5, indicating that a stock that is up in value is more than 50 percent more likely to be sold from day to day than a stock that is down」。加仓侧：「For the entire sample PLPA = 0.135 and PGPA = 0.094」，t = 19。后续表现：「For winners that are sold, the average excess return over the following year is 3.4 percent more than it is for losers that are not sold」（超额收益相对 CRSP 市值加权指数）。算例：卖 1000 美元的亏损股而非盈利股，「the investor's return is about 4.4 percent higher over the next year」，其中含提前抵税折现约 10 美元、后续持股收益差 34 美元，边际税率假设 15% |
| <https://doi.org/10.1016/j.jmoneco.2022.01.001>（An L, Lou D, Shi D, 2022, Journal of Monetary Economics 126:134-153）；数字按作者公开工作论文稿逐字核对：<https://personal.lse.ac.uk/loud/AnLouShi.pdf>（2021 年 10 月稿） | 是 | 上交所逐日账户数据，「cover the entire investor population of roughly 40M accounts」，「nearly 90% of the trading volume is contributed by retail accounts」。主样本 2014 年 7 月至 2015 年 12 月共 18 个月，上证综指「climbed more than 150%… to its peak at 5166.35 on June 12th 2015, before crashing 40% by the end of December 2015」。按期初账户市值以 50 万、300 万、1000 万元分四档，最低档占 85%、最高档占 0.5%。结果：「the bottom 85% households lose 250B RMB due to active trading (i.e., relative to a buy-and-hold strategy)… while the top 0.5% gain 254B RMB」；期初持仓市值分别为 880B 和 808B RMB，故「the cumulative loss… amounts to 28% of their initial wealth in equities」、最高档「a gain of 31%」（摘要口径写作 30%）。对照期 2012 年 1 月至 2014 年 6 月，任意 18 个月子期最高档收益「1-3% of the initial equity wealth」。换手：「households churn their positions once every three weeks (or nearly 18 times a year)」 |

## 定级与量级

**两条都定 A。** Odean 1998 给出比例、差值与 t 值，且全文可逐字核对；An-Lou-Shi 用的是交易所全量行政数据，给出绝对金额与占期初市值的百分比。两条都不是荟萃分析，但按项目口径「大型队列 + 可量化数字」够 A。

**来源栏为什么带工作论文链接。** 期刊正式版在 ScienceDirect，本机取不到正文（此前记录已注明 tandfonline/Wiley 一类出版商站点被挡，本轮实测 Wiley 是 Cloudflare 质询、Springer 该 DOI 404）。Crossref 与 Semantic Scholar 都没有这篇的摘要。所以条目里的数字是按作者本人公开的 2021 年 10 月工作论文稿逐字核的，来源栏两个链接都给出，并写明数字按后者核对。正式版摘要把两侧统一写成「30% of either group's initial equity wealth」，工作论文正文分开写 28% 和 31%，条目取后者并同时给出「各约三成」。

**第 37 条收益定「中」。** 金钱口径按金额阈值套：可核对的量是「此后一年高 3.4 个百分点」和算例里的 4.4%，落到十万元级的账户上是数千元一年，属「数百到数千」这一档。没有定「大」，是因为原文没有给出累计金额；第 15 条定「大」是因为那篇给的是年化 6.5 个百分点的长期缺口。

**第 38 条收益定「大」。** 原文给的是「相当于本组期初股票市值的 28%」，十万元级账户对应万元级损失，落在「万元级」这一档。

**毅力都定「些」。** 和同簇的第 15、16 条保持一致：这两条要改的是一个决策习惯，不是每天都要对抗的长期惯性。

## 写法上的三个决定

**第 37 条把「补仓摊平成本」正面承认对了一半。** 直接说「补仓是错的」会被读者当成算术错误反驳（多买确实拉低平均成本）。备注写成「算术上没错，错的是把它当翻身的办法」，再点出它真实的效果是加大单一标的仓位，接到第 19 条上去。

**抵税那一段标明是美国税制。** 4.4% 里含提前实现亏损的抵税收益，这一部分在中国不成立。备注只写「中国不照搬，其余部分仍然成立」，没有去写中国的税制细节——那需要单独引财税文件，不是这条的题目。

**第 38 条的「损失」口径写在正文里。** 原文的 250B 是相对 buy-and-hold 的主动交易损益，不是账面浮亏，两者差别很大。收益栏专门加了一句「这里的『损失』比的是一直持有不动」，否则读者会把它当成「跌掉了 2500 亿」。

## 同步

引用检查基线 545 处，新增 3 处（第 37 条引第 15、19 条，第 38 条引第 15 条），预期 548 处。`tools/sync-stats.ps1` 已跑，README、index.html、tools/og.html 与 og.png 同步。
