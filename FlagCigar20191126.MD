Question 1-5： BAM FLAG
1. Explain BAM FLAG value： 143
    read paired (0x1)—— read序列为双端测序
    read mapped in proper pair (0x2)—— read测序结果与模板序列相匹配
    read unmapped (0x4)—— read序列没有与模板序列相匹配
    mate unmapped (0x8)——next read 序列没有与模板相匹配
    second in pair (0x80)——代表read 序列读取的第二段或者是最后一段序列 

2. Explain BAM FLAG value： 99
    read paired (0x1)—— read序列为双端测序
    read mapped in proper pair (0x2)——read测序结果与模板序列相匹配
    mate reverse strand (0x20)——read 序列与模板的互补序列相匹配
    first in pair (0x40)——代表read 序列读取的第一段序列

3. Explain BAM FLAG value：516
    read unmapped (0x4)——read序列没有与模板序列相匹配
    read fails platform/vendor quality checks (0x200)——read 序列没有通过质量检测

4. Explain BAM FLAG value： 2064
    read reverse strand (0x10)——第一个read序列的反向序列
    supplementary alignment (0x800)——代表read序列对应的比对线是嵌合比对的一部分

5. Explain BAM FLAG value： 147
    read paired (0x1)—— read序列为双端测序
    read mapped in proper pair (0x2)—— read测序结果与模板序列相匹配
    read reverse strand (0x10)——第一个read序列的反向序列
    second in pair (0x80)——代表read 序列读取的第二段或者是最后一段序列 
Question 6-10： BAM CIGAR
6. Explain BAM CIGAR：14M2D31M
14M：测序序列的14个碱基与模板匹配
2D：测序序列有两个碱基缺失
31M：测序序列的31个碱基与模板匹配
7. Explain BAM CIGAR：3S6M1D5M
3S：测序序列有三段和模板匹配
6M：测序序列的6个碱基与模板匹配
1D：测序序列有1个碱基缺失
5M：测序序列的5个碱基与模板匹配
8. Explain BAM CIGAR: 6M14N5M
6M：测序序列的6个碱基与模板匹配
14N：测序序列有14个碱基的跳跃
5M：测序序列的5个碱基与模板匹配
9. Explain BAM CIGAR: 7M5D8M2I14M  (小写：7m5d8m2i14m）
7M：测序序列的7个碱基与模板匹配
5D：测序序列有5个碱基缺失
8M：测序序列的8个碱基与模板匹配
2I：测序序列有2个碱基的插入
4M ：测序序列的4个碱基与模板匹配
10. how long is the read with alignment CIGAR of 7M5D8M2I14M?
7+8+2+14=31bp