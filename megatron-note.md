# Megatron-LM源码

## pipeline



1. F then B memory = K x M   有K个micro batch，每个micro batch的激活值为M。因为每个 m的前向传播结果必须保存到反向传播开始才能释放。
2. 