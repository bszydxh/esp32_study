# esp32_study

#### ------更新于12/28-------
## 写在前面
整个项目立于2021-11-10

起因是b站上突然发现的视频

视频就不放了

    关键词:esp8266 舵机 开灯

然后在cubegarden群(某个mc屑服务器)友好的交流之后

就忍痛不氪了原神小月卡

买了个实体月卡 (不是)

心想着欸↗,美滋滋

得...坐牢的开始 (嘤嘤嘤)

言归正传 本项目基于arduino框架

vscode platfromio平台开发

本人小白 大佬轻喷
## 配置清单
    Goouuu-ESP32模块开发板 * 1

    面包板 * 1

    ws2812b 灯带 (滴胶 60灯/m) * 2m

    0.96寸 SSD1306 OLED屏 (4引脚单色) * 1

    mirco转usb<u>数据线</u>

    dc母头 接线器 若干

    灯带免焊连接口(对应店家的) 若干

    快速接线端子 若干

    usb转dc线 若干

    三色导线 若干 (适配灯带)

    杜邦线 若干 (公对母,公对公,母对母)

## 支持功能
1. 小爱同学操控(无外部按键,blinker接入)
2. 流光溢彩/音效律动效果(电脑端下载Prismatik软件,选择adalight)
3. 显示屏(一言/西安疫情实时人数/天气/时钟)
## 注意事项 
1. 灯带不必外接电容/电阻
2. 务必保证所有电源共地(esp32/灯带供电)
3. 禁止用esp32对灯带供电,灯带电流约5A,会烧的
4. 务必保证灯带不进水,走线不碰水
5. 保证你的esp32有多余引脚进行配置(3个或以上)
## TODO LIST
1. 蓝牙相关功能开发
2. 基于esp32自带freertos进一步优化任务调布
## Q&A(自问自答)
1. 至于第一块? 

    别问,问就是5v的电压接在了3.3v的引脚上了把这东西击穿了(手贱),显示屏也烧了
    
        这esp32十分的珍贵
    
    一片30CNY , 嘤嘤嘤
2. 引脚设置?

   main.cpp前面的注释标明了

3. 灯带走线?

   上48,下48,侧24
   因地制宜