[![Build Status](https://travis-ci.org/fossasia/bodyapps-viz.svg?branch=master)](https://travis-ci.org/fossasia/bodyapps-viz)
[![Join the chat at https://gitter.im/fossasia/bodyapps-android](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/fossasia/bodyapps?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

http://bodyapps-viz.luhui.net/


[![Netlify Status](https://api.netlify.com/api/v1/badges/30d2fb2f-1ace-4ea7-96cf-c0f594965597/deploy-status)](https://app.netlify.com/sites/bodyapps-viz/deploys)

https://bodyapps-viz.netlify.app/


luhui BodyApps 3D 身体可视化器
#luhui bodyapps 项目的 3D 身体可视化组件

关于
luhui Body Visualiser 应用程序试图创建一个基于 Web 的 3D 人体可视化器，其中包含导入身体测量值的选项，使用 Fashiontec 的 BodyApps Web 服务并使用滑块功能对人体进行建模。

该应用程序支持男性、女性和中性儿童身体模型，并可选择修改以下身体尺寸和特征。

## 绘制展示
![luhui BodyApps 3D 身体可视化器绘制展示](http://bodyapps-viz.luhui.net/luhuiOpnTecbodyapps-vizthumbnails1.jpg)
![luhui BodyApps 3D 身体可视化器绘制展示](http://bodyapps-viz.luhui.net/luhuiOpnTecbodyapps-vizthumbnails2.jpg)
![luhui BodyApps 3D 身体可视化器绘制展示](http://bodyapps-viz.luhui.net/luhuiOpnTecbodyapps-vizthumbnails3.jpg)
![luhui BodyApps 3D 身体可视化器绘制展示](http://bodyapps-viz.luhui.net/luhuiOpnTecbodyapps-vizthumbnails4.jpg)


高度
胸部/胸部
颈围
颈部高度
肩膀
肩坡
胸围
胃型
腰部
臂长
上臂围
手腕
臀围
臀高
大腿围
小腿长度
小牛
沟通
请加入我们的沟通渠道。

邮件列表位于：https ://groups.google.com/forum/#!forum/bodyapps

Gitter 聊天：https ://gitter.im/fossasia/bodyapps

构建项目
1.Clone Master Repo 2.找到文件夹，然后运行index.html（如果没有启用则启用Javascript）

文件夹
BodyViz 项目有 3 个文件夹

css - 包含 BodyVisualiser 的样式表
模型 - 包含人类基础模型及其变形目标的 .js 文件以及所有模型的配置文件
js-包含三个.js 和 UCSCharacter.js，允许渲染和自定义模型。
除此之外还有其他三个文件

index.html - 可视化男性身体
female.html-可视化女性身体
kids.html-可视化孩子的身体
楷模
剥皮的

统一通信系统

basic.js-Three.js 人体男性模型，由 Blender 导出

female.js-Three.js 人体女性模型，由 Blender 导出

child.js-Three.js 人体模型，由 Blender 导出

皮肤

Highlighted_Muscles.jpg：人体模型的皮肤 UV 贴图。

testconfig.json - 男性身体的配置文件。

女性身体的 femaleconfig.json-config 文件。

孩子身体的 childconfig.json-config 文件。

###js

Orbit.js-由three.js org开发，具有设置相机轨道和启用3D切换视图的功能。
Three.js-由three.js org开发，具有在web视图中渲染three.js导出的模型并使用Morph Targets自定义人体模型的功能
data.gui.js-由 data.gui.js 开发，允许为可视化器创建滑块和 gui。
detector.js-检测windows分辨率并根据它调整可视化器的分辨率
UCSCharacter.js-包含渲染调用模型数据并使用three.js库渲染它的函数。它还具有监听滑块变化和根据需要更新身体可视化模型的函数。
使用的其他软件和库
三.js
Three.js 是一个轻量级的跨浏览器 JavaScript 库/API，用于在 Web 浏览器上创建和显示动画 3D 计算机图形。Three.js 脚本可以与 HTML5 画布元素、SVG 或 WebGL 结合使用。源代码托管在 GitHub 上的存储库中。

搅拌机 2.70
Blender 是一个用于建模、动画、渲染、合成、视频编辑和游戏创建的开源 3D 应用程序。Blender 可用于 Linux、Mac OS X 和 Windows，并拥有庞大的全球社区。Blender 可以免费用于任何目的，包括商业用途和分发。它是免费的开源软件，在 GNU GPL 许可下发布。

该项目广泛使用 Blender 和 Three.js 导出/导入脚本[1][2] 来设计变形目标，然后以 three.js 格式导出模型。

造人
MakeHuman 是一个开源 3D 计算机图形软件中间件，专为照片逼真的人形机器人原型设计。它由对角色 3D 建模感兴趣的程序员、艺术家和学者组成的社区开发。MakeHuman 是完全开源的。MakeHuman 的字符输出在 CC0 下发布到公共领域，以便在商业和非商业项目中自由使用。数据库和代码在 GNU 许可证 Affero GPL 下发布。

MakeHuman 模型被用作该项目的基础模型，并且从 MakeHuman 项目的变形目标中获得了一些变形目标的开发。MakeHuman 项目允许以各种格式导出模型。
