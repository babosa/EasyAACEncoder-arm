## EasyAACEncoder-arm ##

**EasyAACEncoder-arm** 是EasyDarwin流媒体团队开发与维护的一款商用音频转码到AAC的工具库，目前支持G711a/G711u/G726/PCM等音频格式的转码，跨平台，支持Windows（32&64）/Linux（32&64）/ARM各平台，相比于其他普通类型的音频转码库，效率有极大提升；

> 我们发现在类似于hisi海思芯片的大部分ARM系统中，对浮点运算的支持都不是很好，效率非常低，导致在ARM设备中直接将PCM类型音频转成AAC时，效率非常低，于是我们根据特定的ARM平台定制整理出了一套商用版本的音频转码EasyAACEncoder SDK，目前海思（hisiv100、hisiv200、hisiv300、hisiv400）全系列均已支持，CPU占用率极低，能非常好地满足ARM平台的AAC音频转码需求！


## 调用示例 ##

- **testEasyAACEncoder**：通过EasyAACEncoderAPI对G711A/G711U/G726进行AAC转码；

		chmod +x ./Buildit
		./Buildit


- **ARM版本目前已经定制了hisiv100、hisiv200、hisiv300、hisiv400多个平台，如需其他ARM平台版本，请发送邮件support@easydarwin.org，附上对应ARM平台的交叉编译工具链，我们为您定制开发对应版本的EasyAACEncoder-arm转码库！**；

## 调用过程 ##
![](http://www.easydarwin.org/skin/easydarwin/images/easyaacencoder20180822.png)


## 特殊说明 ##
EasyAACEncoder目前支持的音视频格式：

	/* Audio Codec */
	enum Law
	{
		Law_ULaw	=	0, 		/**< U law */
		Law_ALaw	=	1, 		/**< A law */
		Law_PCM16	=	2, 		/**< 16 bit uniform PCM values. 原始 pcm 数据 */  
		Law_G726	=	3		/**< G726 */
	};
	
	/* Rate Bits */
	enum Rate
	{
		Rate16kBits=2,	/**< 16k bits per second (2 bits per ADPCM sample) */
		Rate24kBits=3,	/**< 24k bits per second (3 bits per ADPCM sample) */
		Rate32kBits=4,	/**< 32k bits per second (4 bits per ADPCM sample) */
		Rate40kBits=5	/**< 40k bits per second (5 bits per ADPCM sample) */
	};

## 技术支持 ##

- 邮件：[support@easydarwin.org](mailto:support@easydarwin.org) 

- QQ交流群：<a href="https://jq.qq.com/?_wv=1027&k=5gM0Fex" title="EasyAACEncoder-arm" target="_blank">**538316953**</a>

> EasyAACEncoder-arm是一款非常稳定、高效的音频转码组件，各平台版本需要经过授权才能商业使用，商业授权方案可以通过以上渠道进行更深入的技术与合作咨询；


## 获取更多信息 ##

**EasyDSS**商用流媒体解决方案：[www.EasyDSS.com](http://www.easydss.com)

**EasyNVR**无插件直播方案：[www.EasyNVR.com](http://www.easynvr.com)

Copyright &copy; EasyDarwin Team 2012-2019

![EasyDarwin](http://www.easydarwin.org/skin/easydarwin/images/wx_qrcode.jpg)
