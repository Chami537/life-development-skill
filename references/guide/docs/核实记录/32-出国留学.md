# 第 32 节 出国留学：身份、打工、保险和回国认证 · 核实记录（2026-09-18）

任务来源：仓库 issue #8 读者问「有没有给常见留学国家留学生的建议，比如美国、加拿大、英国、澳大利亚，身为留学生有什么权益、如何维护」。

原有覆盖：第 21 节写的是出国与境外安全（外交部安全提醒、12308、领事保护边界、境外医疗与转运保险、境外高薪招聘陷阱），不含留学生身份与学业。第 23 节写学历回报，不含境外学历认证。所以新开一节，不与两节重复，正文里做了互相指路。

落点：新增 `book/32-出国留学.md`，10 条。覆盖国家按读者提问限定为美国、加拿大、英国、澳大利亚，逐国写数字。**本节所有外国政策数字标注截至 2026 年 9 月，正文和节首都写明要读者按来源链接自查，不长期维护。**

取源工具：本机 curl 段错误、`Invoke-WebRequest` 对 canada.ca 与 cscse.edu.cn 超时或断连，改用无头 Chrome `--dump-dom` 取渲染后 DOM（jsj.moe.gov.cn 与 immi.homeaffairs.gov.au 是前端渲染，必须走这条路）。全节 17 条外链在 2026-09-18 逐条跑过可达性，除 canada.ca 外均返回 200；canada.ca 本机 PowerShell 取不到但无头 Chrome 可取全文，内容已逐字核对。

## 第 1 条（认证院校名单）

| URL | 复核 | 依据 |
|---|---|---|
| <http://yxcx.cscse.edu.cn/>（留服中心「认证院校查询」入口，从 cscse.edu.cn 首页锚点取得） | 是 | 页面为按国家和院校名检索的查询入口 |
| <https://jsj.moe.gov.cn/>（教育部教育涉外监管信息网首页） | 是 | 栏目含文件政策、预警信息、合作办学 |
| <http://rzzccx.crs.jsj.edu.cn/>（中外合作办学证书认证注册信息查询） | 是 | 「自 2008 年入学就读的学生，可凭本人姓名、身份证号码查询境外学历学位证书认证注册序号」 |

定级 A：查询入口和制度安排均可在官方页面逐字核对。收益量级「大」——金钱口径按万元级定档，学费与一到两年时间的量级远超万元。备注里「名单会变、每年复查」是操作建议，非文件原文。

## 第 2 条（美国固定入境期限与 30 天离境窗口）

| URL | 复核 | 原文要点 |
|---|---|---|
| <https://www.ecfr.gov/current/title-8/chapter-I/subchapter-B/part-214/section-214.2>（eCFR 现行文本 8 CFR 214.2(f)） | 是 | 完成学业与已获批实习的 F-1，自项目结束日期、四年最长入境期限或 OPT/STEM OPT 许可结束日起「an additional 30-day period」用于准备离境或另求合法身份；提前结束学业或培训的，自结束之日起 30 日内离境或另求合法身份 |
| <https://www.federalregister.gov/documents/2026/07/17/2026-14439/establishing-a-fixed-time-period-of-admission-and-an-extension-of-stay-procedure-for-nonimmigrant>（联邦公报最终规则） | 是 | publication_date 2026-07-17，effective_on 2026-09-15（经 federalregister.gov API 取字段核对） |

**2026-09-25 更正（issue #32）**：这项规则**没有**在 2026-09-15 生效。2026-09-14，马萨诸塞州联邦地区法院 Saylor 法官在 Presidents' Alliance on Higher Education and Immigration v. DHS（No. 1:26-cv-13799-FDS）一案中，依 5 U.S.C. § 705 推迟了整份规则的生效，效力及于全国；撤销（vacatur）与简易判决请求被驳回、允许再提。条目已据此改写为「新规被暂停，眼下仍是 D/S 与 60 天宽限期」。

