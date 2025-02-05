# 关于OpenAI API申请的实用指南

在课程中，我们介绍了如何使用第三方API，但很多学员也希望申请一个OpenAI的官方账号。尽管演示过程顺利，考虑到不同学员的网络环境差异，以下是一些补充建议。

👉 [WildCard | 一分钟注册，轻松订阅海外线上服务](https://bbtdd.com/WildCard)

## 浏览器设置

首先，确保在隐私模式下操作。不同浏览器有不同的隐私模式名称，例如Edge的InPrivate模式。

![InPrivate模式](https://bbtdd.com/img/6209194779238.webp)

## 网络环境配置

其次，开启全局代理，并选择非大陆地区的网络环境，如英美、新加坡等。某些线路因使用人数过多可能被OpenAI或谷歌邮箱拉黑，此时需要切换线路。更换线路后，请重新打开隐私模式。

如果需要稳定的网络环境，可以考虑使用WildCard提供的服务，它们提供美国家庭的浏览器环境，能够有效避免被拉黑。

👉 [WildCard | 一分钟注册，轻松订阅海外线上服务](https://bbtdd.com/WildCard)

## 谷歌邮箱申请

虽然不是所有人都需要OpenAI账号，但谷歌邮箱确实非常实用。如果你有多年前申请的谷歌账号，那是最理想的。如果没有，需要重新申请。

部分用户在申请过程中无需短信验证，但大多数用户可能需要借助 [https://sms-activate.org/cn](https://sms-activate.org/cn) 进行验证。注册后，建议先用一周（每天登录）确保账号不会被封号后再用于OpenAI注册。

## OpenAI注册

在注册OpenAI时，如果遇到短信验证或绑卡失败，建议更换环境。有用户尝试了7、8次才成功。

短信验证可以选择以下两种方法：

1. 使用 [https://sms-activate.org/cn](https://sms-activate.org/cn)，选择英、美地区的非虚拟手机号。
   ![短信验证](https://bbtdd.com/img/00728122809.webp)
2. 使用WildCard提供的免费短信服务（资源可能有限）。

## OpenAI绑卡付费

绑卡失败通常与网络环境和卡段有关。经过多次测试，我们推荐使用WildCard的虚拟信用卡，因其自动扣费功能更为可靠。WildCard还提供远程环境，能显著提高绑卡成功率。

如果绑卡失败，请联系WildCard客服解决。

👉 [WildCard | 一分钟注册，轻松订阅海外线上服务](https://bbtdd.com/WildCard)

绑卡后，OpenAI会每月根据使用量自动扣费（每月5号出账）。如果扣款失败，请联系发卡商客服解决。如不打算继续使用，建议取消付费计划，避免盗刷。

![取消](https://bbtdd.com/img/04986954819.webp)

## API使用

大部分基于OpenAI API开发的工具默认使用官方API地址 [https://api.openai.com](https://api.openai.com)。然而，此地址对网络环境要求较高。如需为国内用户提供帮助，建议使用第三方服务，他们通常会对国内环境进行优化。如需自建转发服务器，可参考 [https://www.openai-proxy.com](https://www.openai-proxy.com)。

部分应用对API地址有特殊要求，如utools的ChatGPT好友需加上 `/v1/chat/completions`，使用时请留意调整。