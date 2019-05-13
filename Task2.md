[如何从零开始学习Excel，并在工作中熟练运用](https://www.zhihu.com/question/36888983/answer/84860536?from=profile_answer_card)

[Task2](https://github.com/mobenlu/Excel/edit/master/DataAnalyst.xlsx)

**任务一**
- 1.1将列salary最低工资提取出来，假如单元格为“10k以上”、“8k以下”等，最低工资直接为10和8。
[EXCEL中字符串提取函数](http://blog.sina.com.cn/s/blog_818b22e50102vte6.html)

=MID($P3,1,FIND("k",$P3,1)-1)


- 1.2 计算北京最低工资的平均值？
- 1.3 最低工资平均值最低的城市是哪一个？
- 1.4 北京本科的招聘中，最低工资介于7-11（大于7小于11）的岗位有多少个？

**任务二** 
- 将职位标签（positionLables）中，包含“大数据”的岗位筛选出来。

**任务三** 
- 将最低工资分段，（0,4]为低，（4,8]为中，8以上为高。
