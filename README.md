![输入图片说明](doc/logo-banner.png)
<p align="center">
    <img src='https://gitee.com/TDuckApp/tduck-platform/badge/star.svg?theme=dark' alt='star'></img>
    <img src='https://gitee.com/TDuckApp/tduck-platform/badge/fork.svg?theme=dark' alt='fork'></img>
    <img src='https://img.shields.io/github/stars/tduckcloud/tduck-platform?style=social' alt='star'></img>
    <img src='https://img.shields.io/github/forks/tduckcloud/tduck-platform?style=social' alt='fork'></img>
    <img src='https://img.shields.io/badge/TduckSurvey-V5.0-brightgreen' alt='fork'></img>
    <img src='https://img.shields.io/badge/license-MIT%20-orange' alt='fork'></img>
    <br />
    <br />   
    <a href="https://www.tduckcloud.com/" target="_blank">官方网站</a>&nbsp;
    <a href="https://doc.tduckcloud.com"  target="_blank" >部署文档</a>&nbsp;
    <a href="https://gitee.com/TDuckApp/tduck-platform/issues" target="_blank">用户社区</a>&nbsp;
    <a href="https://space.bilibili.com/409825300" target="_blank">Bilibili频道</a>
</p>

<p align="center">
【最新通知-📢】

<p align="center">
如果您不想部署，欢迎品鉴在线产品 <a href="https://nium.top" target="_blank">🔥 Nium牛码二维码</a> 开始探索二维码和表单的新能力。
</p>

**<p align="center">如果您觉得我们的开源项目有帮助，请点击 :star: Star 支持 TDuck 开源团队:heart:</p>**

---


简体中文 |  [English](./README_en.md)


## 一、关于TDuck

TDuck填鸭表单 是国内首批基于Vue开源的问卷/表单收集工具。

系统采用无代码设计理念，使用者可以通过拖拽的方式创建问卷表单，所见即所得；与此同时也支持专业技术人员自行二次开发自定义组件，来满足企不同企业组织的个性化需求。系统采用SpringBoot+Vue+ElementUI技术栈，无需复杂学习即可快速上手，功能强大UI界面清新，通过简要部署就能够助力企业组织快速赋能业务。

