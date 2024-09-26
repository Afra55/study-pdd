## 起因

源头还是23年的一篇文章： [深蓝洞察 」2022 年度最“不可赦”漏洞](https://mp.weixin.qq.com/s?__biz=MzkyMjM5MTk3NQ==\&mid=2247484287\&idx=1\&sn=73ebf1ae3aee7bbe1a1e479246fbd7f7\&scene=21#wechat_redirect)。

揭露了P，D，D的一系列[骚操作](https://mp.weixin.qq.com/s/kiLvnJSDZpYRHI_XiUx9gg)（当 App 有了系统权限，真的可以为所欲为？），

其**针对华为、Oppo、Vivo、Xiaomi 等厂商都有专门的处理**。

因此，简单记录了一下，如何基于各类大牛的研究成果，来了解P，D，D代码。

## 下载6.49版本的APK

<https://github.com/androidseclover/pinduoduo-apk>

## 下载所有脱壳后的DEX文件

<https://github.com/davinci1010/pinduoduo_backdoor>

将这些dex重名名，按照序号排在apk已有dex之后，

将这些文件使用zip命令合进apk中方便反解查看：

    zip -m demo.apk classesXX.dex

## 下载脱壳后的部分代码

<https://github.com/elllusion/pinduoduo_backdoor_code?tab=readme-ov-file>

## 分析代码

使用JEB查看apk中的代码。

使用jadx-gui查看脱壳后的class代码。

基本能分析所有的p，d，d骚操作代码了。

