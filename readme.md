
# Data Viewer

## 1.介绍
Data Viewer 是一个开源的TDMS和Execl数据回放查看器，源码采用Actor　Freamwork编写，在AF的基础上构建了MVVM的思想进行封装，该工具采用MVVM的基础架构实现，并且实现以下功能，同时此代码可以作为学习使用；
1. 数据波形查看；
2. 数据表格查看；
3. 自动播放；
4. 上一帧；
5. 下一帧；
6. 颜色主题设置；（绿白、蓝白、黑暗）；
7. 支持多通道选择；
8. 支持TDMS和Excel;

---
 :smile: 
 
---

## 2.开发环境

1. LabVIEW 2020
2. Actor Freamwork

依赖：
1. agilet_lib_mullistbox-1.0.0.2.vip

## 3. 文件夹说明
```
├─01 Design \\设计文档
├─02 Docs  \\文档
├─03 Depend On \\依赖库安装包
├─04 Source
│  ├─Controller \\控制器
│  │  └─Controller
│  │      └─Controller
│  │          ├─Accessor
│  │          ├─Control
│  │          ├─Message
│  │          ├─Method
│  │          ├─Override
│  │          └─Private
│  ├─Controls  \\控件库
│  ├─Data
│  │  └─icons \\数据文件
│  ├─Depden On \\ 架构文件
│  │  ├─Abstruct View \\View
│  │  │  ├─Abstruct View
│  │  │  │  ├─Data Accessors
│  │  │  │  ├─Methods
│  │  │  │  └─Override
│  │  │  └─Abstruct View Messages
│  │  │      ├─Hidden Front Msg
│  │  │      ├─Insert Panel Msg
│  │  │      └─Show Front Msg
│  │  ├─ActorMap \\数据结构
│  │  │  └─methods
│  │  └─MVVM Framework \\MVVM 架构 
│  │      ├─Abstruct Data
│  │      │  └─Accessors
│  │      ├─Enqueues Data
│  │      │  └─Accessors
│  │      ├─Model&View Interface
│  │      ├─Model&View Interface Messages
│  │      │  └─Brocast Data Msg
│  │      ├─MVVM Abstruct Controller
│  │      │  ├─MVVM Abstruct Controller
│  │      │  │  ├─Accessor
│  │      │  │  ├─Control
│  │      │  │  ├─Message
│  │      │  │  ├─Method
│  │      │  │  ├─Override
│  │      │  │  ├─Private
│  │      │  │  └─Utils
│  │      │  └─MVVM Abstruct Controller Messages
│  │      │      ├─Add & Register Models Msg
│  │      │      ├─Add & Register Views Msg
│  │      │      └─Brocadcast Models&Views Msg
│  │      ├─MVVM Abstruct Model
│  │      │  └─MVVM Abstruct Model
│  │      │      ├─Accessor
│  │      │      ├─Control
│  │      │      ├─Message
│  │      │      ├─Method
│  │      │      ├─Override
│  │      │      ├─Private
│  │      │      └─Utils
│  │      └─MVVM Abstruct View
│  │          └─MVVM Abstruct View
│  │              ├─Accessor
│  │              ├─Control
│  │              ├─Message
│  │              ├─Method
│  │              ├─Override
│  │              ├─Private
│  │              └─Utils
│  ├─Models \\ Model
│  │  ├─Data List
│  │  │  └─Accessors
│  │  ├─Data Loader
│  │  │  ├─Data Load Interface
│  │  │  │  ├─Data Load Interface
│  │  │  │  └─Data Load Interface Messages
│  │  │  │      ├─File Range Msg
│  │  │  │      ├─Load File Msg
│  │  │  │      ├─Select Channel Msg
│  │  │  │      └─Select File Msg
│  │  │  └─Data Loader
│  │  │      └─Data Loader
│  │  │          ├─Accessor
│  │  │          ├─Control
│  │  │          ├─Message
│  │  │          ├─Method
│  │  │          ├─Override
│  │  │          └─Private
│  │  └─Data Types
│  │      ├─Abstrut Data
│  │      │  ├─Accessors
│  │      │  ├─Methods
│  │      │  └─Override
│  │      ├─File Operate Interface
│  │      │  └─Methods
│  │      └─TDMS
│  │          └─Override
│  ├─Test
│  ├─Test Data
│  └─Views 
│      ├─Color Interface \\接口
│      │  ├─Color
│      │  │  └─Accessors
│      │  ├─Color Interface
│      │  └─Color Interface Messages
│      │      └─Set Color Msg
│      ├─Data Interface
│      │  ├─Data Interface
│      │  ├─Data Interface Messages
│      │  │  └─Update Data Msg
│      │  └─Message
│      ├─Data List Infor Interface
│      ├─Data List Infor Interface Messages
│      │  └─Data List Msg
│      ├─Setting View
│      │  ├─Setting View
│      │  │  ├─Accessor
│      │  │  ├─Control
│      │  │  ├─Message
│      │  │  ├─Method
│      │  │  ├─Override
│      │  │  └─Private
│      │  └─Setting View Messages
│      │      └─Set Color To Caller Msg
│      ├─System Tree View
│      │  ├─System Tree View
│      │  │  ├─Control
│      │  │  ├─Data Accessor
│      │  │  ├─Message
│      │  │  ├─Methods
│      │  │  ├─Override Methods
│      │  │  └─Private
│      │  ├─System Tree View Messages
│      │  │  ├─Add Msg To Seq Msg
│      │  │  └─Update Tree Items Msg
│      │  ├─Unit Test
│      │  └─[V]System Tree View Messages
│      │      └─Select Channels Msg
│      ├─Table View
│      │  └─Table View
│      │      ├─Accessor
│      │      ├─Control
│      │      ├─Message
│      │      ├─Method
│      │      ├─Override
│      │      └─Private
│      ├─[V] Main UI
│      │  ├─[V] Main UI
│      │  │  ├─Accessor
│      │  │  ├─Control
│      │  │  ├─Message
│      │  │  ├─Method
│      │  │  ├─Override
│      │  │  └─Private
│      │  └─[V] Main UI Messages
│      │      ├─Data View Display Msg
│      │      ├─Last Frame Msg
│      │      ├─Launch Setting Msg
│      │      ├─Next Frame Msg
│      │      ├─Play Pause Msg
│      │      ├─Range Msg
│      │      └─Select Path Msg
│      └─[V]Waveform Display
│          └─[V]Waveform Display
│              ├─Accessor
│              ├─Control
│              ├─Message
│              ├─Method
│              ├─Override
│              └─Private
└─05 Release \\发布版本
    └─Version 1.0
```

## 4. 演示视频


![image](https://github.com/ShoutangYang/DataViewer/blob/master/02%20Docs/Data%20View%20Blue.PNG?raw=true)


![image](https://github.com/ShoutangYang/DataViewer/blob/master/02%20Docs/Data%20View%20Green.PNG?raw=true)



<iframe src="https://github.com/ShoutangYang/DataViewer/blob/master/02%20Docs/Data%20Viewer.mp4" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> 
</iframe>



<iframe src="https://www.bilibili.com/video/BV1q44y1d76B/?share_source=copy_web&vd_source=2facec77856aaa88af1acdb09c60574b" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>

