1CSDN首页
博客
社区
GitCode
猿如意
git
 搜索

会员中心 
消息
历史
创作中心
发布
你所不知道的 GitHub 快捷键及实用技巧

Shang.Liang

于 2022-07-10 08:00:00 发布

1332
 收藏 12
分类专栏： 云原生 文章标签： 云原生 源代码管理 github git
版权

云原生
专栏收录该内容
6 篇文章0 订阅
订阅专栏
目录

一、 搜索

1. 快捷键 S 或 / ， 聚焦搜索栏

2. 高级搜索

2.1 按 star 数查询

2.2 按 fork 数查询

2.3 按 topic 数查询

2.4 按时间查询

2.5 按作者查询

2.6 排除特定内容

二、网页快捷键

1. GitHub 全局快捷键

1.1 快捷键 S 或 / ， 聚焦搜索栏

1.2 快捷键 G + N，跳转到消息页

1.3 快捷键 G + D，调转到首页

1.4 快捷键 ？，打开快捷键帮助弹窗

2. 项目选项卡快捷键

2.1 Code：G + C 

2.2 Issues：G + I

2.3 Pull requests：G + P

2.4 Action： G + A

2.5 Projects：G + B

2.6 Wiki： G + W  

2.7 Security：G + S

3. 项目页面/代码页

3.1 快捷键 W，切换分支

3.2 快捷键 T ，搜索项目内文件

3.3 快捷键 Y，切换文件永久访问地址

3.4 快捷键 L，跳转至代码中的某一个行

3.5 快捷键 B，追溯文件变更记录

4. Issues 页

4.1 快捷键 C，新建 issues

4.2 快捷键 L，按标签过滤

4.3 快捷键 M，按里程碑过滤 

4.4 快捷键 A，按人员过滤

5. CTRL+K / Command + K ，GitHub 命令面板

三、在线 vscode 编辑器打开项目源码

1. 在项目页面单击句号 。 按键

2. 将 github.com 地址改为 github.dev 

一、 搜索
1. 快捷键 S 或 / ， 聚焦搜索栏
2. 高级搜索
2.1 按 star 数查询
stars:>100 匹配 stars 超过 100 的仓库

格式：

stars:>=n  stars 大于等于 n 的仓库

stars:<=n  stars 小于等于 n 的仓库

stars:n..* stars 大于等于 n 的仓库

stars:*..n stars 小于等于 n 的仓库

stars:n..m stars 大于等于 n 小于等于 m 的仓库

2.2 按 fork 数查询
forks:>100 匹配 fork 数超过 100 的仓库

2.3 按 topic 数查询
topics:>=5 匹配有 5 个以上 topic 的仓库

2.4 按时间查询
created:>2022-01-01 创建时间晚于 2022 年 01 月 01 日

pushed:>2022-01-01 推送时间晚于 2022 年 01 月 01 日

updated:>2022-01-01 更新事件晚于 2022 年 01 月 01 日

created:>2022-01-01T12:00:00Z 创建时间晚于 2022-01-01 12:00:00 

created:>2022-01-01T12:00:00+08:00 创建时间晚于 2022-01-01 12:00:00 (UTC 偏移 08:00)

2.5 按作者查询
fullname:zhangsan  全名 zhangsan

location:china  位置 china

followers:>10  10个以上 follower

repos:>10  10个以上公开仓库

2.6 排除特定内容
hello NOT world  匹配含有 hello 字样但不包含 world 字样的仓库

hello -language:java 匹配包含 hello 字样单不是 java 语言编写的仓库

字符串如包含空格，如 spring NOT "hello world" ，匹配有 spring 字样且不含有 "hello world" 字样的仓库

二、网页快捷键
1. GitHub 全局快捷键
1.1 快捷键 S 或 / ， 聚焦搜索栏
1.2 快捷键 G + N，跳转到消息页
1.3 快捷键 G + D，调转到首页
1.4 快捷键 ？，打开快捷键帮助弹窗
2. 项目选项卡快捷键
任意一个项目页面，有如下选项卡，可通过快捷键切换选项卡



G + C 快捷键操作为 按住字母 G 的同时按字母 C ， 同 Ctrl + C，Ctrl + V 为复制粘贴操作一样

