# 阵列优配 Precision Array

阵列优配是一个用于长方体工件自动排列的网页工具。它面向存在加工公差、尺寸微小差异和侧面倾斜的工件，帮助用户在给定 L/W/H 阵列数量和成品公差范围后，计算每一块工件更适合放在哪个位置、采用哪种翻转方向。

## 网站能做什么

- 输入 L、W、H 三个方向的排列数量。
- 输入单个工件的名义尺寸、公差和成品允许公差。
- 手动填写或导入每块工件的实测数据。
- 按预计时间、计算次数或完整枚举进行优化计算。
- 输出推荐排列方案，并用三维位置模型标出每个工件的位置。
- 提供让位逻辑演示，解释相邻工件接触面倾斜时为什么可能需要避让。
- 支持直接下载 Excel 数据模板。

## 适用场景

这个工具适合用于长方体工件的组合装配、叠放、阵列排列和尺寸风险评估。  
当每块工件虽然都在公差范围内，但实际长宽高、侧面倾斜或局部读数存在差异时，可以用它辅助寻找更合理的排列方式。

## 如何使用

打开网站首页 `index.html`，按页面顺序填写：

1. 组合数量：L 数量、W 数量、H 数量。
2. 单件尺寸：单个工件的 L/W/H 名义尺寸和单件上下偏差。
3. 成品公差：最终组合后整体 L/W/H 允许的上下偏差。
4. 工件实测数据：可手动输入，也可以下载模板后导入 Excel。
5. 选择重点方向和计算方式。
6. 点击“计算”，查看推荐排列结果。

如果想理解接触面倾斜导致的让位逻辑，可以点击首页中的“打开让位逻辑演示”。

## 文件说明

- `index.html`：主网站页面，包含核心界面、样式、计算逻辑和模板下载。
- `logic.html`：让位逻辑演示页面，用动画解释相邻工件的接触面避让逻辑。
- `README.md`：项目说明文件。

## 当前限制

- 当前版本主要考虑长方体工件。
- 计算结果用于辅助排列决策，实际装配仍需结合现场工艺、胶层、夹具和测量方式判断。
- 让位逻辑演示用于解释算法思想，不等同于完整有限元或真实接触仿真。

## Project Summary

Precision Array is a browser-based tool for optimizing the arrangement of rectangular workpieces with real-world dimensional tolerances. It helps users evaluate measured L/W/H data, side inclination readings, product tolerance limits, and recommended placement/orientation for each block in an L/W/H array.
