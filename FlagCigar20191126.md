1. Explain BAM FLAG value： 143=128+8+4+2+1
在paired reads中，该read是与参考序列比对的第二条；该read是成对的paired reads中的一个；paired reads中每个都正确比对到参考序列上；与该read成对的matepair read没有比对到参考序列上；该read没比对到参考序列上。
2. Explain BAM FLAG value： 99=64+32+2+1
在paired reads中，该read是与参考序列比对的第一条；与该read成对的matepair read其反向互补序列能够比对到参考序列；该read是成对的paired reads中的一个； paired reads中每个都正确比对到参考序列上。
3. Explain BAM FLAG value：516=512+4
该read没有通过质量控制 ；该read没比对到参考序列上。
4. Explain BAM FLAG value： 2064=2048+16
补充匹配的read；该read其反向互补序列能够比对到参考序列。
5. Explain BAM FLAG value： 147=128+16+2+1
在paired reads中，该read是与参考序列比对的第二条；该read其反向互补序列能够比对到参考序列；paired reads中每个都正确比对到参考序列上；该read是成对的paired reads中的一个。
6. Explain BAM CIGAR：14M2D31M
read的碱基序列前端有14个碱基、尾端有31个碱基可mapping到第三列的序列上，与第三列的序列碱基相同；read的碱基序列的中间相对于第三列的RNAME序列，有2个碱基的删除。
7. Explain BAM CIGAR：3S6M1D5M
read的碱基序列前端有3个碱基soft clipping；read的碱基序列中间有6个碱基、尾端有5个碱基可mapping到第三列的序列上，与第三列的序列碱基相同；read的碱基序列的中间相对于第三列的RNAME序列，有1个碱基的删除。
8. Explain BAM CIGAR: 6M14N5M
read的碱基序列前端有6个碱基、尾端有5个碱基可mapping到第三列的序列上，与第三列的序列碱基相同；read的碱基序列中间有14个碱基的可变剪接位置。
9. Explain BAM CIGAR: 7M5D8M2I14M  (小写：7m5d8m2i14m）
read的碱基序列前端有7个碱基、中间有8个碱基、尾端有14个碱基可mapping到第三列的序列上，与第三列的序列碱基相同；在read的碱基序列中相对于第三列的RNAME序列，有5个碱基的删除，这段序列位于7个可mapping的碱基序列和8个可mapping的碱基序列中间；read的碱基序列相对于第三列的RNAME序列，有2个碱基的插入，这段序列位于8个可mapping的碱基序列和14个可mapping的碱基序列中间。
10. how long is the read with alignment CIGAR of 7M5D8M2I14M?
M:7+8+14=31;I：2；序列长度：M+I=31+2=33           