2.1 Code：G + C 
2.2 Issues：G + I
2.3 Pull requests：G + P
2.4 Action： G + A
2.5 Projects：G + B
2.6 Wiki： G + W  
2.7 Security：G + S
3. 项目页面/代码页
3.1 快捷键 W，切换分支
点击字母 W 键，弹出分支切换窗口，搜索分支名称回车切换



3.2 快捷键 T ，搜索项目内文件
任意项目 Code 标签页下，单击字母 T 键，进入文件搜索页面，支持按文件名搜索项目内任意文件

↑ ↓ 键选择文件，回车键访问文件内容， esc 退出搜索界面



3.3 快捷键 Y，切换文件永久访问地址
正常我们访问一个文件，地址格式 ：/账号/项目名称/blob/分支/文件.txt ， 如果我们将该地址分享出去后，文件.txt 有新的变动，则通过该地址看到的文件与我们分享出去时的内容就不一致了。

在浏览单个文件页面，单击字母 Y 键，访问地址将会变更为 ：/账号/项目名称/blob/提交ID/文件.txt 格式，此时我们将该地址分享出去后，无论后续 文件.txt 发生任何内容变更，访问它的任何人都将看到与你分享时完全一致的内容。

3.4 快捷键 L，跳转至代码中的某一个行
在某个代码文件访问页面，单击字母 L 键，会弹出一个入口框，输入行号后回切，即可快速跳转到对应代码的行号。

​

3.5 快捷键 B，追溯文件变更记录
在任意文件访问页面，单击字母 B 键 ，跳转到文件追溯视图

​

4. Issues 页
4.1 快捷键 C，新建 issues
4.2 快捷键 L，按标签过滤
​

4.3 快捷键 M，按里程碑过滤 
​

4.4 快捷键 A，按人员过滤
 ​

5. CTRL+K / Command + K ，GitHub 命令面板
不同页面下的命令面板，命令有所不同 

​

​

三、在线 vscode 编辑器打开项目源码
1. 在项目页面单击句号 。 按键
 以 Spring-Boot 项目为例效果如下：

​

2. 将 github.com 地址改为 github.dev 
以 Spring-Boot 项目为例效果如下：

​

文章知识点与官方知识档案匹配，可进一步学习相关知识
云原生入门技能树首页概览9657 人正在系统学习中

显示推荐内容


Shang.Liang
关注

7


12

0

专栏目录
目录
一、 搜索
1. 快捷键 S 或 / ， 聚焦搜索栏
2. 高级搜索
2.1 按 star 数查询
2.2 按 fork 数查询
2.3 按 topic 数查询
2.4 按时间查询
2.5 按作者查询
2.6 排除特定内容
二、网页快捷键
1. GitHub 全局快捷键
1.1 快捷键 S 或 / ， 聚焦搜索栏
1.2 快捷键 G + N，跳转到消息页
1.3 快捷键 G + D，调转到首页
1.4 快捷键 ？，打开快捷键帮助弹窗
2. 项目选项卡快捷键
2.1 Code：G + C 
2.2 Issues：G + I
2.3 Pull requests：G + P
2.4 Action： G + A
2.5 Projects：G + B
2.6 Wiki： G + W  
2.7 Security：G + S
3. 项目页面/代码页
3.1 快捷键 W，切换分支
3.2 快捷键 T ，搜索项目内文件
3.3 快捷键 Y，切换文件永久访问地址
3.4 快捷键 L，跳转至代码中的某一个行
3.5 快捷键 B，追溯文件变更记录
4. Issues 页
4.1 快捷键 C，新建 issues
4.2 快捷键 L，按标签过滤
4.3 快捷键 M，按里程碑过滤 
4.4 快捷键 A，按人员过滤
5. CTRL+K / Command + K ，GitHub 命令面板
三、在线 vscode 编辑器打开项目源码
1. 在项目页面单击句号 。 按键
2. 将 github.com 地址改为 github.dev 

Shang.Liang
码龄11年
 企业员工
44
原创
7万+
周排名
10万+
总排名
4万+
访问

等级
668
积分
672
粉丝
40
获赞
22
评论
123
收藏
签到新秀
签到达人
签到王者
领英
GitHub
脉脉勋章
笔耕不辍
技术圈认证
阅读者勋章
分享小兵
分享达人
持之以恒
勤写标兵
私信
关注


举报
