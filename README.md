# 百宝箱
```
    百宝箱：寓意是满足我的一家三口的各种奇葩需求为起发
    我的需求：有2009年的笔记本电脑，不舍得仍，但是什么也做不了，所以拿他作nas存储部分
    老婆需求：记录宝宝生活、成长线、根据照片生成宝宝墙
    宝宝需求：实时定位

    项目成员：我一个人儿
    项目开发：前端flutter，后端java,服务器docker搭建、视频服务Python
    技术背景：技术上有现学的，有吃老本的
    开发周期：边奶娃，边写bug，时间无参考性
```
#### 2024-12：功能清单

    一、首页
        1.音视频
            1.1 音乐
                1.1.1 音乐播放时控制相关动画
                1.1.2 播放列表与播放logo切换
                1.1.3 播放列表自动滚动至播放位置
                1.1.4 后台播放服务

            1.2 视频
                1.2.1 视频封面（视频服务自动上报）
                1.2.2 视频播放功能按钮清单（播放、暂停、全屏、倍速、进度条）
                1.2.3 视频后台播放（前后台播放自动衔接播放进度和播放状态）
                1.2.4 视频服务：处理视频、视频数据上报、视频水印

        2.图库
            2.1 多数据源，数据合并
            2.2 图片缩放、下载、删除

        3.拍照
            3.1 拍照图片立即上传

        4. 启动页
            4.1 加载必要数据   

    二、侧边栏
        1.常用工具
            1.1 扫码
                1.1.1 文本生成二维码
                1.1.2 提取二维码内容 
                1.1.3 提取本地二维码图片中内容
            
            1.2 文件视图
                1.2.1 上传文件、视频、图片
                1.2.2 支持大文件上传 （断点续传）
                1.2.3 数据同步图库和视频列表中
                1.2.3 视频通知视频服务处理与数据上报

            1.3 悬浮按钮
                1.3.1 全局按钮，单击返回
                1.3.2 四个方向滑动，相应的功能打开

            1.4 天气查询
                1.4.1 查询各地方天气（个人喜好）

        2.会员福利
            2.1 笔记
                2.1.1 上传图片、上传视频
                2.1.2 非常讨厌绑定手机号、广告、使用时的限制条件

            2.2 我的硬盘
                2.2.1 上传 视频 图片
                2.2.2 解析图片隐藏信息，展示隐藏信息
                2.2.3 上报视频数据至视频服务，视频解析和数据上报 ，视频水印
                2.2.4 视频和图片同步到视频和图库列表
                2.2.5 支持大文件上传（断点续传）
                2.2.6 支持文件下载至本地（断点续传）

            2.3 聊天闲扯
                2.3.1 会话列表
                    2.3.1.1 好友会话
                    2.3.1.2 群聊会话
                        2.3.1.2.1 聊天成员管理
                2.3.2 好友列表
                2.3.3 我的
                2.3.4 添加好友
                2.3.5 创建群聊
                2.3.6 聊天功能
                    2.3.6.1 发送图片
                    2.3.6.2 发送视频
                    2.3.6.3 发送语音
                    2.3.6.4 听筒模式、喇叭模式
                    2.3.6.5 键盘弹性高度
                    2.3.6.6 键盘与功能面板切换

            2.4 网关工具
        
        3.Beta版本
            3.1 翻译

            3.2 定位
                3.2.1 宝宝专用

            3.3 黑乎乎（路线轨迹）
                3.2.1 宝宝专用

            3.4 图片自术
                3.4.1 图片扩展信息

            3.5 在线人数

            3.6 跨机复制
                3.6.1 信息数据共享
    
    三、登录与在线
        1. 网络状态
            1.1 检测当下网络状态与服务器连接状态（绿色、红色区分）

        2. 登录、注册
   
    四、保活

    五、视频服务

---

历史分割线

---
####   历史

```

      十几年的开发，让我深刻体会到：理论家不好干，实践未必简单多少~

```

**第一部分：**

初衷：
家里有几台闲置多年的老旧电脑，闲置而又不舍得处理，因此萌生了自己开发家庭App的想法。通过这个过程，不仅能够学习技术，还能够全面了解产品开发的整个流程，包括机器环境搭建、技术方案选择以及移动端开发知识等。

**第二部分：**

