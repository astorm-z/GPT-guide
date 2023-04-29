# GPT-guide
> 主要收集了GPT从注册、绑卡到一些热门开源项目的接入，提供比较详细集中的指引（主要for api调用的）

## 更新记录
- 20230427 初版

## 简介
想要玩GPT，需要经过以下的流程：

### 零. 科学上网
下面的一些操作，大部分都需要科学上网，下面需要用到的场景大概有两类:
1. openAI帐号的注册、绑卡
`
要求比较严，需要比较干净的IP，所以有很多机场是用不了的（因为太多人用）
建议去azure建一个美国服务器，按量计费的，用远程桌面的方式远程弄，省时省力
`
2. 调用api
`
要求不高，海外节点大多数都可以
这里推荐一个免费的：linux + clash(软件) + glados(获取订阅url)。具体教程写在了本项目子文件夹下的readme了([这里]())
`

### 一. 注册openAI帐号
注册只需要一个邮箱+海外手机号，注册完成你将拥有5美元的试用额度，时长3个月，这里是网上搜罗的一份注册教程（[教程[外链]](https://www.pythonthree.com/register-openai-chatgpt/)）

注册完openAI帐号，你将可以：
1. 使用[chatGPT](https://chat.openai.com/chat)（官方网页版），这个是免费的，但由于用得人多，所以很慢，当然你可以开通plus会员（120美元一个月），plus会员仅对官方网页版的chatGPT有用，无关api方式调用
2. 获得openAI的apikey，可以在[这里[外链]](https://platform.openai.com/account/api-keys)创建和生成apikey【别乱泄漏哦】
3. 通过apikey你可以调openAI的api（要钱的），帐号注册送的5美元应该够你用一段时间了

### 二. openAI 绑卡
注册完后有5美元其实也够你试玩一下了，但如果你稍微深度一点玩你会发现api调用不稳定，有时候很慢，而且有限额，调没几次就超限，第二天才能用（具体限额[官方文档](https://platform.openai.com/docs/guides/rate-limits)有写，当然可能有些隐藏的不为人知的规则）

### 三. 有趣的开源项目
有了apikey之后，就可以用自己喜欢的方式去调用api了。但有些人不是开发者，或者懒（比如我），有现成的开源项目可以用的话岂不是很美。以下是搜罗到的个人觉得比较ok的开源项目

#### 1. [Yidadaa/ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web.git)
> 一个
