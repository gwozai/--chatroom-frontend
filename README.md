# chatroom-frontend
An anonymous chatroom UI

---

npm install

gulp

(then modify any .js file in /src directory, save changes, and /dist will be created...)



> 本文由 [简悦 SimpRead](http://ksria.com/simpread/) 转码， 原文地址 [ld246.com](https://ld246.com/article/1534741351807?r=icheer)

> 首先访问任意网站，打开浏览器开发者工具 (win 下一般是按 F12，mac 在网页中右键选 “审查元素”)，在 Console 里输入 ↓ var s=document.createElement('sc......

😋 首先访问任意网站，打开浏览器开发者工具 (win 下一般是按 F12，mac 在网页中右键选 “审查元素”)，在 Console 里输入 ↓

```
var s=document.createElement('script');
s.src='//topurl.cn/chat.js';
document.body.append(s);


```

😋 或者，在浏览器地址栏输入 (需要注意, 复制粘贴时 chrome 会吞掉 javascript: 这个头部, 手动敲上即可) ↓

```
javascript:var s=document.createElement('script');s.src='//topurl.cn/chat.js';document.body.append(s);


```

😋 还可以把上面↖️这行代码作为网址**保存成书签**, 添加到书签栏, 进入聊天室更方便

**就能和 <来自同一个域名 && 同样如此操作的> 网友在聊天室里尬聊了...**

![](https://ld246.com/images/img-loading.svg)

* * *

_部分安全防范极高的网站不支持，比如 github，因为他启用了 [CSP （ Content Security Policy ）](https://ld246.com/forward?goto=http%3A%2F%2Fwww.ruanyifeng.com%2Fblog%2F2016%2F09%2Fcsp.html)_

~为了方便您看懂以上操作，还录了一个视频上传 。如果实在嫌麻烦也可以直接访问这个部署过聊天服务的网站，找人尬聊。[topurl.cn](https://ld246.com/forward?goto=http%3A%2F%2Fa.topurl.cn)~

* * *

如何在自己管理的站点植入聊天室？只需在 html 任意位置加入：

```
<script src="//topurl.cn/chat.js" async="async"></script>


```

添加 fold 属性可以让聊天室默认折叠起来：

```
<script src="//topurl.cn/chat.js" async="async" fold></script>


```

* * *

技术栈  
前台: gulp + browserify + babel + jquery-slim  
后台: nodejs + ws + https + node-schedule + psl(用于识别根域名) + axios + 图灵机器人 (tuling123.com)

*   [创造](https://ld246.com/tag/creation)
    
    你创造的作品可能会帮助到很多人，如果是开源项目的话就更赞了！
    
    153 引用 • 898 回帖
    
*   [聊天室](https://ld246.com/tag/%E8%81%8A%E5%A4%A9%E5%AE%A4)

26.5k 147 2.1k 1.7k 1 1.7k 637 196 485 19.4k
