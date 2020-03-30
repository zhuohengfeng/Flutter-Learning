# Flutter入门笔记

## 一，环境搭建

### Flutter SDK安装

* 1. 在[Flutter官网](https://flutter.dev/docs/development/tools/sdk/releases)下载最新安装包，或者直接在Android Studio创建Flutter工程时下载SDK

* 2. 如果是下载安装包，解压到对应目录，然后设置到环境变量中：

```
$ cd ~
$ vim .bash_profile
```
 
修改.bash_profile：

```
export PATH="$PATH:'pwd'/flutter/bin"
```

* 3. 运行[^flutter doctor]来检测环境是否搭建成功

```
$ flutter doctor
```


### 创建和运行一个Flutter项目

* 1. 可以通过命令行的方式创建和运行Flutter项目：

```
$ flutter create my_first_app
$ cd my_first_app
$ flutter run -d 7B2A282E-24AC-4E9E-BEA1-F5F8F19AFB7C
$ flutter run -d ‘iPhone X’
```

* 2. 推荐使用Android Studio等IDE来创建项目(注意可以在这里安装SDK)：

<img width="480" alt="创建工程" src="images/chart_01/1_as_create_project.png">

> 需要安装 flutter 和 Dart 这2个插件 

* 3. 在Android Sutido中，可以指定启动的iOS或者Android的模拟器或者真机:

![选择设备](images/chart_01/2_as_select_device.png)

* 4. 运行后可以看到初始的demo界面：

<img width="240" alt="运行工程" src="images/chart_01/3_as_run_project.png">

> 任意的修改保存后，flutter会自动刷新UI 


### Flutter项目的构成

由于flutter是跨平台的，所以在工程中包含了android和ios的工程结构，可以分别用Android Studio和XCode来打开：

<img width="360" alt="工程结构" src="images/chart_01/4_as_project_structure.png">


## 二，入门基础知识


### 如何导入Widget

> 在Fluter中，万物皆Widget!!!

在Flutter中，要使用<font color=red>Material Design</font>库中的小部件，则需要导入<font color=red></font>material.dart包；
如果要使用iOS样式的widget，则要导入<font color=red>Cupertino</font>库。
要使用更基本的窗口widget集，需要导入widget库。当然，也可以导入自己编写的widget:

```java
import 'package:flutter/material.dart';
import 'package:flutter/cupertino.dart'; 
import 'package:flutter/widgets.dart'; 
import 'package:flutter/my_custom_widgets.dart'; 
```

### 如何写一个Hello World

在flutter中，可以使用Center和Text这2个widget来实现一个最简单的hello world：

<img width="480" alt="HelloWorld" src="images/chart_02/1_helloworld_code.png">

<img width="360" alt="HelloWorld" src="images/chart_02/2_helloworld_show.png">


### 如何生成更复杂的Widget树

> 重要的事情再说一遍：在Fluter中，万物皆Widget!!!

在flutter中，widget是用户界面的基本构建块，每个窗口widget都嵌套在父窗口的widget中，并从其父窗口继承属性。甚至应用程序对象本身也是一个组件。

Widget可以定义：

- 结构元素 - 如按钮或菜单
- 文本元素 - 像字体或颜色主题
- 类似布局的填充或对齐的一个方向





## 三，项目结构、资源、依赖、本地化


## 四，认识视图(Views)


## 五，布局与列表


## 六，状态管理


## 七，路由与导航


## 八，线程和异步UI


## 九，手势检测及触摸事件处理


## 十，主题和文字处理


## 十一，表单输入与富文本


## 十二，调用硬件、第三方SDK以及平台交互、通知









