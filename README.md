Skip to content
Search or jump to…

Pull requests
Issues
Marketplace
Explore
 
@Puzozhitel 
wangziyingwen
/
AutoApi
1
38
Code
Issues
1
Pull requests
Projects
Wiki
Security
Insights
You’re making changes in a project you don’t have write access to. Submitting a change will write it to a new branch in your fork Puzozhitel/AutoApi, so you can send a pull request.
AutoApi
/
README.md
 

Spaces

4

Soft wrap
1
# AutoApi v6.1 (2021-2-10) ———— E5自动续期
2
AutoApi系列：~~AutoApi(v1.0)~~、~~AutoApiSecret(v2.0)~~、~~AutoApiSR(v3.0)~~、~~AutoApiS(v4.0)~~、~~AutoApiP(v5.0)~~
3
​
4
## 说明 ##
5
* E5自动续期程序，但是**不保证续期**
6
* 设置了**周六日(UTC时间)不启动**自动调用，周1-5每6小时自动启动一次 （修改看教程）
7
* 调用api保活：
8
     * 查询系api：onedrive,outkook,notebook,site等
9
     * 创建系api: 自动发送邮件，上传文件，修改excel等
10
     
11
### 相关 ###
12
* AutoApi: https://github.com/wangziyingwen/AutoApi
13
* **错误及解决办法/续期相关知识/更新日志**：https://github.com/wangziyingwen/Autoapi-test
14
   * 大部分错误说明已更新进程序，详细请运行后看action日志报告
15
* 视频教程：
16
   * B站：https://www.bilibili.com/video/BV185411n7Mq/
17
​
18
## 步骤 ##
19
* 准备工具：
20
   * E5开发者账号（**非个人/私人账号**）
21
       * 管理员号 ———— 必选 
22
       * 子号 ———— 可选 （不清楚微软是否会统计子号的活跃度，想弄可选择性补充运行）    
23
   * rclone软件，[下载地址 rclone.org ](https://downloads.rclone.org/v1.53.3/rclone-v1.53.3-windows-amd64.zip)，(windows 64）
24
   * 教程图片看不到请科学上网
25
   
26
* 步骤大纲：
27
   * 微软方面的准备工作 （获取应用id、密码、密钥）
28
   * GIHTHUB方面的准备工作  （获取Github密钥、设置secret）
29
   * 试运行
30
   
31
#### 微软方面的准备工作 ####
32
​
33
* **第一步，注册应用，获取应用id、secret**
34
​
35
    * 1）点击打开[仪表板](https://aad.portal.azure.com/)，左边点击**所有服务**，找到**应用注册**，点击+**新注册**
36
    
37
     ![image](https://github.com/wangziyingwen/ImageHosting/blob/master/AutoApiP/creatapp.png)
38
    
39
    * 2）填入名字，受支持账户类型前三任选，重定向填入 http://localhost:53682/ ，点击**注册**
40
    
41
    ![image](https://github.com/wangziyingwen/ImageHosting/blob/master/AutoApiP/creatapp2.png)
42
    
43
    * 3）复制应用程序（客户端）ID到记事本备用(**获得了应用程序ID**！)，点击左边管理的**证书和密码**，点击+**新客户端密码**，点击添加，复制新客户端密码的**值**保存（**获得了应用程序密码**！）
44
    
45
    ![image](https://github.com/wangziyingwen/ImageHosting/blob/master/AutoApiP/creatapp3.png)
@Puzozhitel
Propose changes
Commit summary
Create README.md
Optional extended description
Add an optional extended description…
 
© 2021 GitHub, Inc.
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
