### 什么是WIFI CSI
CSI全称叫做 信道状态信息(Channel State Information)。 它记录和表征了通信信道从发送端到接收端的各种状态信息。 由于周围物体的反射、衍射,散射，无线信号经过多个路径从发送端到达接收端， CSI用来量化发送与接收端之间的无线传播信道。 **本质上，CSI表征了每对天线之间每个子载波的信道频率响应(CFR)**。 [1] 
<img src="./img/WIFI-CSI.png">

> 这里需要补充一点，需要做的工作是获取CSI数据，根据CSI数据进行深度学习。 通过CSI数据的变化来判断人体手势变化。 所以工作的重点不在于CSI数据所代表的通信知识，而是获取到CSI数据后的利用。 所以这里对CSI数据以及背后的通信知识做一个简单了解即可 (个人理解)  

#### 名词解释
* 载波(carrier) : 指的是承载信息的信号波。 
* CFR(信道频率响应) : 信号的多径传播在时域上表现为时延扩展，信道的冲击响应通常就代表了这信息。信道的这些影响在频域上带来的影响是选择性衰。直观上看这是由于信道中有不同延时的路径，通过不同路径的信号在接收端叠加增强或相消，使不同的频率的信号发生不同的衰减。 [2] 
* OFDM(正交频分复用) : 是一种多载波调制技术，优点是：有效对抗频率选择性衰落，克服信号符号间的干扰。
### 如何收集WIFI CSI数据
能够收集CSI数据的方式有很多种.[3] [4]
#### Widar3 Dataset
使用现有数据集是最快，最简单的方法。 [5]
下载链接: http://tns.thss.tsinghua.edu.cn/widar3.0/
该数据集主要由三部分组成 CSI文件夹、DFS文件夹、BVP文件夹。 
##### 概念解释
DFS(Doppler frequency shift) : 是CSI的一个物理特征，叫做多普勒频率偏移
BVP( body-coordinate ve-locity profile) : 描述了不同速度下的功率分布，其中身体部位参与手势运动。  (Widar3独有的一种方法)

#### PicoScenes Platform

#### Intel 5300 NIC CSI Tool
#### Atheros CSI Tool
#### ESP32 CSI Toolkit

### 基于WIFI CSI数据的手势识别

#### 知识点

#### 实现步骤及手段






### references

[1] WIFI CSI-based vital signs monitoring
[2] https://iot-book.github.io/
[3] Hands-on Wireless Sensing with Wi-Fi A Tutorial
[4] https://iot-book.github.io/17_WiFi%E6%84%9F%E7%9F%A5/S1_%E4%BF%A1%E9%81%93%E7%8A%B6%E6%80%81%E4%BF%A1%E6%81%AF%E8%8E%B7%E5%8F%96/
[5] TPAMI_Widar3.0_paper.pdf