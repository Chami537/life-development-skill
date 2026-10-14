# 追加：第 6 节第 31 条，别靠 AI 聊天机器人自己判断病情和法律问题

2026-10-09，issue #103「AI 什么时候不可信」。读者想让书回答三件事：大模型为什么会产生幻觉，怎么靠外部来源核对，重大决定前别盲信 AI 的专业回答。四问：普通读者现在常拿 AI 问病情和法律；AI 回答的语气很肯定，多数人想不到要核；全书原有的 AI 条目只讲中转站（第 11 节第 19 条、第 14 节第 10 条）、AI 造图（第 9 节第 1 条）和服务备案（第 11 节第 17 条），没有「信不信它的回答」这件事；来源是同行评审的随机试验和法学期刊。用户定放第 6 节反面清单。

原理（issue 第 1 点）按全书规矩不展开，只在备注写一句。

## 1. 普通人用 AI 判断病情的随机试验
- 题录：Bean AM 等 (2026). Nature Medicine 32(2):609-615. <https://doi.org/10.1038/s41591-025-04074-y>（PMID 41663592，PMC12920132），全文 XML 经 Europe PMC REST 取得。卷期页码经 Crossref 核对。
- 摘要原文：「We tested whether LLMs can assist members of the public in identifying underlying conditions and choosing a course of action (disposition) in ten medical scenarios in a controlled study with 1,298 participants. Participants were randomly assigned to receive assistance from an LLM (GPT-4o, Llama 3, Command R+) or a source of their choice (control). Tested alone, LLMs complete the scenarios accurately, correctly identifying conditions in 94.9% of cases and disposition in 56.3% on average. However, participants using the same LLMs identified relevant conditions in fewer than 34.5% of cases and disposition in fewer than 44.2%, both no better than the control group.」
- 正文原文：「Participants in the control group had 1.76 (95% CI = 1.45–2.13) times higher odds of identifying a relevant condition than the aggregate of the participants using LLMs. They were also 1.57 (95% CI = 1.28–1.92) times more likely to identify conditions from the more serious 'red flag' list.」
- 正文原文：「Participants using LLMs did not have statistically significant differences in disposition accuracy from the control group」
- 对照组用什么：「Post-treatment surveys indicated that most participants used a search engine or went directly to trusted websites, most often the NHS website」
- 失败原因：「with both users providing LLMs with incomplete information and LLMs suggesting correct answers but not effectively conveying this information to the users」；「Despite these correct suggestions appearing in the conversations, users did not consistently include them in the final responses」
- 每人两个病例：「We assigned each participant two scenarios to complete consecutively.」样本按英国人口结构分层：「stratified to reflect the demographics of the UK」。
- 「AI 单独考试的成绩预测不了普通人用它的效果」：「Standard benchmarks for medical knowledge and simulated patient interactions do not predict the failures we find with human participants.」

## 2. 通用大模型答法律问题
- 题录：Dahl M, Magesh V, Suzgun M, Ho DE (2024). Journal of Legal Analysis 16(1):64-93. <https://doi.org/10.1093/jla/laae003>，摘要经 Crossref 取得。
- 摘要原文：「Using OpenAI's ChatGPT 4 and other public models, we show that LLMs hallucinate at least 58% of the time, struggle to predict their own hallucinations, and often uncritically accept users' incorrect legal assumptions.」幻觉的定义：「textual output that is not consistent with legal facts」。
- 同一篇的 arXiv 版（<https://arxiv.org/abs/2401.01301>，经 arXiv API 取得）摘要写明了题目范围和各模型的数：「legal hallucinations are alarmingly prevalent, occurring between 58% of the time with ChatGPT 4 and 88% with Llama 2, when these models are asked specific, verifiable questions about random federal court cases」。条目「问美国联邦法院的判例」「Llama 2 高到 88%」按这句写。作者单位没逐一核，条目只写「一个美国研究团队」。

## 3. 专业法律 AI 工具
- 题录：Magesh V 等 (2025). Journal of Empirical Legal Studies 22(2):216-242. <https://doi.org/10.1111/jels.12413>，摘要经 Crossref 取得。
- 摘要原文：「the AI research tools made by LexisNexis (Lexis+ AI) and Thomson Reuters (Westlaw AI-Assisted Research and Ask Practical Law AI) each hallucinate between 17% and 33% of the time」；「certain legal research providers have touted methods such as retrieval-augmented generation (RAG) as "eliminating" or "avoid[ing]" hallucinations」

## 4. 幻觉的成因（只进备注）
- 题录：Kalai AT, Nachum O, Vempala SS, Zhang E (2025). Why Language Models Hallucinate. arXiv:2509.04664，经 arXiv API 取得。issue 附的 OpenAI 中文页面对应这篇。未经同行评审，所以只在备注里写一句，不进收益栏。
- 摘要原文：「We argue that language models hallucinate because the training and evaluation procedures reward guessing over acknowledging uncertainty」；「language models are optimized to be good test-takers, and guessing when uncertain improves test performance」

## 5. 反方
- 题录：Ayers JW 等 (2023). JAMA Internal Medicine 183(6):589. <https://doi.org/10.1001/jamainternmed.2023.1838>，摘要经 Europe PMC 取得。
- 摘要原文：「a public and nonidentifiable database of questions from a public social media forum (Reddit's r/AskDocs) was used to randomly draw 195 exchanges」；「evaluators preferred chatbot responses to physician responses in 78.6% (95% CI, 75.0%-81.8%) of the 585 evaluations」
- 它评的是回答的质量和同理心，没看提问的人最后判断对没有，所以和 Bean 2026 不矛盾。备注写明了这一点。

## 没收
- Mata v. Avianca（美国律师用 ChatGPT 编判例被罚）：CourtListener 搜索 API 没检索到这份意见书，原文书没取到，没写。
- 国内普通人用 AI 问病情或法律出错的官方统计和判决，这次没有去查。
- 收益定小：Bean 2026 的终点是「认没认出相关疾病」，属于中间指标，没有死亡或住院的数字。
