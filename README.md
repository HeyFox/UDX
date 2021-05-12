# UDX A Fast and Reliable ARQ and AQR Protocol - FastUdx A NEW TCP OVER UDP IMPL

UDX协议是FastUdx的缩写，原本的意思是UDP的扩展，X表示未知，强大的意思。UDX是基于标准C++接口开发的一套UDP可靠协议。

![image](https://github.com/HeyFox/UDX/blob/main/my_logo_big.png)


# UDX能干什么？

 1.高效的传输模块;
 
 2.NAT P2P穿透，转发模块;
 
 3.文件传输模块;

# 技术特性：

 UDX是为充分利用带宽，并且不增加延迟。完全模拟TCP行为的一套UDP传输系统。可与FEC纠错算法一起工作。
 
 较目前国内外同类协议有较明显优势。

# 技术指标：

 1.吞吐量: 在较低包率下，达到90%以上的代宽利用率。
 
 2.低延迟: 如果线路固有的PING值在100MS的话，当最大吞吐量的时候，PING值不应该大于200ms.
 
 3.流量稳定: 通过流量工具软件，比如一些带UI的界面工具，可以看到，收发流量基本稳定在一个水平，流量波形形成一条直线为佳。

 4.rtt稳定: 如果线路固有的PING值在100MS的话，当最大吞吐量的时候，RTT值稳定在100-200ms之间。
 
 5.低ACK:在最大吞吐量的情况下，100mbps的吞吐量，ACK量不应该超过100kbps.

 6.双向稳流:比如，家用代宽，上传速度为40mbps,下载速度为200mbps。那么最好通双向同时上传与下载达到40m上传与200m的速度，并且满足条件4.


# 基本使用：

 客户端:
 
  ./fudx c server_ip server_port upload
  
  ./fudx c server_ip server_port  upload10  带FEC模式
  
 服务端 :
 
  ./fudx s server_port

# demo系统要求：centeros64 /WIN7

# 主页：www.goodudx.com