产品：
在开发过程中，我将产品定位为一个大杂烩，因为我喜欢自由发挥，遇到好奇的东西就会尝试开发对应的功能。

1. **爷爷专属App：** 这个App是为了解决带孙子的爷爷们记事不便的问题而设计的。通过这个App，爷爷们可以方便地记录重要事项，不用把家里的箱子写满，无处可写，哈哈(这个事情事后想起业界一句话了：快速迭代)。

2. **自嗨App：** 这个App是我个人天马行空，电脑的废物利用，其次摆脱了其他App频繁广告和强制操作等

   - **笔记功能：** 为了实现自由而创造的功能，避免了其他App的广告和各种绑定，而且现在好多东西还需要会员啥的。
   
   - **私聊功能：** 由于个人对通信技术的好奇，以及对聊天记录的理论与实践探索，实现了使用Netty进行私聊功能的开发，此前是理论家，只有大学时通过 socket开发过一个版本，事隔多日，自己有机会又搞了个。
   
   - **大文件上传：** 基于对技术的猎奇，实现了自己版本的大文件上传功能，了解断点续传，也是从理论家到实践中，多走了一步。
   
   - **临时数据：** 解决了跨设备传输信息的麻烦，简单的不得了，但是对自己而言好用的不得了。
   
   - **视频播放：** 主要是出于以前做过相关行业的工作，但是在视频操作上，始终停留在理论层面，这次算是实践下。
   
   - **刻录生活：** 此功能正在计划中，旨在记录宝宝的成长过程。

**第三部分：**

#### 初期小品展示：

##### 图片

<div style="display: flex; justify-content: space-between;">
    <img src="https://github.com/superluo/try2fly/blob/main/attach/s_1.png" alt="第1个" style="width: 280px; margin-right: 150px;">
    <img src="https://github.com/superluo/try2fly/blob/main/attach/s_2.jpg" alt="第2个" style="width: 280px; margin-right: 10px;">
</div>
<div style="display: flex; justify-content: space-between;">
    <img src="https://github.com/superluo/try2fly/blob/main/attach/s_3.png" alt="第3个" style="width: 280px; margin-right: 150px;">
    <img src="https://github.com/superluo/try2fly/blob/main/attach/s_4.png" alt="第4个" style="width: 280px; margin-right: 10px;">
</div>

<div style="display: flex; justify-content: space-between;">
    <img src="https://github.com/superluo/try2fly/blob/main/attach/s_6.jpg" alt="第5个" style="width: 280px; margin-right: 150px;">
    <img src="https://github.com/superluo/try2fly/blob/main/attach/s_5.png" alt="第6个" style="width: 280px; margin-right: 10px;">
</div>

<div style="display: flex; justify-content: space-between;">
    <img src="https://github.com/superluo/try2fly/blob/main/attach/s_8.jpg" alt="第7个" style="width: 280px; margin-right: 150px;">
    <img src="https://github.com/superluo/try2fly/blob/main/attach/s_7.jpg" alt="第8个" style="width: 280px; margin-right: 10px;">
</div>

<div style="display: flex; justify-content: space-between;">
    <img src="https://github.com/superluo/try2fly/blob/main/attach/s_9.png" alt="第9个" style="width: 280px; margin-right: 150px;">
    <img src="https://github.com/superluo/try2fly/blob/main/attach/s_10.png" alt="第10个" style="width: 280px; margin-right: 10px;">
</div>

<div style="display: flex; justify-content: space-between;">
    <img src="https://github.com/superluo/try2fly/blob/main/attach/s_11.png" alt="第11个" style="width: 280px; margin-right: 150px;">
    <img src="https://github.com/superluo/try2fly/blob/main/attach/s_12.png" alt="第12个" style="width: 280px; margin-right: 10px;">
</div>
---

##### 视频(可看完整的：attach/cover.mp4)

<video controls width="500">
  <source src="https://github.com/superluo/try2fly/blob/main/attach/tmp.mp4" type="video/mp4">
  可去附件中查看相对完整的功能：attach/cover.mp4
</video>

**The End**

```

争做技术应用学实践者：

勉强算是拥有些许联网行业相关开发经验，
包括互联网电视业务、广告投放平台引擎搭建、物联网IOT、旅游景点app(聚合支付)、美团酒店业务以及阿里电商交易和话费充值等领域。
不知不觉写了11年。

```