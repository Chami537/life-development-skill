# issue #28：八处条目补来源（2026-09-23）

任务来源：GitHub issue #28（dlgrv），提议给 8 处标着「作者经验」「待核实」「TODO」的条目补原始文献，每条附了引文和链接。issue 里的引文只当线索，下表每一条都是本轮自己抓原文逐字核的。

## 逐条核对与处理

| 条目 | 来源 | 复核 | 原文要点 | 处理 |
|---|---|---|---|---|
| 第 13 节第 18 条（触电） | <https://www.cdc.gov/natural-disasters/response/what-to-do-protect-yourself-from-electrical-hazards.html> | 是（curl 403，无头 Chrome 取得） | First aid 一节：「Look first. Don't touch. The person may still be in contact with the electrical source.」「Turn off the source of electricity if possible. If not, move the source away from you and the affected person using a non-conducting object made of cardboard, plastic or wood.」「If either has stopped or seems dangerously slow or shallow, begin cardiopulmonary resuscitation (CPR) immediately.」 | 采纳 |
| 同上 | <https://doi.org/10.7326/0003-4819-145-7-200610030-00011>（Spies & Trohman 2006） | 是（Europe PMC 摘要） | 「patients successfully resuscitated after cardiopulmonary arrest often have a favorable prognosis」 | 采纳 |
| 同上 | Moran 1986 JAMA（10.1001/jama.1986.03370160055007） | 否 | Europe PMC 无摘要，内容核不了 | 不采纳 |
| 同上 | ERC 2021 特殊情况心脏骤停（10.1016/j.resuscitation.2021.02.011） | 是（摘要） | 摘要列出的特殊原因、场景和人群里都没有触电，issue 说「2021 版无触电章节」属实 | 从来源栏删掉；原来源栏说它「含触电章节」是错的 |
| 第 20 节第 9 条（不摇晃婴儿） | <https://doi.org/10.15585/mmwr.mm6520a1>（MMWR 2016） | 是（摘要） | 「During this period, AHT resulted in nearly 2,250 deaths among U.S. resident children aged <5 years」 | 采纳 |
| 同上 | <https://doi.org/10.1007/s00247-018-4149-1>（Choudhary 2018 共识声明） | 是（摘要） | 「Abusive head trauma (AHT) is the leading cause of fatal head injuries in children younger than 2 years」；病因「multifactorial (shaking, shaking and impact, impact, etc.)」；「subdural hematoma… complex retinal hemorrhages」 | 采纳 |
| 同上 | AAP 背书版（10.1542/peds.2018-1504） | 未核 | 和共识声明是同一内容的背书，不另加 | 不采纳 |
| 第 13 节第 27 条（无人区） | <https://www.nps.gov/articles/000/desertdrivingsafety.htm> | 是（curl 直取） | 「Staying with your car is the most important thing you can do in the event of an emergency. While not often, people have died from exposure trying to walk back to the paved roads.」 | 采纳，等级不变 |
| 第 4 节第 15 条（刷屏上限） | CNNIC 第 56 次报告 PDF | 是（pdftotext 可逐字抽中文） | 第 821 行「截至 2025 年 6 月，我国网民的人均每周上网时长为 30.6 个小时，较 2024 年 12 月提升 1.9 个小时」；第 94 行「短视频用户规模达 10.68 亿人，占网民整体的 95.1%」 | 采纳，TODO 移除 |
| 第 5 节第 17 条（指数基金） | SPIVA U.S. Scorecard Year-End 2024 | 是（官网 403 且无头 Chrome 被拒，按 Wayback 2025-05-12 快照核） | 「65% of all active large-cap U.S. equity funds underperformed the S&P 500, worse than the 60% rate observed in 2023 and slightly above the 64% average annual rate reported over the 24-year history」；「Over the 15-year period ending December 2024, there were no categories in which a majority of active managers outperformed.」 | 采纳，TODO 移除。条目缺的是「长期」数字，所以除了 issue 引的单年 65%，另加 24 年均值和 15 年的结论 |
| 同上 | SPIVA Institutional Scorecard Year-End 2024 PDF | 未用 | 机构账户和 wrap 账户，普通读者买不到这类产品 | 不采纳 |
| 第 14 节第 2 条（邮箱密码） | <https://www.cisa.gov/secure-our-world/use-strong-passwords> | 是（curl 直取） | 「Create long, random, unique passwords with a password manager」；「At least 16 characters—longer is stronger!」；「Use a different strong password for each account」 | 采纳，等级不变 |
| 第 14 节第 3 条（SIM 卡 PIN） | FCC DOC-398483A1（2023-11-15 新闻稿） | 是（pdftotext） | 管的是运营商在转号、换卡前核验身份，针对的是「without ever gaining physical control of a consumer's phone」的换卡诈骗 | **不采纳**。条目防的是手机丢了、卡被拔下来插进别的手机，这正好是对方拿到了实体卡的情形，两件事不是一回事 |
| 第 14 节第 4 条（手机丢了） | <https://www.fcc.gov/consumers/guides/protect-your-mobile-device> | 是（curl 403，无头 Chrome 取得） | 「Even if you think you may have only lost the device, you should remotely lock it to be safe. If the device was stolen, immediately report the theft to the police, including the make and model, serial and IMEI or MEID or ESN number.」「Immediately report the theft or loss to your service provider.」 | 采纳；步骤先后顺序仍是作者经验，来源栏写明 |

## 定级

**只有两条改了等级：第 13 节第 18 条和第 20 节第 9 条，都是 C 升 B。** 两条现在都有官方指南或专业共识，另有一篇研究支撑，但都没有能直接换算成「做了少死多少」的数字，按口径是 B。

其余几条等级不变。官方机构的操作提示（NPS、CISA、FCC）不是研究，按本书惯例仍定 C（第 13 节第 27 条一直就是这个处理）。第 4、5 节两条只是移除 TODO、补上数字，等级不动。

## 没照 issue 做的地方

- 翻译本身不合入本仓库（CLAUDE.md 规则），这次只处理对中文原文的来源建议。
- issue 提议可以直接开 PR。本轮已经在本地改完，不需要 PR。
