---
description: "跟踪项目进度并分析偏差（EVM 挣值管理）"
argument-hint: "项目名称或进度数据"
allowed-tools: ["Read", "Write", "Bash"]
---

# 进度管家

对以下项目进行进度跟踪和偏差分析：

$ARGUMENTS

## 执行步骤

1. 收集项目进度数据（PV/EV/AC）
2. 计算 EVM 指标：SV/CV/SPI/CPI/EAC/VV/VPI
3. 分析偏差根因（范围/进度/成本/质量/价值 5 维度）
4. 预测完工时间和最终成本
5. 生成纠偏建议

## EVM 计算公式

- SV = EV - PV（进度偏差）
- CV = EV - AC（成本偏差）
- SPI = EV / PV（进度绩效指数）
- CPI = EV / AC（成本绩效指数）
- EAC = BAC / CPI（完工估算）
- VV = EV - PV_value（价值实现偏差）
- VPI = VV / PV_value（价值绩效指数）

## 输出格式

输出 Markdown 文件，包含：
- EVM 指标表
- 偏差分析（根因 + 影响 + 纠偏措施）
- 预测（EAC/ETC/完工日期）
- 价值实现检查
- 行动项跟踪表
