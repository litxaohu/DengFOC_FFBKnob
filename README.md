# DengFOC_FFBKnob

灯哥开源力反馈旋钮 是基于DengFOC V4驱动板开发的一个开源小巧无刷力控旋钮应用套件。
<div align=center> <img src="Image\FFBKnob.png" width = 90% /> </div>

## 演示视频
[旋钮演示视频](https://www.bilibili.com/video/BV19C4y1X7oA)

## 介绍

该开源项目基于 DengFOC V4驱动板开发。
如对本项目感兴趣，可以在我们[灯哥开源店铺](https://shop564514875.taobao.com/)里搜索 **力反馈旋钮** 购买。  
您的支持就是我们持续做开源内容和课程的动力，项目收益将用于后续开发DengFOC和做课程~


本项目使用[DengFOC V4无刷电机驱动板](http://dengfoc.com/#/dengfoc/DengFOC%E5%AE%98%E6%96%B9%E7%A1%AC%E4%BB%B6/1%E9%A9%B1%E5%8A%A8%E5%99%A8/1.1V4)通过DengFOC库来实现来实现旋钮的力反馈效果，并能够像微软的Surface Dial那样控制电脑的功能。此外，它还可以根据旋钮模式展现各种灯效。

- 硬件方案说明  
  力反馈旋钮由四个模块组成，分别为 DengFOC V4驱动板、磁编码器模块、RGB模块以及按键模块。  
  DengFOC V4驱动板是最主要的模块，该模块集成了ESP32主控，实现对各路模块和电机的控制，其中包括①板上逆变电路控制电机；②通过IIC读取编码器模块的电机角度信息；③通过单线串码控制RGB模块中每盏RGB灯的亮度以及颜色；④读取按键电平状态。

- 软件方案说明  
  开发环境：Arduino IDE  
  引用库：  
    + [DengFOC V0.4 开源电机驱动库详情点击查看](https://github.com/ToanTech/DengFOC_Lib/)  
    + DFOC_RGB   
    + OneButton
    + Blekeyboard

- 后续计划   
  + 增加更多酷炫的灯效  
  + 按键更改不同的盖帽  

## 特性

- 无刷电机力反馈效果
- 基于DengFOC V0.4 开源电机驱动库
- 支持控制电脑
- 支持多种灯效

## 仓库说明
- Src-力反馈旋钮实现代码
- Hardware-硬件，机械结构相关资料。包含3D打印文件，相关模块原理图、BOM等
- Docs-相关文档，包含安装文档，软件安装等
- Images


## 准备

硬件：
 - DengFOC V4驱动板（含INA240电流传感器）
 - 2208电机   
 - AS5600编码器
 - WS2812B光环
 - 轻触开关
 - SH1.0 5P线、GH1.25 4P线
 - 铜柱、螺丝若干

软件：
 - Arduino IDE或PlatformIO
 - Vofa +



## 搭建

- 力反馈旋钮安装  
详看本仓库Docs->安装文档

- 程序编译和下载  
  软件安装详看Docs->软件安装  
  程序代码详看本仓库Src



## 免费力反馈旋钮原理教学课程
  + [课时1 概论和课程简介](https://www.bilibili.com/video/BV18K411t7Wd/?vd_source=5d20af79ff500db9da1b6e7e1213da51)
  + [课时2  机械结构设计和DIY组装](https://www.bilibili.com/video/BV1d64y1K7nG/)
  + 课时3 旋钮力控功能实现-棘轮模式
  + 课时4 旋钮力控功能实现-边界模式
  + 课时5 旋钮力控功能实现-顺滑阻尼模式
  + 课时6 旋钮其他功能实现-按键、灯效
  + 课时7 旋钮其他功能实现-控制电脑

## 技术支持
为了更好地服务购买本产品的客户，我们设立了一个专门的售后群，用于解决客户在使用过程中遇到的问题。此外，我们还会定期发布有关产品的最新动态，以及有关产品的使用技巧，以帮助客户更好地了解产品，提高使用效率。Q群号：450913932


## 许可证
This project is licensed under the GPL-2.0 license

