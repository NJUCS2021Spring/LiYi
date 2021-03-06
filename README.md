# Welcome
欢迎南京大学计算机系2020级新生参与本次项目实践！！

本项目期望通过一次较大型项目的编程实践将一些常用的开发工具以及流程介绍给大家，有序促进大家的复习和预习工作，动手开始吧！

## Step 0：使用Git进行代码管理

选择项目说明中的任意一个项目进行构思，按照参考材料中的"GitHub远程仓库使用"说明，向自己的仓库中添加项目说明文件`REDAME.md`，简要介绍下自己的项目。项目介绍文件的编写示例可见`参考材料/任务0/项目ReadMe示例.md`

## Step 1：数据结构定义

自行预习程序设计基础教材中**类和对象**部分内容，找出项目中的关键对象并抽象成类（或结构体），为其定义数据成员和函数成员。定义类及其成员的思维过程可以参考`参考材料/任务1/类的功能与实现——以项目2为例.md`

类及其数据成员一定程度反映了项目的数据结构；而对数据结构的操纵则属于算法的范畴，一般在函数成员中实现。当然还未系统学习算法和数据结构的同学们不要被这两个高大上的概念吓唬到，函数成员一般是项目中的某个应用场景，例如主界面显示`main_menu()`;或是某个细分的小功能，例如排序等等，大家可以自行思考和设计。

上述类及其成员的定义一般在**单独的头文件**中完成。

**建议DLL:2021-2-22 23:59:59**

## Step 2：项目框架搭建

在完成类及其成员的定义后，我们并不能确保自己拍拍脑袋想出来的函数成员已经涵盖所有功能，但应该保证足以搭建整个项目的框架代码。换言之，我们为类添加的成员函数应该为项目的所有业务搭建顺畅的逻辑，比如：界面的跳转。当框架搭建完成后，我们再完成功能的填充，此时任务1中未考虑到的功能函数只要随用随添加便可。

在本次任务中，我们将完成项目框架的搭建，目标是实现一个包含功能选择以及界面跳转的程序，具体功能留空，只做一个能run起来、看起来像样的项目框架。参考材料见`参考材料/任务2/`

在任务2的过程中我们可以重新思考、修改和完善任务1中的类定义

**建议DDL:2021-2-23 23:59:59**

## Step 3：具体功能实现

在项目框架搭建完后，只需要把每个功能函数具体实现，整个项目便大功告成了。

该部分不必多言，敲就完事儿！

我们可以采用最朴素的思想去实现每个功能，譬如采用顺序遍历的方法去做单词的查找、车次的查找，但当数据量十分庞大时，低效的方法通常带来过长的响应时间，这将大大降低使用体验。我们不得不考虑算法设计范畴的效率问题，参考材料会给大家介绍一些日后要学习的、与项目相关的算法，包括：排序、查找、字符串匹配等。感兴趣的同学可以自行学习，当然采用最朴素的想法亦可完成项目！

**建议DDL:2021-2-27 23:59:59**

## Step 4：GUI

GUI（Graphical User Interface）即图形用户界面，是采用图形方式显示计算机用户的操作界面，大家目前使用的大部分应用程序都是通过GUI与用户交互的。

在实现所有的项目功能后，大家可能也厌倦了命令行黑框框程序，通过命令行输入功能序号来选择功能远比直接使用鼠标点击繁琐。接下来就让我们为项目设计GUI吧！

我们将使用Qt作为开发框架，大家可以先自学Qt相关知识 https://www.bilibili.com/video/av837578381/

值得提醒的是，GUI设计并不是GUI程序开发的最后一步，而是在Step1-Step3的每一步都有涉及，彼时，Step1-Step3的所有工作将在一个特定的框架（例如Qt)下进行。

**Duration:2021-2-28 00:00:00 - to be decided**



## 结语

以上步骤是给大家进行此类项目开发的一个流程参考，给出的DLL并不是firm DDL，大家照此进度进行将便于我们收集材料和问题并统一给出反馈。期望大家在寒假的尾声能够合理安排时间，充实生活，充实自己，提前祝大家返校顺利，假期愉快！！