---
banner: "![[image1.jpg]]"
banner_y: 0.6
banner_icon: 📖 
---

# 🌈 01 简介

- 一个专为科研人打造的Obsidian开箱即用库！
- 利用双链、各种插件&优秀软件联动来**搭建个人wiki知识库**、**提升笔记书写体验**以及**进行学术写作**！

![Home](https://user-images.githubusercontent.com/120721474/208292126-33453a8a-53f7-4406-8612-bf587215f770.png)


# 🛠️ 02 Changelog
- 2022/12/18日更新
	- 新增学术写作场景
	- 更新文献笔记阅读模板
	- 文献笔记汇总管理由dataview更换为db folder
	- 更新Home页呈现方式


# 🧭 03 使用指南

## 3.1 Obsidian基础设置

- 删除文件设置：软件内回收站
- 附件：已设置新附件自动添加到Z-附件/images文件夹下
- 新建笔记：已设置为存放在当前打开的笔记所在的文件夹下
- 模板：几个模板文件，都在Z-附件/Templates文件夹下
- 搜索命令：ctrl+P
- 搜索笔记：ctrl+K
- 快速添加标题级别：ctrl+1,2,3,4,5,6（最多到6级标题，本人基本只用到3级）

## 3.2 主题

- 本库一共内置了3款主题，分别为Obsidian官方主题、minimal主题和Blue Topaz主题，当前使用的是Blue Topaz主题
- 如果你不喜欢此主题可以自行[[更换主题]]，这不会对本库的功能产生任何影响
- 如果你不喜欢主题的某些点（比如字号、字体、字体颜色、链接颜色、页面背景等等）
	- 可以通过[[主题设置插件]]进行调节
	- 可以通过css片段（自己写或者去论坛找）来配置外观

> 一点儿小建议：不要总是折腾主题，多做点儿有用的笔记吧~


## 3.3 文件列表介绍
在文件列表区一共展示了6个文件夹和2个文件
- **@Inbox文件夹**：主要用于存放简悦、以及一些待处理的文件/文件夹
- **A-专业知识**：用来存放知识体系中最基本的概念，原理等（可涉及各学科），本人一般将其和B-科研笔记文件夹搭配使用（后面会介绍）
- **B-科研笔记**：用来存放和科研学术相关的所有笔记
- **C-生活规划**：用来存放日常备忘以及一些书影音等笔记
- **D-软件技能**：用来存放软件和技能学习的笔记
- **Z-附件**：用来存放[[模板]]、[[附件]]之类的文件
- **Home页**：也就是[[MOC]]（Map of Contents），主要用于添加常用笔记的双链，当然还可以用来汇总**文献笔记**和[[一键随想笔记]]

## 3.4 本库两大核心使用场景

### 3.4.1 文献阅读笔记场景

- 阅读前
	- 打开zotero&Obsidian
	- 通过Mdnotes插件在zotero中创建此篇文献的笔记，并导入Obsidian中
	- 使用zotero自带的PDF阅读器或者其它PDF软件打开此篇文献
- 阅读中
	- 边阅读边思考边回答笔记中的几个问题
	- 遇到需要补充的专业知识，直接点击下方状态栏中的专业知识图标，然后填入名称，就会自动创建一条笔记进入**A-专业知识文件夹**
		-  ![image](https://user-images.githubusercontent.com/120721474/208292032-b6f9748e-c224-454b-8b15-090915ac08ab.png)
	- 遇到搞不懂的问题或者有一些新的想法，直接点击下方状态栏中的文献随想图标，然后填入问题名称，就会自动创建一条随想笔记进入**B-科研笔记/B08-文献阅读/文献阅读随想文件夹**
		- ![image](https://user-images.githubusercontent.com/120721474/208292042-e1497da7-098d-4e3b-994b-36e7881471c7.png)
- 阅读后
	- 点击左侧边栏的工作区图标，然后点击Reading Notes Database
	- 打开Reading Notes Database后，
		- 在Comment这里填入此篇文献有哪些地方是你感兴趣的以及你对此篇文献中的工作有何评价
		- 在标签栏里给其几个标签
		- 在Rating栏里给其评级
	- 在闲暇有空时，记得打开文献阅读随想MOC，尝试回答其中的问题

实现以上效果[[zotero+Obsidian+db folder]]，我们还是需要先在zotero中配置一番的，只需配置zotero中的一部分，Ob中无需配置（包括模板都是现成的，在Z-附件/Templates文件夹下）


### 3.4.2 学术论文写作场景

- 在Ob中直接进行学术论文的书写，包括公式，图片，参考文献插入等都是极其丝滑的
- 如果需要导出word格式，即可一键导出，包括参考文献&图片都能正常导出，并且导出的word文档中的参考文献格式依然可以利用zotero来进行批量管理

[[zotero+word+obsidian]]的配置教程

> 有必要说一下，在本人试用一段时间之后，建议真正想利用markdown编辑器进行学术写作的小伙伴去折腾此配置。毕竟写期刊论文用overleaf已经很舒适了，写毕业论文用word（配置好样式）也是极度舒适的~


## 3.5 Obsidian与各种优秀软件联用

> 以下内容仅作为一些联用场景供大家参考，如有需求可反馈，后续再做详细更新

- 与zotero联用：[https://mp.weixin.qq.com/s/DS3iDtS4JzDSR--F6eHEpg](https://mp.weixin.qq.com/s/DS3iDtS4JzDSR--F6eHEpg)
- 与cubox联用：[Obsidian的最强搭档 (qq.com)](https://mp.weixin.qq.com/s?__biz=MzU4MzgxNjczMA==&mid=2247484436&idx=1&sn=11384d2a4ecb2dcd44ec57bf9b3addf6&chksm=fda20761cad58e773b93786ff632621d0b23b08c4aad6e43b9cb8b9b2a74a7a6e867fbdf9597&scene=21#wechat_redirect)   ；[补充：将网页转换为Markdown的方法 (qq.com)](https://mp.weixin.qq.com/s?__biz=MzU4MzgxNjczMA==&mid=2247484458&idx=1&sn=5250c2eceb49f814e57e8df67e3d171a&chksm=fda2075fcad58e49ab21b280cfd95db9dc8735bcabb9e678e9a93139ce299e8dac1c9c771317&scene=21#wechat_redirect)
- 与github联用：这个也就是利用github仓库做免费图床，[https://mp.weixin.qq.com/s/myEO1nsA9SGKA8ctRgtNkA](https://mp.weixin.qq.com/s/myEO1nsA9SGKA8ctRgtNkA)
- 与ios快捷指令联用：[小技巧增强ios端remotely save同步体验 (qq.com)](https://mp.weixin.qq.com/s?__biz=MzU4MzgxNjczMA==&mid=2247484914&idx=1&sn=11d73cf076bd431fbf8d8cecff8d543c&chksm=fda20687cad58f9137c5b4c3f23034be5e07d7f2330b2f77f28a5f0429941d334f65a0ec31ce&scene=21#wechat_redirect)  ； [利用ios指令提升移动端obsidian使用体验 (qq.com)](https://mp.weixin.qq.com/s?__biz=MzU4MzgxNjczMA==&mid=2247484945&idx=1&sn=9d72c55d55a61610c7e352024b2b7d0f&chksm=fda20564cad58c724e7b3522e3daf3a457d4c72f3c1928a0802e6b5a8ad8ee42791dd2c27d46&scene=21#wechat_redirect)
- 与简悦联用：[https://mp.weixin.qq.com/s/DtwvTA7dnlUpFBK2sqFTfQ](https://mp.weixin.qq.com/s/DtwvTA7dnlUpFBK2sqFTfQ)（网上有免费教程，去看免费的就好）
- 与MN3联用：[https://mp.weixin.qq.com/s/Fxmv6kYAWuXCARcmInqIoQ](https://mp.weixin.qq.com/s/Fxmv6kYAWuXCARcmInqIoQ)
- 与Notion联用：待更新


## 3.6 多端同步 

- 利用remotely save中的onedrive进行同步，具体可看此推文[最舒服的Obsidian第三方多端同步 (qq.com)](https://mp.weixin.qq.com/s?__biz=MzU4MzgxNjczMA==&mid=2247484853&idx=1&sn=301b7cb8a0c3a75c69bb26cdc5399db5&chksm=fda206c0cad58fd6afa83497ac1f26402818f058eb2165f5f1142ba5df69048cdb9ff6394dde&scene=21#wechat_redirect)
- 利用微力同步：[https://mp.weixin.qq.com/s/1pg6b02di4NhWOFWDR0P3w](https://mp.weixin.qq.com/s/1pg6b02di4NhWOFWDR0P3w)

## 3.7 Obsidian悬浮模式

已装备悬浮编辑系列插件，本人特别喜欢且极力推荐的插件，具体可看下面的推文
- [开启Obsidian的"悬浮"模式，大大提升Ob使用体验 (qq.com)](https://mp.weixin.qq.com/s?__biz=MzU4MzgxNjczMA==&mid=2247485012&idx=1&sn=50e6d3af4a03f7b15f22db8b019efa47&chksm=fda20521cad58c37a3e62559ea068221adcdf4bab332c5ee9189cfc2553377082c1e3c68873c&scene=21#wechat_redirect)
- [Obsidian悬浮系列再添一员，有效提升Ob编辑体验 (qq.com)](https://mp.weixin.qq.com/s?__biz=MzU4MzgxNjczMA==&mid=2247485060&idx=1&sn=a36012899c9e17422fa47d7f0539e14d&chksm=fda205f1cad58ce7e1e11b0d1a5955e7118ef22c7e520583bb443826794e191f8de6137416b7&scene=21#wechat_redirect)

## 3.8 Obsidian表格系列

- 简单表格强推markdown table editor，[开启Obsidian的"悬浮"模式，大大提升Ob使用体验 (qq.com)](https://mp.weixin.qq.com/s?__biz=MzU4MzgxNjczMA==&mid=2247485012&idx=1&sn=50e6d3af4a03f7b15f22db8b019efa47&chksm=fda20521cad58c37a3e62559ea068221adcdf4bab332c5ee9189cfc2553377082c1e3c68873c&scene=21#wechat_redirect)
- 类notion多维表格，强推notion-like-tables，虽然与notion还有差距，但是简单使用已足够，之前有出过推文[Obsidian中的notion表格，真不错！ (qq.com)](https://mp.weixin.qq.com/s?__biz=MzU4MzgxNjczMA==&mid=2247485210&idx=1&sn=e8de03ad36cfca9f4483e910bd7649bf&chksm=fda2046fcad58d79e5de8bb5c87fc4937a5b315db2c50c2a1d60ff9e2ab77f9bd8e386213989&scene=21#wechat_redirect) ，目前更新了多个版本，支持更多单元格类型，支持在实时预览模式编辑
- 对于表格的编辑，可看此推文[Obsidian表格利器 | 添加表题-多级表头-合并单元格-表内多行 (qq.com)](https://mp.weixin.qq.com/s?__biz=MzU4MzgxNjczMA==&mid=2247485033&idx=1&sn=df26bce507ea5e477d757e33245ad7b4&chksm=fda2051ccad58c0aca41d80b160dbadb10d379a91f33deb96a7182a8a2157f700509cc518a63&scene=21#wechat_redirect)
- 还有[未来的Obsidian表格天花板插件 (qq.com)](https://mp.weixin.qq.com/s?__biz=MzU4MzgxNjczMA==&mid=2247485088&idx=1&sn=6cd4729408bae2ad2d07b5123837745d&chksm=fda205d5cad58cc3be45b40ff23469bcf1e13ca0065625b194c9918caaead358241f887d7f9b&scene=21#wechat_redirect)

## 3.9 增强编辑体验

- 增强编辑插件：[Obsidian cMenu插件的必备搭档之增强编辑，提升ob编辑体验感 (qq.com)](https://mp.weixin.qq.com/s/T5_pCSkuld4wVD5q7T1AEw)
- 自动补全：[提升Obsidian编辑体验的自动补全插件 (qq.com)](https://mp.weixin.qq.com/s/b6MPkB4jsc3aTFCMeZ_2Jw)
- 双链伴侣：[Obsidian | Ob双链伴侣，挖出潜藏的笔记双链 (qq.com)](https://mp.weixin.qq.com/s/Ll5Qnyp7dh8AuDGPOoQOEQ)
- 自动添加和去除标题序号：[Obsidian插件介绍二 (qq.com)](https://mp.weixin.qq.com/s/NX15kfve96D_9lVysq1WlA)
- Obsidian分栏：[Obsidian | 人人都会做Obsidian分栏，超级方便，无需CSS代码 (qq.com)](https://mp.weixin.qq.com/s/3rUDKsp4zEBuRHBv2hWLSA)
- 24个技巧：[https://mp.weixin.qq.com/s/0Hcdsr7cY1Tm2ujFty-Jpg](https://mp.weixin.qq.com/s/0Hcdsr7cY1Tm2ujFty-Jpg)

## 3.10 Obsidian发布

发布插件有很多，目前仅推荐最简单的obsius，可看此推文[一键发布Obsidian本地笔记到web！太赞了！ (qq.com)](https://mp.weixin.qq.com/s/09JpeZZOe3jMFTBonEzGsw)


# 📌04 问题解答

如果在使用本库时，大家有什么疑问，建议先在本人微信公众号【维客笔记】中检索相应的关键词，然后逛一逛中文社区或者知乎，若找不到解决办法，可以通过以下渠道反馈：

- 免费渠道（仅解答中文社区、知乎&本人公众号没有出现过的问题）
	- github提issue
	- Ob中文社区
	- 【维客笔记】置顶微博：本库也会挂在置顶微博中，有问题可直接评论，希望不要私信，也许别人也有和你同样的问题，看一下评论就明白了，当然也省去了本人重复解答同一问题的时间
- 付费渠道（有问题均可以提问，不论是基础问题还是之前出现过很多次的问题等）
	- 微信群聊：赞赏本人微信公众号任意一篇推文后，即可在公众号聊天界面申请加入【维客笔记交流群】
		- 目前【维客笔记交流群】共有419人，本群聚焦于讨论与科研学术/效率工具/学习/工作方面相关的话题，几乎无闲聊；不能保证你的每一个问题都能得到满意的回答
		- 看了一下最近一个月的群聊天记录，几乎每天都有讨论，不用担心这是一个僵尸群![image](https://user-images.githubusercontent.com/120721474/208292059-7ce127c6-9259-431b-892c-8e734a25ee65.png)
- 远程协助：如果您实在不想自己搞配置，可以请求本人远程协助，不过也需要付费，费用多少，根据您的需求来定

> Obsidian已经经过了两年多的发展，很多问题，网上都能免费检索到答案，也有很多免费Ob群聊，因此建议大家遇到问题多多利用一下这些免费渠道。本人的付费渠道，我是不推荐的，但如果您实在想节省一些自己的时间和精力，也不差钱，那就消耗一下本人呗🤣~


# 📝05 最后说一下

- 如果你喜欢All in one，此库不适合你
- 需要日程管理，写日记，推荐滴答清单
- 需要思维导图请使用Xmind等专业思维导图软件，将文件以链接的形式添加到Ob中
- 需要看PDF，建议使用pdf exchange，两年前我的一套文献阅读方案，至今仍然在使用，可看此文[文献阅读神器组合 (qq.com)](https://mp.weixin.qq.com/s?__biz=MzU4MzgxNjczMA==&mid=2247483885&idx=1&sn=4d48f377dc8dad530e8c22e205f7d4dc&chksm=fda20298cad58b8ea94e7cf384cdbf1ba40357c99ff6516c8dd5a32575c9cd791b2548179526&scene=21#wechat_redirect)
- 需要word，ppt，excel，那就用微软的三件套即可

>感谢各位软件/插件/主题开发者，提供如此优秀的资源👍👍
