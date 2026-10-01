**Sep28, Mon**
- 跑通了20ps的单次模拟->但是没处理好输出，结果被覆盖了。==下次要记得检查输出
- 对`medium, medium-mpa-0, medium-0b3, medium-omat-0`进行了20ps的模拟（20000步），并制作了对比图
- 写了一个续跑脚本，可以分次跑较长的md模拟并分段记录；附带一个融合脚本，将分段的结果合并为一个csv文件
- 以上均已上传到测试库的分支，尚未与main合并。
- 【技术问题】搞定了github的pr审核，以及以后每次pr都要记得写summary- -
---
**Sep29, Tue**
- 一些idea的对齐：burn-in time的概念，对模型性能的系统偏差和显著性分析
- 从（1）显著性（2）时间序列两方面着手对已经取得的四个模型20ps轨迹进行对比分析。(`offset_analysis.py`,`time_sequence_analysis.py`) 结果和昨天的一起在PR#12里。
- 建立workflow board，为融合到大仓库做准备
---
Sep30, Wed
- 开始尝试跑更长步数的、solid的MD结果（20000步），目前进度100ps/200ps
