# 网络通讯模型

> 网络分层模型建议大家参考OSI的分层，因为五层协议模型做了简化少了两层。
这就导致比如像SSL你没办法划分。

对于网络通信的任何问题，都要在心里面有下面这个图。

![network-model](../../assets/imgs/topics/network/network-cover.jpg)


如图是计算机A向计算机B发送消息的过程。A发送的数据
会经过应用层打包，将结果交给表示层，
表示层再进行处理，交给会话层，经过这样层层处理到达
物理层，物理层保存着电信号，经过线路在节点之间传输。
途中会经过众多路由器，帮助我们寻找到B。
当经过重重路由到达B之后，会执行在A的反向过程，
这样B的应用层就可以拿到A发送的原始信息。