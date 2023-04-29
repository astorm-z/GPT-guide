# GPT-guide
> 主要收集了GPT从注册、绑卡到一些热门开源项目的接入，提供比较详细集中的指引（主要for api调用的）

## 更新记录
- 20230427 初版

## 简介
想要玩GPT，需要经过以下的流程：

### 零. 科学上网
下面的一些操作，大部分都需要科学上网，下面需要用到的场景大概有两类:<br>
#### 1. openAI帐号的注册、绑卡<br>
> 要求比较严，需要比较干净的IP，所以有很多机场是用不了的（因为太多人用）
> 建议去azure建一个美国服务器，按量计费的，用远程桌面的方式远程弄，省时省力

#### 2. 调用api<br>
> 要求不高，海外节点大多数都可以
> 这里推荐一个免费的：linux + clash(软件) + glados(获取订阅url)。具体教程写在了本项目子文件夹下的readme了([这里](https://github.com/forczc/GPT-guide/tree/forczc-patch-1/clash))

### 一. 注册openAI帐号
注册只需要一个邮箱+海外手机号，注册完成你将拥有5美元的试用额度，时长3个月，这里是网上搜罗的一份注册教程（[教程[外链]](https://www.pythonthree.com/register-openai-chatgpt/)）

注册完openAI帐号，你将可以：<br>
1. 使用[chatGPT](https://chat.openai.com/chat)（官方网页版），这个是免费的，但由于用得人多，所以很慢，当然你可以开通plus会员（120美元一个月），plus会员仅对官方网页版的chatGPT有用，无关api方式调用<br>
2. 获得openAI的apikey，可以在[这里[外链]](https://platform.openai.com/account/api-keys)创建和生成apikey【别乱泄漏哦】<br>
3. 通过apikey你可以调openAI的api（要钱的），帐号注册送的5美元应该够你用一段时间了<br>

### 二. openAI 绑卡
> 注册完后有5美元其实也够你试玩一下了，但如果你稍微深度一点玩你会发现api调用不稳定，有时候很慢，而且有限额，调没几次就超限，第二天才能用（具体限额规则[官方文档](https://platform.openai.com/docs/guides/rate-limits)有写，当然可能有些隐藏的不为人知的规则）

这是网上搜到的两份绑卡教程，可以参考一下：<br>
1. [OpenAI绑卡教程](https://www.wangpc.cc/aigc/openai-payment-menthonds/)<br>
2. [ChatGPT plus绑卡教程](https://chatgpt-plus.github.io/) <br>

第二份会详细一些，不过是针对ChatGPT plush会员的绑卡，过程是一样的，绑卡的位置不一样。反正可以两份相互参考吧

> PS: <br>
> 1. depay绑卡的话，一般是普通卡，月费1-2美元，对于长期想用的人来说是比较贵的，所以最好的话是升级为"黑卡"<br>
> 2. 升级为黑卡的前提是邀请20个人成功开卡（所以很多人的教程里面的注册链接都是带邀请码的，无可厚非）<br>
> 3. 欧派注册后，充币的话，一般会有24小时-7天不等的冻结时间，冻结期间内不可提现，急用的话可以自行找代充渠道，一般会收手续费<br>
> 4. 虽然注册欧派那些比较麻烦，还要实名，但如果长期想接openai，这还说没法避免的。如果想临时玩玩不想注册欧派，可以邮箱联系我代充，不要手续费，就是需要你用我的depay邀请码注册（我也想要开黑卡哈哈哈），我的邮箱: forczc@foxmail.com <br>

### 三. 有趣的开源项目
有了apikey之后，就可以用自己喜欢的方式去调用api了。但有些人不是开发者，或者懒（比如我），有现成的开源项目可以用的话岂不是很美。以下是搜罗到的个人觉得比较ok的开源项目

#### 1. [Yidadaa/ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)
> 一个调gpt的web项目，有appkey即可用，支持免服务器一键部署自己的网站（就是在vercel免费部署）
> 具体看项目内的readme即可

#### 2. [zhayujie/chatgpt-on-wechat](https://github.com/zhayujie/chatgpt-on-wechat)
> 微信机器人集成gpt和诸多插件，可玩性很强。支持railway一键部署（railway有免费额度）

#### 3. [Significant-Gravitas/Auto-GPT](https://github.com/Significant-Gravitas/Auto-GPT)
> 官方描述"一项使 GPT-4 完全自主的实验性开源尝试。"
> 简单说就是让gpt"自我思考"、"自己提问"，拥有联网搜索能力。目前基于控制台的程序
> 亲测GPT3.5跑不出有什么提高生产力的结果，当然也可能是我提问姿势不对
> 但玩一下还是可以的，目前这个项目快速迭代中，隔几天可能就会变个样