| URL | 复核 | 原文要点 |
|---|---|---|
| <https://oiss.yale.edu/news/important-update-court-action-on-the-ds-rule>（耶鲁国际学生学者办公室，2026-09-14） | 是 | 「issued an order preliminarily enjoining DHS from implementing this rule」「the current D/S framework remains in place for now」「You do not currently need to apply for an Extension of Stay」「The administration may appeal」 |
| <https://www.aila.org/blog/think-immigration-one-day-before-taking-effect-federal-court-postpones-the-f-j-and-i-fixed-admission-period-rule>（美国移民律师协会） | 是 | 「The relief is nationwide, and it reaches the whole rule」「The rule is postponed, not vacated」「the 60-day grace period stands, and there is no new I-539 requirement」「denying the vacatur and summary judgment requests without prejudice to renewal」「the government may seek review in the First Circuit」 |
| <https://www.courtlistener.com/docket/74661796/presidents-alliance-on-higher-education-and-immigration-v-united-states/>（法院案卷） | 是 | 第 50 号（2026-09-14）MEMORANDUM AND ORDER：「GRANTED to the extent that it seeks to postpone the effective date of the Final Rule pursuant to … 5 U.S.C. § 705. To the extent that plaintiffs seek vacatur of the Final Rule, summary judgment, or other relief, the motion is DENIED without prejudice to its renewal」；第 51 号（2026-09-14）「PRELIMINARY INJUNCTION ORDER POSTPONING EFFECTIVE DATE OF FINAL RULE」；同日通知「Status Conference set for 10/2/2026 12:00 PM」。直连 403，走本地代理可取 |

原定级说明（下文）保留作历史记录，其中「2026-09-15 起已被固定期限规则取代」一句已不成立。

定级 A：条文与生效日期均可逐字核对。**这条是本节最要紧的更新**：eCFR 现行文本写的是 30 天，网上通行的「60 天宽限期」与「duration of status 读到毕业」均为旧制，2026-09-15 起已被固定期限规则取代，距本次写作仅三天。收益量级「大」——自由口径，后果是非法滞留与遣返，按「避免刑责 大」一档类推。延期程序在 (f)(7)，正文只指路未展开。

## 第 3 条（四国打工时数）

| URL | 复核 | 原文要点 |
|---|---|---|
| <https://www.ecfr.gov/current/title-8/chapter-I/subchapter-B/part-214/section-214.2>（8 CFR 214.2(f)(9)） | 是 | 校内就业「must not exceed 20 hours a week while school is in session」；经批准的校外兼职「limited to no more than 20 hours a week when school is in session」，假期可全职 |
| <https://www.gov.uk/guidance/immigration-rules/immigration-rules-appendix-student>（移民规则附录 Student，ST26.1 表） | 是 | 学位及以上且保荐方合规：学期内每周 20 小时；学位以下：10 小时；其余含全部非全日制：不得就业。ST26.5 另禁自雇、职业运动员与教练、演艺 |
| <https://www.canada.ca/en/immigration-refugees-citizenship/services/study-canada/work/work-off-campus.html>（IRCC） | 是 | 「You can work up to 24 hours per week」；旧许可印 20 小时的，符合条件仍可做到 24 小时；依据为 IRPR 第 186(v) 条 |
| <https://immi.homeaffairs.gov.au/visas/getting-a-visa/visa-listing/student-500>（内政部 Student visa 500） | 是 | 「work up to 48 hours a fortnight when your course of study or training is in session」，研究型硕士与博士及家属无工时上限 |

定级 A：四国均为移民主管部门现行页面或成文规则，数字逐字可核。收益量级「大」——自由口径，超时属违反签证条件，可致签证取消与遣返。

## 第 4 条（全日制在读是打工资格的根）

| URL | 复核 | 原文要点 |
|---|---|---|
| <https://www.canada.ca/en/immigration-refugees-citizenship/services/study-canada/work/work-off-campus.html> | 是 | 获批休学期间，或转学期间未在学习的，不得校外打工，恢复学业后方可复工 |
| <https://studyinthestates.dhs.gov/students/work/working-in-the-united-states>（DHS Study in the States） | 是 | 校内就业以 SEVIS 中状态为 Active 的 F-1 学生为限；校外就业须先获批，I-765 审理期间不得开工 |
| <https://www.gov.uk/guidance/immigration-rules/immigration-rules-appendix-student>（ST26.1） | 是 | 打工许可按课程类型授予，非全日制课程不得就业 |

定级 A。加拿大页面表述最明确，美英两国以各自规则佐证。收益量级「大」，理由同第 3 条。

## 第 5 条（美国地址变更 10 日内报备）

| URL | 复核 | 原文要点 |
|---|---|---|
| <https://www.ecfr.gov/current/title-8/chapter-I/subchapter-B/part-265/section-265.1> | 是 | 负有登记义务者须「within 10 days of such change」按 USCIS 要求报告地址变更与新地址 |
| <https://www.uscis.gov/ar-11> | 是 | AR-11 表格页，说明须尽快通知地址变更以免错收文书 |

定级 A：10 日期限为条文明文。收益量级「中」——自由口径按「避免行政处罚」一档，且错收文书的实际后果多为程序性不利，未到刑责一级。

## 第 6 条（教育部留学预警）

