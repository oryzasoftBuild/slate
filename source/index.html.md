---
title: OryzaConnector Doc

language_tabs:
  

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>

includes:
  

search: true

---
# OryzaConnector安装说明

1         用途
==============

 

该文档详细描述如何安装OryzaConnector并配置客户ERP系统到Oryza
Platform云服务器的链接。

2         前提
==============

2.1   注册公司
--------------

已经在Oryza
Platform上成功的注册了公司，成功收到来自Oryza的确认邮件，邮件中包含了管理员的邮件地址和登录Oryza
Platform的密码。

2.2   下载OryzaConnector
------------------------

成功下载了*OryzaConnector.tar.gz*，Oryza
Platform的确认邮件中包含下载OryzaConnector软件的地址。

2.3   准备一台计算机安装OryzaConnector
--------------------------------------

### 2.3.1  Windows X64或者Linux X64操作系统

支持的操作系统：

-   Windows X64：

Windows7、Windows8、Windows10、Windows Server 2003、Windows Server
2008和Windows Server 2012

-   Linux X64：

Suse、Centos、Redhat、和Ubuntu

-   内存要求：大于等于4G
-   硬盘空间要求：大于等于10G

### 2.3.2  网络要求

-   该计算机可以连接到企业内部SAP系统
-   该计算机可以登录外网的Oryza Platform云平台

3         安装步骤
==================

3.1   Windows系统上安装OryzaConnector
-------------------------------------

目的

使用Windows Command命令行安装OryzaConnector

操作步骤

1.     上传OryzaConnector.tar.gz到的服务器。

2.    
解压缩OryzaConnector.tar.gz，如解压缩到E:\\OryzaConnector，在该文件中包含install.bat和uninstall.bat文件。

3.     使用管理员模式打开Windows command命令窗口

4.     使用下面的命令进入OryzaConnector文件夹：

**`cd OryzaConnector`**

5.     使用下面的命令安装和启动OryzaConnector：

**`Install.bat`**

**注意：**

·        
浏览器会自动启动并打开OryzaConnector，如果没有自动打开，一分钟之后可以在浏览器中输入<http://localhost:9080/OryzaConnector/login>
打开网页

结果

成功安装了OryzaConnector。

3.2   Linux系统安装上OryzaConnector
-----------------------------------

目的

使用Linux命令行安装OryzaConnector。

操作步骤

1.    
使用ftp工具上传OryzaConnector.tar.gz到Linux服务器上的文件夹下，如/user/local

2.     使用下面的命令解压缩OryzaConnector.tar.gz：

**`tar -xzvf OryzaConnector.tar.gz`**

3.     使用下面的命令进入OryzaConnector文件夹：

**`cd OryzaConnector`**

4.     使用下面的命令启动OryzaConnector：

**`sh bin/startup.sh`**

5.     使用下面的命令确认OryzaConnector是否已经启动：

**`ps -elf | grep OryzaConnector`**

结果

成功安装OryzaConnector。

3.3   配置客户源系统和启动OryzaConnector
----------------------------------------

目的

该步骤配置客户源SAP系统信息和启动OryzaConnector。

操作步骤

1.     打开浏览器输入下面地址打开OryzaConnector

http://\<安装OryzaConnector的计算机IP地址\>:9080/OryzaConnector

