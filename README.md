# 实验名称
Merkle_Tree_following_RFC6962

# 实验步骤
![Screenshot 2022-07-31 070636](https://user-images.githubusercontent.com/104854836/182003031-6b770c7a-bae5-461a-8d68-1b5797b382cd.jpg)
通过这个图，我理解到实现改项目的步骤如下

1.首先对每一个tx进行编码，然后在前面补充0x00，得到和tx数量一样的Hash值

2.从左到右一次遍历，两个一组拼接后两两组合，拼接后在前面补充0x01，如果有落单的Hash值就往上挪一层

3.一层一层以此类推最终得到一个hash值

部分代码如图所示：
![Screenshot 2022-07-31 071221](https://user-images.githubusercontent.com/104854836/182003144-a91f9b59-4901-42e7-82c9-aba7384d6c4b.jpg)

# 实验结果
在本次实验中，我加密了10000个数据，这10000个数字都是随机生成的

![Screenshot 2022-07-31 105620](https://user-images.githubusercontent.com/104854836/182007870-9fe177b3-7f92-4f7c-9644-d4d3e0845eb5.jpg)



