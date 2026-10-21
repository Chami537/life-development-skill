# 追加：第 32 节第 11、12 条，美国 OPT 失业天数上限、加拿大省级证明信

2026-10-14。两条都追加在第 32 节末尾，没有插在中间。本节不到 20 条，不需要节首导览。查重：全书 grep「OPT」「PAL」「省级证明信」「STEM」都没有命中。

四问：① 去美国、加拿大读书的读者会碰上；② OPT 失业天数是会丢身份的硬线，很多人只知道「有 OPT 可以找工作」，不知道没工作的天数有上限；加拿大 2026 年起硕士博士豁免是新变化，被拒后要重拿证明信也少有人知道；③ 动作是新的（记天数、毕业前递申请；拿信前问清退学费）；④ 有官方原文。

## 第 11 条：OPT 失业天数

### 1. 8 CFR 214.2(f)(10)(ii)(E)
- URL：<https://www.ecfr.gov/current/title-8/chapter-I/subchapter-B/part-214/section-214.2>；本次用 eCFR 版本接口取 2026-10-09 版全文（`/api/versioner/v1/full/2026-10-09/title-8.xml?part=214&section=214.2`，要带代理和 `--compressed`）。
- 原文：「(E) Periods of unemployment during post-completion OPT. During post-completion OPT, F-1 status is dependent upon employment. Students may not accrue an aggregate of more than 90 days of unemployment during any post-completion OPT period described in 8 CFR 274a.12(c)(3)(i)(B). Students granted a 24-month OPT extension under paragraph (f)(10)(ii)(C)(2) of this section may not accrue an aggregate of more than 150 days of unemployment during a total OPT period, including any post-completion OPT period described in 8 CFR 274a.12(c)(3)(i)(B) and any subsequent 24-month extension period.」
- 2026-09-01 版和 2026-10-09 版这一段逐字相同，固定入境期限新规没动它。

### 2. 申请时间：60 天还是 30 天
- 2026-09-14 版 (f)(11)(i)(B)(2)：「the student may properly file his or her Form I-765 or successor form up to 90 days prior to his or her program end date and no later than 60 days after his or her program end date. The student must also file his or her Form I-765 or successor form with USCIS within 30 days of the date the DSO enters the recommendation for OPT into his or her SEVIS record.」
- 2026-09-15 版起同一句变成「no later than 30 days after his or her program end date」。eCFR 版本列表显示 214.2 在 2026-09-15 有一次实质修改，对应 2026-07-17 公布、原定 2026-09-15 生效的固定入境期限规则（第 32 节第 2 条）。eCFR 不反映法院暂停，所以网站「current」页现在显示 30 天。
- 法院暂停期间按旧规矩，USCIS 页面仍写 60 天：<https://www.uscis.gov/working-in-the-united-states/students-and-exchange-visitors/optional-practical-training-opt-for-f-1-students>（2026-10-14 取）——「Initial post-completion OPT … Must apply within 30 days after your DSO enters the recommendation for OPT into your SEVIS record, and May apply up to 90 days before you complete your degree, but no later than 60 days after you complete your degree.」
- 所以条目写 60 天，备注提示新规会改成 30 天，建议毕业前就递。

### 3. SEVP 说明：没登记雇主算失业、可被手动终止
- URL：<https://studyinthestates.dhs.gov/sevis-help-hub/student-records/fm-student-employment/f-1-optional-practical-training-opt>（2026-10-14 带代理取到）
- 原文：「While students are not required to have an employer when OPT is requested in SEVIS, students authorized for post-completion OPT are expected to be employed. A student on post-completion OPT can be unemployed for a total of 90 days. A student whose record lacks employer information is considered unemployed. SEVP officials can manually terminate a student who accrues 90 total days of unemployment.」

### 4. OPT 收费提议
- Federal Register API 取 2026-20660 号文件摘要：「This rule proposes new fees for Optional Practical Training (OPT) … $70,000 for initial OPT; and $30,000 for any subsequent OPT.」类型 Proposed Rule，2026-10-08 公布，comments_close_on 2026-11-09。
- URL：<https://www.federalregister.gov/documents/2026/10/08/2026-20660/optional-practical-training-fees>
- 只是提议，条目备注写明没有生效。

### 等级与量级
- 证据等级 A：联邦法规原文加官方说明。
- 收益大、口径自由：超限的后果是 F-1 身份被终止，和本节第 3、4 条（违反签证条件、身份断掉）同一量级，沿用本节标法。

## 第 12 条：加拿大省级证明信（PAL/TAL）

### 1. IRCC，Provincial attestation letter or territorial attestation letter
- URL：<https://www.canada.ca/en/immigration-refugees-citizenship/services/study-canada/study-permit/get-documents/provincial-attestation-letter.html>（curl 超时，无头 Chrome 带代理取到；页面 dcterms.modified 为 2026-09-02）
- 是什么：「The provincial attestation letter or territorial attestation letter (PAL/TAL) is a letter from the province or territory where you plan to study that confirms there's space for you provided by the designated learning institution (DLI) you plan to attend usually required to apply for a study permit」；「It confirms that you've been assigned one of the available spaces to study in that province or territory.」
- 怎么拿、何时交：「You should contact your school (DLI) to find out how to apply for a PAL/TAL.」；「You should submit a PAL/TAL with your study permit application, not after」
- 豁免（节选）：「preschool primary school (including kindergarten) secondary school (up to grade 12) degree-granting graduate program at the master's or doctoral level at a public DLI starting January 1, 2026」；「You're an exchange student studying under an exchange arrangement between your home institution and a DLI in Canada, and you don't pay tuition fees to the DLI.」；「You're applying for a study permit extension at the same DLI and level of study as your current study permit.」；「You need to provide proof that you meet one of the above exceptions if you don't provide a PAL/TAL with your study permit application.」
- 魁北克：「If you want to study in Quebec, you need an attestation of issuance of your Quebec Acceptance Certificate (CAQ), which is issued by the Government of Quebec.」
- 有效期：「until December 31, 2026, for the 2026 study permit cap year」；「Your PAL/TAL needs to be valid when you apply for your study permit. It does not need to be valid when you start your studies.」
- 重新拿：「You can't reapply with the same PAL/TAL if your study permit application was approved or refused.」；「As of January 22, 2025, you must get a new PAL/TAL before you submit your study permit application when changing schools.」

### 2. IRCC，Study permit: Get the right documents
- URL：<https://www.canada.ca/en/immigration-refugees-citizenship/services/study-canada/study-permit/get-documents.html>（无头 Chrome 带代理取到；dcterms.modified 2026-10-06）
- 原文：「Get a provincial or territorial attestation letter (PAL/TAL) from your school. In most cases, you need to accept your offer and pay your tuition fees, either in part or in full, to get your PAL/TAL.」

### 等级与量级
- 证据等级 A：移民局官网原文。
- 收益中、口径金钱，凭判断：没交证明信或拿旧信再申请，损失的是申请费、时间和可能退不全的学费，后果是钱和时间，不涉及人身自由。官网没有给出被拒时学费退多少的统一规定，所以条目只让读者问学校，没写数字。
- 没写「没有证明信会被退件」：这一说法在两页原文里没有逐字找到。