2019年一次偶然的启发，我们开始开发 [TDuck填鸭表单社区版](https://demo.tduckapp.com)， 经过了2年的优化沉淀功能趋于稳定；

2021年下半年推出了: [填鸭表单-TDuckPro版](https://pro.tduckcloud.com)；

2023年5月推出: <a href="https://report.tduckcloud.com" target="_blank">TReport可视化大屏</a>；

2023年12月推出: <a href="https://www.tduckcloud.com/x" target="_blank">🔥填鸭表单-TDuckX-Vue3旗舰版</a>；

> ps：问卷系统有3个版本，此处绕不清的友友可以看看 [填表单功能对比](http://https://docs.qq.com/sheet/DSUhoR2pOc2RuZ0Va?tab=BB08J2)

我们一直在寻找一个数据收集后的呈现方案，同时为了方便所有TDuck的使用用户，我们决定在 2024年1月 **全量开源** 大屏产品：<a href="https://gitee.com/TDuckApp/tduck-report-platform" target="_blank">TReport可视化大屏</a>，所有用户都能 **免费** 通过大屏将数据进行快捷呈现！

2024年4月支持表单数据通过WebHook集成至大屏端，实现数据同步：[表单与TReport数据同步教程](https://www.bilibili.com/video/BV1MH4y1K7Xa/)；

2024年5月一次全新的尝试，我们推出 **免费的在线产品**  <a href="https://nium.top" target="_blank">🔥 Nium牛码二维码</a> 开始探索二维码和表单的新能力...

---

### 二、社区活动
社区版表单编辑器暂未开源，该模块通过npm引用，不影响使用、二开其他功能。

可以通过给项目助力，获取社区版最新 **表单编辑器源码**！（限时）

活动参与方式：[点击查看](https://doc.tduckcloud.com/openSource/activity.html)

项目发展离不开您的助力，如有帮助请点亮star

![登录](readmeImages/star.gif)

---

### 三、如何体验及文档
- 查看不同版本的 <a href="http://www.tduckcloud.com" target="_blank">在线体验</a>
- 部署文档、docker快速启动，请查看 <a href="https://doc.tduckcloud.com" target="_blank">项目文档</a>
- 前端项目地址： https://gitee.com/TDuckApp/tduck-front

- 社区版：https://demo.tduckapp.com/home
- 官网：https://www.tduckcloud.com
- 小程序插件：https://doc.tduckcloud.com/functionDesc/uniappDesc.html

### 四、项目部署
> - 部署管理员账号：admin@tduckcloud.com
> - 部署默认密码：123456

#### ①使用docker命令快速启动
```shell
docker run -e SPRING_DATASOURCE_URL="jdbc:mysql://127.0.0.1:3310/tduck-v4?useSSL=false&useUnicode=true&characterEncoding=utf8&serverTimezone=Asia/Shanghai&tinyInt1isBit=false&nullCatalogMeansCurrent=true" -e SPRING_DATASOURCE_USERNAME=root -e SPRING_DATASOURCE_PASSWORD=tduck@tduck -p 8999:8999  -v /upload:/application/BOOT-INF/lib/upload  tduckcloud/tduck-platform
```
#### ②使用docker-compose 部署环境及项目
```shell
1.先安装docker-compose
2.下载tduck源码
3.进入目录下的docker目录 cd docker，执行命令：docker-compose up
4.运行结束 会自动安装mysql以及tduck程序
```
#### ③使用宝塔部署项目
- 部署文档：https://doc.tduckcloud.com/openSource/deploy/openSourceDeploy.html
- 使用指定配置文件：https://doc.tduckcloud.com/openSource/deploy/startByProfile.html

#### ④前后端分离部署
- 部署文档：https://doc.tduckcloud.com/openSource/deploy/fenli.html
- 常见问题：https://doc.tduckcloud.com/openSource/deploy/usualQuestion.html

### 五、关于问题咨询
- 如果您在使用社区版过程中遇到了问题，可在社区查看常见问题或留言进行求助 - [点击进入填鸭问答社区](https://gitee.com/TDuckApp/tduck-platform/issues)
------------------------------

### 六、预览-社区版 - Preview

![登录](readmeImages/screely-1680875090915.png)
![我的项目](readmeImages/screely-1713235168567.png)
![表单设计器](readmeImages/screely-1680873554938.png)
![模板中心](readmeImages/screely-1680874308945.png)
![逻辑设置](readmeImages/screely-1680873488767.png)
![用户管理](readmeImages/screely-1713235303271.png)
![系统配置](readmeImages/screely-1713235232698.png)
![回收设置](readmeImages/screely-1680873612592.png)
![数据详情](readmeImages/screely-1680873703554.png)
![保存模板](readmeImages/screely-1680873844396.png)
![发布表单](readmeImages/screely-1680873661475.png)
![统计概览](readmeImages/screely-1680873817576.png)
![外观设置](readmeImages/screely-1680873577743.png)


### 七、免责声明

**近期我们收到了有关单位的反馈，有用户在使用填鸭表单产品从事非法行为**。

TDUCK填鸭表单一直严格遵守国家相关法律法规，致力于确保平台和用户的安全，为用户提供绿色、安全、健康、便捷的工具。 为此，TDUCK特发表以下优化后的免责声明：

TDUCK填鸭表单仅通过官网tduckcloud.com展示产品信息，并提供官网上介绍的销售联系方式进行直接销售。我们没有授权任何分销商，也没有任何分公司、代理商、办事处、经销商等销售TDUCK旗下的产品。

任何用户不得利用TDUCK的产品从事非法行为，必须合法合规地使用产品。如果我们发现客户在使用产品时存在任何非法行为，**我们将会全力配合有关机关进行调查或向政府部门举报**。TDUCK不承担因客户的非法行为而产生的任何法律责任。

TDUCK填鸭表单不提供任何形式的保证。所有与使用本站相关的资源由客户自行承担直接风险。

TDUCK填鸭表单一直坚持合法合规的开发和销售软件产品。我们诚挚地希望所有用户遵守国家法律法规，在合法的前提下使用我们的产品。

特此声明。


