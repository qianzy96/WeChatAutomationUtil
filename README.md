#### 微信自动化工具---自动发送朋友圈（非root权限）
### 一、效果图
![微信自动化](https://github.com/EdwardSituwende/WeChatAutomationUtil/blob/master/wechat_auto.gif?raw=true)
</br></br></br>
### 二、测试Android设备
我在这两款设备测试正常，其它设备如果有什么问题，欢迎给我反馈^_^
</br>
夜神模拟器(Android 4.3)、华为荣耀8青春版(Android 7.0)
</br></br></br>
### 三、原理
整个app的核心是AccessibilitySampleService类，它继承了AccessibilityService服务。
在辅助功能打开之后，AccessibilitySampleService类会监听目标APP（微信）页面的状态变化。
之后使用Android官方提供的UI Automator Viewer工具，查看目标APP（微信）的布局结构树。
![](https://github.com/EdwardSituwende/WeChatAutomationUtil/blob/master/wechat_auto1.png?raw=true)
根据rescoure-id搜索出相应的控件，再对这些控件执行点击、复制、粘贴等操作。
</br></br></br>
### 四、注意事项
1、Android设备必须安装微信app
</br>
2、Android Sdk Version>18
</br>
<font color=#ff0000>特别提醒（不需要获取root权限）</font>
</br></br></br>
### 五、Repository
https://github.com/EdwardSituwende/WeChatAutomationUtil
</br></br></br></br></br></br>