| URL | 复核 | 原文要点 |
|---|---|---|
| <https://jsj.moe.gov.cn/n2/2/2/2001.shtml> | 是 | 2025 年第 1 号（2025-04-09），美国有关州高等教育法案含涉华消极条款 |
| <https://jsj.moe.gov.cn/n2/2/2/2030.shtml> | 是 | 第 2 号（2025-07-18），菲律宾治安不靖、针对中国公民犯罪多发 |
| <https://jsj.moe.gov.cn/n2/2/2/2035.shtml> | 是 | 第 3 号（2025-08-30），再次提示菲律宾 |
| <https://jsj.moe.gov.cn/n2/2/2/2060.shtml> | 是 | 第 4 号（2025-11-16），日本治安形势与留学环境不佳，建议谨慎规划赴日留学 |

定级 A：四份预警的编号、日期、指向国家均逐条核对。正文来源栏只列第 4 号与第 1 号加栏目首页，避免来源行过长。收益量级「中」——预警是风险提示不是禁令，不直接对应可量化后果。**预警名单随形势变动，本节按 CLAUDE.md 第 21 节同一惯例，不长期维护。**

## 第 7 条（澳大利亚 OSHC）

| URL | 复核 | 原文要点 |
|---|---|---|
| <https://immi.homeaffairs.gov.au/visas/getting-a-visa/visa-listing/student-500> | 是 | 须持有并全程维持 OSHC，除非属豁免情形；与前一签证的保险之间不得有空档；入境时无法证明已投保者可能被拒绝入境；先于课程开始入境的，保险起始日为抵澳之日 |

定级 A。收益量级「中」——金钱口径，保费为数千到上万元级，属「数百到数千」与万元级交界，取中。成本标签钱=多（按签证年限一次性支出）。

## 第 8 条（英国签证费与医疗附加费）

| URL | 复核 | 原文要点 |
|---|---|---|
| <https://www.gov.uk/student-visa> | 是 | 境外申请与境内延期或转换均为 £558；年满 18 岁读学位及以上通常最长停留 5 年，学位以下 2 年 |
| <https://www.gov.uk/healthcare-immigration-application> | 是 | 学生及其家属每年 £776（2 年签证即 £1,552），其他申请人每年 £1,035；超过 6 个月不足 1 年按整年收取 |

定级 A：金额逐字取自 gov.uk 当期页面。收益量级「中」——金钱口径，两项合计为数千元人民币量级。正文未换算人民币具体数额，只写「按当前汇率一万几千元」的量级，避免汇率变动导致数字失效。

## 第 9 条（留服认证时限）

| URL | 复核 | 原文要点 |
|---|---|---|
| <http://zwfw.cscse.edu.cn/>（留服中心网上服务大厅） | 是 | 学历学位认证流程为注册实名认证、提交申请与材料、在线缴费、评估与审核；「认证工作时限 10-20 个工作日」；申请材料含文凭证书、护照或通行证、居留卡或签证签注、证件照片、授权声明；出入境记录由系统取 |

定级 A：时限与材料清单为页面明示。收益量级「中」、口径时间——节省的是错过截止日期的风险，不是每天的时间，按「一次性」本应定小，但错过秋招或考公报名的后果按窗口期计，取中；此处为判断，非机械套阈值，依 CLAUDE.md 要求在此写明。

## 第 10 条（加强认证审查名单）

| URL | 复核 | 原文要点 |
|---|---|---|
| <https://www.cscse.edu.cn/cscse/sy/tzgg/2025102809225023345/index.html> | 是 | 《关于对部分国外院校学历学位认证加强认证审查的公告（九）》，2025-10-28 发布 |
| <https://www.cscse.edu.cn/> | 是 | 通知公告栏同时列有「关于谨防借国（境）外学历学位认证实施诈骗的重要提示」「关于对部分国（境）外学历学位认证书失效处置的公告」「关于暂停泰国彭世洛大学学历学位认证申请的公告」 |

定级 A：公告标题、期号与日期可逐字核对。收益量级「中」——金钱口径，后果是认证受阻或延迟，未必全额损失学费，故不取大。正文未点名任何具体院校（除引用公告标题中已公开的一所），避免名单变动后失准。

## 本节没写的

- 各国的税务申报义务（如美国 F-1 无收入也需报送表格）本轮未取得可逐字核对的官方页面，未写入。
- 加拿大、英国、澳大利亚的地址变更报备期限各不相同，未逐国取原文，第 5 条只写美国并在备注里提示其余三国另按本国规定办。
- 学生签证被拒或身份失效后的补救程序（美国的 reinstatement 等）未写，属专门程序，超出本节「不知道就吃亏」的定位。
- 日本、新西兰、新加坡等其他留学目的国不在读者提问范围内，未纳入。
