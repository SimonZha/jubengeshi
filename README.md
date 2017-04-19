作者：小丑

日期：2017-02-08

工具：Mou

出处：[打字小丑 jokeright.com](http://www.jokeright.com)

---


# 总述

在剧本写作过程中，为了把尽量多的精力和时间，集中放在内容本身上，而非格式的整理。

因此开发了这个工具，可以将写作完成的文本自动整理成剧本格式。格式比较简单，只针对以下主要内容：

**剧本的五个元素**

- 场景
- 行为
- 角色
- 对白
- 补充说明

*本身这个规范是参考fountain标记语言来设计的，这个语言是好莱坞剧本软件的通用规则，但是由于这门语言大多数并不支持中文，因此我做了一些调整。*

## 场景

场景前后必须有各一个空行,并以【##+空格】开头。

例如

```

## 内 晨 PHIL CONNORS办公室

我们看不到任何人，但是从办公室本身可以看出它的住户，钢人（橄榄球队）鼎盛时期的合影，一个纪念罗伯特·克莱门特的画像，一个艾美奖，一个可擦除的天气图以及一些堆成山的垃圾遍布在桌子上、窗台、和各种能看到的地方。

随着字幕结束，我们注意到沙发上有一个睡着的人，深埋在一堆衣服和偷来的航空毛毯下。

```

## 行为

行为,或场景描述,除了场景、角色、对白、补充说明等元素，都称之为行为元素。段落前后必须各有一个空行，分段由自己来决定。

例如

```
Hawley 追着Phil穿过了第九频道的办公室套间，这是一个典型的大城市新闻制作间。墙上挂着logo标志着这里是WPGH - Pittsburgh。

Phil躲进录制间。
```
ps：在行为段落里，如果某个角色名字在剧本中第一次出现，应该加粗。加粗的格式是：
```
**名字**
```


## 角色/对白/补充说明

角色和对白、补充说明之间没有任何空行。对白紧跟在角色（或补充说明）的下一行。补充说明要用括号括起来。

角色前要有一个空行。

例如

```
PHIL
（睡眼惺忪）
干嘛？

HAWLEY
今天是2月1号，你知道明天是什么日子吗？
```

## 完整示例

> 以下剧本内容是翻译自《土拨鼠日》的开场片段

```
## 内 晨 PHIL CONNORS办公室

我们看不到任何人，但是从办公室本身可以看出它的住户，钢人（橄榄球队）鼎盛时期的合影，一个纪念罗伯特·克莱门特的画像，一个艾美奖，一个可擦除的天气图以及一些堆成山的垃圾遍布在桌子上、窗台、和各种能看到的地方。

随着字幕结束，我们注意到沙发上有一个睡着的人，深埋在一堆衣服和偷来的航空毛毯下。

GIL HAWLEY , Action News的执行制片人，将头探进门。

HAWLEY
我的天呐，Phil

睡觉的人行了过来，朝外看向HAWLEY。

这男人叫Phil，第九频道 Action News 的天气播报员。

PHIL
（睡眼惺忪）
干嘛？

HAWLEY
今天是2月1号，你知道明天是什么日子吗？

Phil站了起来，努力地想。他35岁，挺聪明，脸上有皱纹，看起来长得挺着急，但 是一个有个性的人。

PHIL
（懂了）
不会吧……

他跳了起来，逃出办公室。Hawley在后面追着他。

PHIL
门儿都没有，我才不去。

## 内 晨 走廊

Hawley 追着Phil穿过了第九频道的办公室套间，这是一个典型的大城市新闻制作间。墙上挂着logo标志着这里是WPGH - Pittsburgh。

Phil躲进录制间。

```

# 如何使用

在写剧本的时候，只要按照规则来写即可，实际上，在对白比较多的剧本中，这样的规则能帮你省下不少打冒号的时间。

在写完之后，因为文本本身有特定规则，因此在电脑上可以通过应用程序进行快速排版。


[应用程序：剧本格式整理工具](http://www.jokeright.com/?q=jubengeshi)

以下是我的屏幕截图：

**写作阶段：**

在任何文本处理器中都可以进行，因为是纯文本写作。

![](http://www.jokeright.com/img/script-text.png)

**格式整理之后：**

将文本复制过来，点一个按钮，即可一键整理成标准的剧本格式。

![](http://www.jokeright.com/img/script-format.png)

**PS:程序设计原理**

```
一段的开头关键字为"## "，即两个#+一个空格，则为场景元素。
其他情况:
	如果当前段落前面有空行、后面也有空行，则为行为元素。
	如果当前段落前面有空行、后面没有空行，则为角色元素。
	如果当前段落前面无空行，则为对白元素。补充说明在的格式同对白元素一致（因为文本中已经有括号可以区分开）。
```
