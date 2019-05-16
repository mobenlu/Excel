[如何从零开始学习Excel，并在工作中熟练运用](https://www.zhihu.com/question/36888983/answer/84860536?from=profile_answer_card)

**Task3**

[Source Excel](https://github.com/mobenlu/Excel/blob/master/DataAnalyst.xlsx)

[REF1](https://zhuanlan.zhihu.com/p/39292027)

**一**
- 用vlookup函数 查找以下公司的 companyId | companyFullName   | |:----| | 上海云贝网络科技有限公司   | | 携程计算机技术（上海）有限公司   | | 浙江康健绿线网络技术有限公司   | | 久亿财富（北京）投资有限公司   | | 杭州木瓜科技有限公司   | | 思特沃克软件技术（成都）有限公司   | | 北京金山云网络技术有限公司   |

=VLOOKUP(A2,DataAnalyst!B1:C6877,2,FALSE)

**二**
- 用match和index函数实现第一题的功能
- (https://zhuanlan.zhihu.com/p/32308992)

=INDEX(DataAnalyst!C2:C6877,MATCH(A2,DataAnalyst!B2:B6877,0))


**三**
- 用match和index函数查找以下id对应的公司名称，注意id是横向排列的| companyId     | 127200   | 151079   | 22225   | |----|----|----|----|

=INDEX(DataAnalyst!B2:B6877,MATCH(B13,DataAnalyst!C2:C6877,0))
=INDEX(DataAnalyst!B2:B6877,MATCH(C13,DataAnalyst!C2:C6877,0))
=INDEX(DataAnalyst!B2:B6877,MATCH(D13,DataAnalyst!C2:C6877,0))

**四**
- 请根据companyId和postionId两个条件查找对应的工资水平| companyId   | positionId   | salary   | |:----|:----|:----| | 62   | 938038   |    | | 1575   | 1157620   |    | | 157392   | 2574696   |    |