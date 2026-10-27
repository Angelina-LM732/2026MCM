# 2026 MCM — Problem B: Creating a Moon Colony Using a Space Elevator System

**Team Control Number:** 2631051
**Paper title:** *Flying to the Moon: the Space Elevator with Rockets — Optimizing Planetary-Scale Transport System*

## Summary

We design an Earth–Moon transport plan for a 100,000-person Moon colony (about 100 million tonnes of material), comparing a space-elevator system, conventional rockets, and a combination of the two.

| Question | Method | Main finding |
|---|---|---|
| Three transport plans | Cost–time bi-objective optimization, Pareto front | Elevator only ≈ 186 years; rockets only ≈ 164 years at far higher cost; the hybrid plan takes **87.1 years and US$18.2 trillion**, with the elevator carrying 46.75% of the mass |
| Non-ideal operation | Repairable series-system availability (MTBF/MTTR) + Monte Carlo (10,000 runs), 3% rocket failure rate | Schedule +28.6%, cost +3.1%; optimal split shifts to 52.3% elevator / 47.7% rockets |
| Water for one year | EOQ-type inventory–resupply optimization at 15 / 30 / 50 L per person per day | Elevator + Apex transfer is always cheaper than ground rockets; resupply about every six months |
| Environmental impact | Cost–time–emissions tri-objective optimization under three policies | Emissions −85% at +15% cost and +17% time |

**My role:** led the modeling team.

> 中文说明见下方。

## 文件 / Files

| 文件 | 说明 |
|---|---|
| [`2631051_Paper.pdf`](2631051_Paper.pdf) | 我们队的完整论文（含摘要页、目录、正文、致 MCM Agency 信件、参考文献、AI 使用报告） |
| 题目原文 | 2026 MCM B 题（© COMAP），见 [COMAP 2026 赛题页面](https://www.contest.comap.com/undergraduate/contests/mcm/contests/2026/problems/) 或 [COMAP 资源页](https://www.comap.com/membership/member-resources/item/creating-a-moon-colony-using-a-space-elevator-system) |

## 题目概要

为一个 10 万人的月球殖民地（2050 年起建，约 1 亿吨建材）设计地月运输方案，比较三种方式：
1. 仅用太空电梯系统（3 个 Galactic Harbour，每年共 179,000 吨/港）
2. 仅用现有地面火箭发射场
3. 两者组合

并分析系统故障影响、殖民地一年用水需求、对地球环境的影响，最后给 MCM Agency 写一页建议信。

## 我们的模型

| 问题 | 方法 | 主要结论 |
|---|---|---|
| 问题 1：三种运输方案 | 成本–时间双目标优化，Pareto 前沿 | 仅电梯约 186 年；仅火箭约 164 年且成本高得多；混合方案约 **87.1 年、18.2 万亿美元**，电梯承担 46.75% 质量 |
| 问题 2：系统非理想运行 | 可修复串联系统可用度（MTBF/MTTR）+ Monte Carlo（10,000 次），火箭失败率 3% | 平均工期 +28.6%，成本 +3.1%；最优分配调整为电梯 52.3% / 火箭 47.7% |
| 问题 3：一年用水 | EOQ 变体的库存–补给优化，人均日用水 15 / 30 / 50 L 三档 | 电梯 + Apex 中转模式年成本始终低于地面火箭；建议约半年补给一次 |
| 问题 4：环境影响 | 成本–时间–碳排放三目标优化；碳税、排放上限、清洁运输优先三种策略 | 排放可降 85%，代价是成本 +15%、工期 +17% |
| 敏感性分析 | 电价/能效/维护系数、火箭单次载荷与成本、单位存储成本 | 能效是电梯成本最敏感的因素 |

**建议：** 采用灵活的多模式运输——太空电梯承担基础运量，火箭用于时间敏感的货物。

## 关键词

Multi-objective optimization · Monte Carlo simulation · Hybrid transport strategy · EOQ · Risk-aware logistics · Carbon-emission minimization
