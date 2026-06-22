# 0001: SQL从学术到生产 — 窗口函数、JOIN、CTE、Hive差异

**日期**: 2025-06-22

## 学到什么

用户已经具备基础 SQL 能力（数据科学硕士课程覆盖），关键提升点在于三个维度：
1. **窗口函数**：ROW_NUMBER（去重取最新）、DENSE_RANK（连续排名）、LAG/LEAD（环比）是面试最高频考点
2. **生产实践**：LEFT JOIN 的 ON vs WHERE 条件位置差异（退化为 INNER JOIN 的陷阱）、CTE 替代嵌套子查询提升可读性
3. **Hive 差异**：分区表必须带 WHERE dt= 否则全表扫描、collect_list/lateral view explode 等 Hive 独有语法

## 为什么重要

这个 JD 的「业务治理分析」第一要务就是 SQL。面试官通常用一道窗口函数题 + 一道多表 JOIN 题来筛选候选人。Hive SQL 是互联网公司标配，JD 里写「SQL」实际上 70% 指 Hive。用户需要在牛客网上刷完 SQL 实战模块（至少中等难度），才能达到面试要求。

## 下一步

Lesson 2 将进入「业务指标体系」—— 会写 SQL 只是工具，知道查什么、怎么解读才是数据分析师的核心价值。
