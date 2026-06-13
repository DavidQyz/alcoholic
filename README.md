# 酒饮记录项目 · Alcohol Tasting Journal

这个项目用于系统记录和整理我所有喝过的酒——分类体系、品评笔记、探店记录。

目标：建立一套自己的品评语言，而不仅仅是"好喝"或"不好喝"。

---

## 当前进度

- [x] 清酒（日本酒）— 体系已建立，17条品饮记录（2025-08 大阪·京都·和歌山行），东京行程记录待补
- [x] 葡萄酒 — 体系建立中（WSET Level 3 方向），首批记录来自斯洛文尼亚 & 意大利北部（11款）
- [x] 咖啡 — 品鉴表单与产区概览已建（非酒类的附加品类）
- [~] 威士忌 — 架子已建，**以记录为主**（轻品评，无系统品饮体系）
- [ ] 鸡尾酒探店

---

## 目录结构

```
sake/
  sake-primer.md       # 清酒基础知识与分类体系
  brewing/             # 酿造工艺笔记（01原料処理 ~ 06後処理）
  brewing-moto.md      # 酒母专题
  regional-impressions.md  # 产地印象
  venues.md            # 探访过的酒吧/酒厂列表
  templates/           # 清酒品评模板
  records/             # 清酒品鉴记录，按 都道府県/蔵元/ 组织
wine/
  wine-primer.md       # 葡萄酒基础知识（WSET Level 3 方向）
  varieties/           # 品种卡片（red/ + white/）
  study/               # WSET3 教材学习笔记（11章）
  templates/           # 品评模板、产区概览模板
  records/             # 葡萄酒品鉴记录，按 产国/产区/ 组织（含产区概览）
  WSET3-*.pdf/xlsx/docx  # 教材原文
whisky/
  whisky-primer.md     # 产区/类型对照（以记录为主，轻参考）
  templates/           # 轻品评模板、产区概览模板
  records/             # 威士忌记录，按 产国/产区/酒厂 组织
coffee/
  templates/           # 咖啡品鉴表单（md/html/pdf/xlsx）与产区概览
docs/
  tasting-templates/   # 鸡尾酒探店模板等
  *.py / *-form.*      # 品鉴表单生成脚本与产物
project_management/
  WORKLOG.md           # 工作日志（AgentOS 会话连续性）
  agentos_lesson_candidates.md  # 可泛化工作流经验候选
CLAUDE.md              # 给Claude的项目记忆文件（顶层规则）
```

---

## 品评记录格式

每款酒一个 `.md` 文件：

- **清酒**：放在 `sake/records/都道府県/蔵元名/` 下，文件名 `评分_YYYY-MM_蔵元名_酒款名.md`
  （日期精确到日时用 `YYYY-MM-DD`；蔵元文件夹内可另建 `蔵元紹介.md`）
  例：`★★★_2025-08_吉村秀雄商店_車坂-山廃.md`
- **葡萄酒**：放在 `wine/records/产国/产区/` 下，文件名 `类型-YYYY-酒庄-酒款名.md`
  （类型：红 / 白 / 橙 / 白浸皮等；每个产区另建 `产区概览.md`）
  例：`红-2025-Ausonia-Montepulciano.md`
- **威士忌**：放在 `whisky/records/产国/产区/酒厂/` 下，文件名 `评分_YYYY_酒厂_酒款名.md`
  （以记录为主、轻品评；产区概念弱的产国中间一级可用产国名占位）
  例：`★★★_2018_Lagavulin_16年.md`

---

## 评分说明

本项目不使用100分制。用三个维度的简单标记：

| 符号 | 含义 |
|------|------|
| ★★★ | 印象深刻，会主动再找来喝 |
| ★★  | 好喝，场合合适会点 |
| ★   | 普通或不符合个人口味 |
| —   | 信息记录为主，无评价 |

---

## 品评语言参考

- 清酒：参见 `sake/sake-primer.md`（基于SAKE DIPLOMA / SSI唎酒師体系）
- 葡萄酒：参见 `wine/wine-primer.md`、`wine/varieties/` 与 `wine/study/`（基于WSET Level 3 SAT体系）
- 威士忌：参见 `whisky/whisky-primer.md`（产区/类型对照，以记录为主，无系统品评体系）

---

## 相关行程

- 2025-06 东京四日（个人行）— 澤乃井酒造见学、和幻十四代飲み比べ、原価酒蔵新政の日
- 2025-06 东京四日（家庭行）— 石川酒造见学、原価酒蔵
- 2025 斯洛文尼亚 & 意大利北部 — 橙酒、Brda 自然酒、Barolo 初探（11款）