例如：[http://192.168.101.101:9080/OryzaConnector](http://192.168.101.101:9080/OryzaConnector)

2.     在OryzaConnector初始化登录界面，根据下面表格输入

字段 		| 描述 | 说明
-------------- | -------------- | --------------
组织管理员账号 		|  | 输入申请公司时的邮件地址
密码 				|  | 管理员密码
服务条款和隐私政策 		|  | 必须选中
设置代理 				|  | 如上网需要代理，请选中
代理服务站地址 		|  | 输入代理服务器地址 
端口 				|  | 输入代理服务器地址的端口号码
密码验证 				|  |  如果上网需要密码，请选中
用户名 				|  | 输入用户名
密码 				|  | 输入密码
 

3.     点击***登录按钮*，进入配置源系统页面，根据下面表格输入

字段 		| 描述 | 说明
-------------- | -------------- | --------------
系统类型 		|  | 例如选择SAP ERP
应用程序服务器 |  | 输入SAP服务器地址或者IP地址
系统标识 		|  | 例如输入00
客户端 		|  | 例如输入100 
用户名 		|  | 输入用户名
密码 		|  |  输入密码
语言 		|  | 选择登录SAP的语言，例如选择中文

4.     点击 *下一步***自动连接到Oryza Platform云服务器，可以在页签
*状态* 中查看
连接状态，也可以查看到连接时间、本地计算机地址、源系统信息和代理信息等。

结果

成功配置客户源系统和成功连接到Oryza Platform的云服务器。

接下来打开手机、安装OryzaLink App并执行应用程序[公司初始化]
的来初始化公司。

4         附录
==============

4.1   修改客户ERP配置
---------------------

目的

该步骤修改客户源SAP系统的配置信息

操作步骤

1.    
登入OryzaConnector后***源系统***页签，进入配置源系统页面，根据下面表格输入

字段 		| 描述 | 说明
-------------- | -------------- | --------------
系统类型 		|  | 例如选择SAP ERP
应用程序服务器 |  | 输入SAP服务器地址或者IP地址
系统标识 		|  | 例如输入00
客户端 		|  | 例如输入100 
用户名 		|  | 输入用户名
密码 		|  |  输入密码
语言 		|  | 选择登录SAP的语言，例如选择中文


2.     点击 *更新***更新客户源系统配置信息

结果

成功修改客户源系统的配置信息。

4.2      常见问题解答
---------------------

问题 | 回答 
-------------- | -------------- 
Windows系统下如何停止和删除OryzaConnector | 使用命令uninstall.bat
Linux系统下如何停止和删除OryzaConnector   | 使用命令sh bin/shutdown.sh 

# 测试脚本

# 测试脚本

1           App列表
===================


模块/Module | 应用名称(ZH)	 | App Name(EN)
-------------- | -------------- | --------------
系统管理/Administrator | 	公司初始化 | 	System Initialization
	 | 进程管理 | 	Task manager
	 | 用户管理	 | Users
物料管理/Materials Management | 	采购订单（审批）	 | Purchase Orders(Approve)
	 | 所有采购订单	 | Purchase Orders
	 | 创建采购订单（单项目）	 | Create Purchase Order(OneItem)
	 | 创建采购订单（多项目） | 	Create Purchase Order(MultipleItems)
	 | 采购申请（审批）	 | Purchase Requisitions
	 | 创建采购申请（单项目） | 	Create Purchase Requisition(OneItem)
	 | 创建采购申请（多项目）	 | Create Purchase Requisition(MultipleItems)
人力资源管理/Human Resources	 | 工时维护	 | Timesheet Entry
	 | 工时审批	 | Timesheet Approve
工厂维护/Plant Maintenance | 	维修订单	 | Work Orders
	 | 创建维修订单（单项目）	 | Create Work Order(OneItem)
	 | 创建维修订单（多项目）	 | Create Work Order(MultipleItems)
	 | 设备	 | Equipment
	 | 创建设备	 | Create Equipment
	 | 功能位置	 | Function Locations
	 | 创建功能位置	 | Create Function Locations
销售和分销/Sales and Distribution	 | 销售订单	 | Sales Orders
	 | 创建销售订单（多项目）	 | Create Sales Order(MultipleItems)
	 | 创建销售订单（单项目）	 | Create Sales Order(OneItem)
搜索/Search	 | 搜主数据	 | Search Master Data
	 | 主数据 | 	Master Data
	 | 配置表	 | Configuration table



2           测试App
===================

2.1         采购申请
--------------------

1.       添加应用  *创建采购申请（单项目），*创建一个采购申请

·         物料：R14或者R12；数量：大于2500

2.       记下 采购申请号码

3.       添加应用
 *采购申请（审批），*应用名称：01/EH；选择*审批代码**/**下达组* 01/EH

4.       查找到上面创建的 采购申请号码，点击按钮 *采购申请审批，***检查
*消息*

5.       添加应用
 *采购申请（审批），*应用名称：02/EH；选择*审批代码**/**下达组* 02/EH

6.       查找到上面创建的 采购申请号码，点击按钮 *采购申请审批，***检查
*消息*

7.       添加应用
 *采购申请（审批），*应用名称：03/EH；选择*审批代码**/**下达组* 03/EH

8.       查找到上面创建的 采购申请号码，点击按钮 *采购申请审批，***检查
*消息*

9.       添加应用  *创建采购订单（多项目）*

·         项目编号 00010；物料：R14；数量：大于2500

·         项目编号00020；物料：R15；数量：大于2500

10.    重复上面步骤4、步骤6和步骤8

2.2         采购订单
--------------------

1.       添加应用  *创建采购订单（单项目），*创建一个采购订单

·        
供应商：300007或者300001；物料：R1602；数量：大于100                                                

2.       记下 采购申请号码

3.       添加应用
 *采购订单（审批），*应用名称：01/PH；选择*审批代码**/**下达组* 01/PH

4.       查找到上面创建的 采购申请号码，点击按钮 *采购订单审批，***检查
*消息*

5.       添加应用
 *采购订单（审批），*应用名称：02/PH；选择*审批代码**/**下达组* 02/PH

6.       查找到上面创建的 采购申请号码，点击按钮 *采购订单审批，***检查
*消息*

7.       添加应用
 *采购订单（审批），*应用名称：03/PH；选择*审批代码**/**下达组* 03/PH

8.       查找到上面创建的 采购申请号码，点击按钮 *采购订单审批，***检查
*消息*

9.       添加应用  *创建采购订单（多项目）*

·         供应商：300007或者300001；

·         项目编号 00010；物料：R1602；数量：大于100

·         项目编号00020；物料：R1602；数量：大于100

 

10.    重复上面步骤4、步骤6和步骤8

2.3         工时维护
--------------------

1.       添加应用  *工时维护，*添加一笔工时，查看 *消息*

·         日期：自由选择；小时：1\~8；描述：自由输入

2.       记下 新工时的日期、工时和、描述

3.       修改该工时

4.       删除该工时

5.       再新增一笔工时

6.       添加应用  *工时审批*

7.       查找到上面创建的 工时，点击按钮 *工时审批，***检查 *消息*

2.4         维修订单
--------------------

1.       添加应用  *创建维修订单（单项目），*创建一个维修订单

·         订单描述：自由输入

2.       记下 维修订单号码

3.       添加应用  *维修订单*

4.       查找到上面的维修订单

5.       新增一条
工序0030和一个组件0030（使用该工序0030），选择*修改维修订单*

*6.      **计划维修订单*

*7.      **可用性检查维修订单*

*8.      **下达维修订单*

*9.      **技术关闭维修订单*

10.    添加应用  *创建维修订单（多项目），*再创建一个维修订单

11.    重复上面的步骤2到步骤9

2.5         功能位置
--------------------

1.       添加应用  *创建功能位置，*创建一个功能位置

·         编码：Z001-Z00/Bxxx

·         一般&组织-\>技术对象说明：输入一个地点或者位置信息

2.       记下 功能位置的编码和说明

3.       添加应用  *功能位置*

4.       查找到上面的功能位置

2.6         设备
----------------

1.       添加应用  *创建设备，*创建一个设备

·         编码：大于0000000000200000001小于0000000000299999999

·         一般&组织-\>技术对象说明：输入设备名称

2.       记下 设备的编码和说明

3.       添加应用  *设备*

4.       查找到上面的设备

2.7         销售订单
--------------------

1.       添加应用  *创建销售订单（单项目），*创建一个维修订单，查看
*消息*

客户100002、100003或者100004；物料：H11；数量：大于100\~1000

1.       记下销售订单号码

2.       添加应用  *销售订单，*选择上面使用的客户

3.       查找到上面的销售订单

4.       查找到订单中的客户，查找到该客户地址和电话，并拨打电话

2.8         搜索
----------------

1.       添加应用  *搜主数据，*查找客户 *宇博****的地址和电话*

2.       添加应用  *主数据，*检查所有主数据

3.       添加应用  *配置表，*检查所有配置表

3           测试新注册公司
==========================

3.1         申请公司
--------------------

POST
[http://api.oryzasoft.com/rs/v1/admin/company](http://api.oryzasoft.com/rs/v1/admin/company)                                                     
{                                                                        
                                                                          
   "email": "admin@appxxx.com",                                           
                                                                          
   "name":"apple admin",                                                  
                                                                          
   "companyName": "apple公司"                                             
                                                                          
}

注意：如果用的是无效email的话，需要去dm\_platform-\>dm\_users表查看密码

3.2         登录app
-------------------

1.       手机Chrome浏览器打开mobile.oryzasoft.com

2.       使用上面的email和密码登录

3.       首页面会有下面三个app

a.        公司初始化

b.       进程管理

c.        用户管理

4.       系统会提示设置SAP账号，先不用设定

5.       修改密码

3.3         安装OryzaConnector
------------------------------

1.       启动SAP vm，记录下SAP服务器新获取到的IP地址

2.       解压缩OryzConnector到 本地磁盘，如D:\\OryzaConnector

3.       在管理员模式下运行cmd

4.       执行命令 cd D:\\OryzaConnector

5.       执行命令 install.bat，浏览器会自动打开OryzaConnector的登录界面

a.        登录：上面的email和密码

b.      
设置SAP系统：IP使用vm中的IP，系统标识00，客户端100，用户名TESTER\_ADM，密码Welcome1,语言中文

c.        设置代理： proxy.pvgl.sap.corp 8080

6.       Connector会自动连接上服务器

3.4         公司初始化
----------------------

1.       手机Chrome浏览器打开mobile.oryzasoft.com

2.       打开应用*公司初始化*，按照向导完成6个步骤

3.       打开应用*进程管理*，

a.        可以检查同步的table状态

b.       可以‘重新抽取’

c.        可以修改‘数据同步参数’

d.       可以修改‘定时参数’

3.5         添加用户
--------------------

1.       打开应用*用户管理*，添加用户，如添加：
[tester01@appxxx.com;tester02@appxxx.com](mailto:tester01@appxxx.com;tester02@appxxx.com)

2.       测试删除一个用户

3.       密码需要去dm\_platform-\>dm\_users中查看

4.       使用新用户测试上面的其他所有业务app，新的用户可以使用下面的SAP
user

a.        TESTER01 密码Welcome1

b.       TESTER02 密码Welcome1

c.        TESTER03 密码Welcome1

3.6         测试数据增量同步
----------------------------

1.       SAP系统MM03修改物料CH-100的描述，描述后增加v1，v2的字节

2.       N分钟（N分钟在*进程管理*中的定时参数中设定）去应用*主数据***检查物料描述是否更新