# [首页查询更多项目](https://github.com/GraduationProject-ssm) 包安装运行


# ssm039基于Java的菜匣子优选系统设计与实现+jsp

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV1T48XecE9G?p=38)


# 第一章 绪 论
1.1背景及意义

系统管理也都将通过计算机进行整体智能化操作，对于菜匣子优选生鲜电商系统所牵扯的管理及数据保存都是非常多的，例如管理员；主页、个人中心、用户管理、商品分类管理、商品信息管理、系统管理、订单管理，用户；主页、个人中心、我的收藏管理、订单管理，前台首页；商品信息、新闻资讯、我的、跳转到后台、购物车等，这给管理者的工作带来了巨大的挑战，面对大量的信息，传统的管理系统，都是通过笔记的方式进行详细信息的统计，后来出现电脑，通过电脑输入软件将纸质的信息统计到电脑上，这种方式比较传统，而且想要统计数据信息比较麻烦，还受时间和空间的影响，所以为此开发了菜匣子优选生鲜电商系统；为用户提供了方便管理平台，方便管理员查看及维护，并且可以通过需求进行商品信息内容的编辑及维护等；对于用户而言，可以随时进行查看商品分类和订单信息等，管理员可以足不出户就可以获取到系统的数据信息等，而且还能节省用户很多时间，所以开发菜匣子优选生鲜电商系统给管理者带来了很大的方便，同时也方便管理员对用户信息进行处理。

本论文菜匣子优选生鲜电商系统主要牵扯到的程序，数据库与计算机技术等。覆盖知识面大，可以大大的提高工作人员的效率。

1.2国内外研究概况

随着国内经济形势的不断发展，中国互联网进入了一个难得的高峰发展时期，这使得中外资本家纷纷转向互联网市场。 然而，许多管理领域的不合理结构，人员不足以及市场管理需求的增加使得更多的人具备了互联网管理的意识。

在当今高度发达的信息中，信息管理改革已成为一种更加广泛和全面的趋势。 “菜匣子优选生鲜电商系统”是基于Mysql数据库，在JSP程序设计的基础上实现的。为确保中国经济的持续发展，信息时代日益更新，同时，随着信息社会的快速发展，各种管理系统面临着越来越多的数据需要处理，如何用方便快捷的方式使管理者在广阔的数据海洋里面查询、存储、管理和共享有效的数据信息，对我们的学习，工作和生活具有重要的现实意义。因此，国内外学术界对此进行了深入而广泛的研究，一个新的研究领域——菜匣子优选生鲜电商系统诞生了。

28

1.3 研究的内容

目前许多人仍将传统的纸质工具作为信息管理的主要工具，而网络技术的应用只是起到辅助作用。在对网络工具的认知程度上，较为传统的office软件等仍是人们使用的主要工具，而相对全面且专业的信息管理软件仍没有得到大多数人的了解或认可。本选题则旨在通过标签分类管理等方式，实现菜匣子优选生鲜电商系统的各种功能，从而达到对菜匣子优选生鲜电商系统的管理。

详细内容介绍，将在以下六章中详细阐述：

第一章、绪论，介绍了研究课题选择的背景及意义、研究现状，简要介绍了本文的章节内容。

第二章、引入技术知识，通过引入关键技术进行开发，向系统中涉及直观表达的技术知识。

第三章、重点分析了系统的分析，从系统强大的供需市场出发，对系统开发的可行性，系统流程以及系统性能和功能进行了探讨。

第四章、介绍了系统的详细设计方案，包括系统结构设计和数据库设计。

第五章、系统设计的实现，通过对系统功能设计的详细说明，论证了系统的结构。

第六章、系统的整体测试，评判系统是否可以上线运行。


# 第二章 关键技术的研究
## 2.1 JSP技术介绍
JSP技术本身是一种脚本语言，但它的功能是十分强大的，因为它可以使用所有的JAVA类。当它与JavaBeans 类进行结合时，它可以使显示逻辑和内容分开，这就极大的方便了用户的需求。JavaBeans 可以对JSP技术的程序进行扩展，从而形成新的应用程序，而且JavaBeans的代码可以重复使用，所以就便于对程序进行维护。JavaBean 组件有内部的接口，可以帮助不同的人对系统进行访问。1999年，Sun微系统公司正式推出了JSP技术，这是一种动态技术，是基于整个JAVA体系和JavaServlet提出的，是具有普遍适用性的WEB技术，也是本系统设计的核心技术之一。JSP技术能够极大的提高WEB网页的运行速度。这些内容会与脚本结合，并且由JavaBean和Servlet组件封装。所有的脚本均在服务器端运行，JSP引擎会针对客户端所 提交的申请进行解释，然后生成脚本程序和JSP标识，然后通过HTML/XML页面将结果反馈给浏览器。因此，开发人员亲自设计最终页面的格式和HTML/XML标识时，完全可以使用JSP技术。

所以结合菜匣子优选生鲜电商系统的需求及功能模块的实现，使用JSP技术是最合适的，而且JSP的拓展性比较好，对于系统在后期使用过程中可以不断对系统功能进行拓展，是系统更完成，更方便的满足用户管理。
## 2.2 JAVA简介
Java主要采用CORBA技术和安全模型，可以在互联网应用的数据保护。它还提供了对EJB（Enterprise JavaBeans）的全面支持，java servlet API，JSP（java server pages），和XML技术。JAVA语言是一种面向对象的语言，它通过提供最基本的方法来完成指定的任务，开发者只需要知道一些概念就能够编写出一些应用程序。Java程序相对较小，其代码能够在小机器上运行。Java是一种计算机编程语言，具有封装、继承和多态性三个主要特性，广泛应用于企业Web应用程序开发和移动应用程序开发。

Java语言和一般编译器以及直译的区别在于，Java首先将源代码转换为字节码，然后将其转换为JVM的可执行文件，JVM可以在各种不同的JVM上运行。因此，实现了它的跨平台特性。虽然这使得Java在早期非常缓慢，但是随着Java的开发，它已经得到了改进。
## 2.3 ECLIPSE 开发环境
ECLIPSE 支持广泛、兼容性高并且功能强大，是一个Eclipse 插件集合，普遍适应于JAVA和J2EE的系统开发，支持 JDBC，Hibernate，AJAX，Struts，Java Servlet，Spring，EJB3等市面上存在的几乎所有数据库链接工具和主流Eclipse产品 开发工具。 

ECLIPSE 在业内是所熟知的开发工具，该平台在开发的过程中运用的就是该工具。ECLIPSE 又被称之为企业级的工作平台，它是以Eclipse IDE为基础的。ECLIPSE 可以帮助我们进行数据库的研发和J2EE的使用，除此之外，还可以提高系统的运营能力，这突出表现在服务器的整合过程中。ECLIPSE 的功能相当完备，能够为J2EE的集成提供必要的环境支持，从而完成编码、测试、调试及发布等功能。它可以支持JSP，HTML，SQL，Javascript，Struts， CSS等。
## 2.4 Tomcat服务器
Tomcat属于一种轻型的服务器，所以说在中小企业中并不具有普适性。但是当程序员需要开发或调试JSP 程序时，则通常会将该服务器作为首选。对于一个仅具有计算机基础知识的人来说，计算机系统具有一个好的Apache服务器，可以很好的对HTML 页面进行访问。Tomcat 虽然是Apache的扩展，但是它们都是可以独立运行的，二者是不互相干扰的。当配置正确的时候，Apache服务器为HTML 页面的运行提供技术支持，Tomcat 的任务则是运行Servle和JSP 页面。Tomca也具有一定的HTML页面处理功能。
## 2.5 MySQL数据库
数据库是系统开发过程中不可或缺的一部分。在WEB应用方面，MySQL AB开发了一个具有很大优势的MySQL关系数据库管理系统。 MySQL可以将数据存储在不同的表中，这非常灵活，并且还可以提高系统在实际应用中的速度。数据库访问最常用于标准SQL语言，MySQL用于SQL语言，因此它具有高度兼容性。数据库的操作是必不可少的，包括对数据库表的增加、删除、修改、查询等功能。现如今，数据库可以分为关系型数据库和非关系型数据库，Mysql属于关系性数据库，Mysql数据库是一款小型的关系型数据库，它以其自身特点：体积小、速度快、成本低等，Mysql数据库是目前最受欢迎的开源数据库。

在WEB应用技术中， Mysql数据库支持不同的操作系统平台，虽然在不同平台下的安装和配置都不相同，但是差别也不是很大，Mysql在Windows平台下两种安装方式，二进制版和免安装版。安装完Mysql数据库之后，需要启动服务进程，相应的客户端就可以连接数据库，客户端可通过命令行或者图形界面工具登录数据库。


# 第三章 系统分析
## 3.1 系统设计目标
菜匣子优选生鲜电商系统主要是为了用户方便对商品信息的了解以及查看商品分类和查看订单信息，也是为了更好的让管理员进行更好存储所有数据信息及快速方便的检索功能，对系统的各个模块是通过许多今天的发达系统做出合理的分析来确定考虑用户的可操作性，遵循开发的系统优化的原则，经过全面的调查和研究。

系统所要实现的功能分析，对于现在网络方便的管理，根据自己的需求可以进行查看商品信息、新闻资讯、我的、跳转到后台、购物车等，这样既能节省用户的时间，不用在像传统的方式，需要查询，由于很多用户的时间原因，没有办法去相关实体店了解信息，真的很难去满足用户的各种需求。所以菜匣子优选生鲜电商系统的开发不仅仅是能满足用户的需求，还能提高管理员的工作效率，减少原有不必要的工作量。
## 3.2 系统可行性分析
系统的开发环境和配置都是可以自行安装的，系统使用JSP开发工具，使用比较成熟的Mysql数据库进行对系统用户和管理员之间相关的数据交互，根据技术语言对数据库，结合需求进行修改维护，可以使得系统运行更具有稳定性和安全性，从而完成实现系统的开发。

（1）硬件可行性分析

菜匣子优选生鲜电商系统及信息分析的设计对于所使用的计算机没有什么硬性的要求，计算机只要可以正常的使用进行代码的编写及页面设计就可行，主要是对于服务器有些要求，对于平台搭建完成要上传的服务器是有一定的要求的，服务器必须选择安全性比较高的，然后就是在打开系统必须顺畅，不能停顿太长时间；性价比高；安全性高。

（2）软件可行性分析

开发整个系统使用的是云计算，流量的可扩展性和基于流量的智能调整云计算的优点就是流量的可扩展性和基于流量的智能调整，保障系统的安全及数据信息的及时备份。

因此，我们从两个方面进行了可行性研究，可以看出系统的开发没有问题。
## 3.3 系统功能分析和描述
使用菜匣子优选生鲜电商系统的用户分管理员和用户两个角色的权限子模块。

管理员所能使用的功能主要有：主页、个人中心、用户管理、商品分类管理、商品信息管理、系统管理、订单管理等。

用户可以实现主页、个人中心、我的收藏管理、订单管理等。

前台首页可以实现商品信息、新闻资讯、我的、跳转到后台、购物车等。

## 3.4系统UML用例分析
### 3.4.1管理员用例
管理员登录后可进行主页、个人中心、用户管理、商品分类管理、商品信息管理、系统管理、订单管理，管理员的用例如图3-1所示。

![](/md/blog.002.png)

图3-1 管理员用例图
### 3.4.2用户用例
用户注册登录后可进行主页、个人中心、我的收藏管理、订单管理，用户用例如图3-2所示。

![](/md/blog.003.png)

图3-2 用户用例图
## 3.5系统流程分析
### 3.5.2添加信息流程
添加信息,编号系统使用自动编号模式,没有用户填写,用户添加信息输入信息,系统将自动确认的信息和数据,验证的成功是有效的信息添加到数据库,信息无效,重新输入信息。添加信息流程如图3-4所示。

![](/md/blog.004.png)

图3-4 添加信息流程图
### 3.5.1操作流程
用户想进入系统，首先进入系统登录界面，通过正确的用户名、密码，选择登录类型登录，系统会检查登录信息，信息正确，然后输入相应的功能界面，提示信息错误，登录失败。系统操作流程如图3-3所示。

![](/md/blog.005.png)

图3-3操作流程图
### 3.5.3删除信息流程
用户选择要删除的信息并单击Delete按钮。系统提示是否删除信息。如果用户想要删除信息，系统将删除信息。系统数据库删除信息。删除信息流程图如图3-5所示。

![](/md/blog.006.png)

图3-5 删除信息流程图


# 第四章 系统设计
## 4.1 系统体系结构
菜匣子优选生鲜电商系统的结构图4-1所示：

网

络

用户

服务器和程序

管理员

![](/md/blog.007.png)

图4-1  系统结构

模块包括主界面，主页、个人中心、用户管理、商品分类管理、商品信息管理、系统管理、订单管理等进行相应的操作。

登录系统结构图，如图4-2所示：

Y

菜匣子优选生鲜电商系统登录界面

用户登录

密码正确

管理员界面

用户界面

![](/md/blog.008.png)

图4-2 登录结构图

这些功能可以充分满足菜匣子优选生鲜电商系统的需求。此系统功能较为全面如下图系统功能结构如图4-4所示。

![](/md/blog.009.png)

图4-4系统功能结构图

## 4.2 数据库设计原则
每个数据库的应用它们都是和区分开的，当运行到一定的程序当中，它就会与自己相关的协议与客户端进行通讯。那么这个系统就会对使这些数据进行连接。当我们选择哪个桥段的时候，接下来就会简单的叙述这个数据库是如何来创建的。当点击完成按钮的时候就会自动在对话框内弹出数据源的名称，在进行点击下一步即可，直接在输入相对应的身份验证和登录密码。 

商品信息实体E-R图，如图4.6所示。

![](/md/blog.010.png)

`    `图4.6商品信息E-R图

用户信息E-R图，如图4.7所示。

![](/md/blog.011.png)

图4.7用户信息E-R图

## 4.3 数据表
将数据库概念设计的E-R图转换为关系数据库。在关系数据库中，数据关系由数据表组成，但是表的结构表现在表的字段上。

表名：shangpinfenlei

功能：商品分类

|字段名称|类型|长度|字段说明|主键|默认值|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|bigint||主键|主键||
|addtime|timestamp||创建时间||CURRENT\_TIMESTAMP|
|shangpinfenlei|varchar|200|商品分类|||




表名：shangpinxinxi

功能：商品信息

|字段名称|类型|长度|字段说明|主键|默认值|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|bigint||主键|主键||
|addtime|timestamp||创建时间||CURRENT\_TIMESTAMP|
|shangpinbianhao|varchar|200|商品编号|||
|shangpinmingcheng|varchar|200|商品名称|||
|shangpinfenlei|varchar|200|商品分类|||
|shuliang|varchar|200|数量|||
|pinpai|varchar|200|品牌|||
|guige|varchar|200|规格|||
|xiangqing|varchar|200|详情|||
|fengmian|varchar|200|封面|||



表名：yonghu

功能：用户

|字段名称|类型|长度|字段说明|主键|默认值|
| :-: | :-: | :-: | :-: | :-: | :-: |
|id|bigint||主键|主键||
|addtime|timestamp||创建时间||CURRENT\_TIMESTAMP|
|yonghuzhanghao|varchar|200|用户账号|||
|yonghuxingming|varchar|200|用户姓名|||
|mima|varchar|200|密码|||
|xingbie|varchar|200|性别|||
|lianxidianhua|varchar|200|联系电话|||
|dianziyouxiang|longtext|4294967295|电子邮箱|||



# 第五章 系统实现


## 5.1管理员功能模块
##
管理员通过用户名和密码填写完成后进行登录，如图5-6所示。管理员登录成功后进入到系统操作界面，可以对主页、个人中心、用户管理、商品分类管理、商品信息管理、系统管理、订单管理等功能模块进行相对应操作。

个人中心：通过列表可以获取原密码、新密码、确认密码等内容，可以进行修改或删除操作，如图5-7所示。

![](/md/blog.012.png)

图5-6管理员登录页面

![](/md/blog.013.png)

图5-7个人中心页面

个人信息：通过列表可以获取用户名等信息，进行删除或修改操作，如图5-8所示。


![](/md/blog.014.png)

图5-8个人信息界面图

用户管理：通过列表可以获取用户账号、用户姓名、密码、性别、联系电话、电子邮箱、余额、积分等信息，进行修改或删除操作，如图5-9所示。

![](/md/blog.015.png)

图5-9用户管理界面图 

商品分类管理：通过列表可以获取商品分类等信息，进行修改或删除操作，如图5-10所示。

![](/md/blog.016.png)

图5-10商品分类管理界面图

商品信息管理：管理员通过列表可以获取商品编号、商品名称、商品分类、数量、品牌、规格、封面、价格、详情等信息，进行修改或删除操作，如图5-11所示。

![](/md/blog.017.png)

图5-11商品信息管理界面图

轮播图；该页面为轮播图管理界面。管理员可以在此页面进行首页轮播图的管理，通过新建操作可在轮播图中加入新的图片，还可以对以上传的图片进行修改操作，以及图片的删除操作，如图5-12所示。

![](/md/blog.018.png)

图5-12轮播图管理界面图

新闻资讯：管理员通过列表可以获取标题、图片、内容等信息，进行修改或删除操作，如图5-13所示。

![](/md/blog.019.png)

图5-13新闻资讯界面图

已完成订单：管理员通过列表可以获取订单id、用户id、商品id、商品名称、商品图片、购买数量、价格/积分、折扣价格、总价格/总积分、折扣总价格、支付类型、状态、地址等信息，进行修改或删除操作，如图5-14所示。

![](/md/blog.020.png)

图5-14已完成订单界面图

已支付订单列表：管理员通过列表可以获取订单id、用户id、商品id、商品名称、商品图片、购买数量、价格/积分、折扣价格、总价格/总积分、折扣总价格、支付类型、

状态、地址等信息，进行修改或删除操作，如图5-15所示。

![](/md/blog.021.png)

图5-15已支付订单列表界面图

已完成订单列表：管理员通过列表可以获取订单id、用户id、商品id、商品名称、商品图片、购买数量、价格/积分、折扣价格、总价格/总积分、折扣总价格、支付类型、

状态、地址等信息，进行修改或删除操作，如图5-16所示。

![](/md/blog.022.png)

图5-16已完成订单列表界面图

## 5.3前台首页功能模块
` `菜匣子优选生鲜电商系统，在菜匣子优选生鲜电商系统可以查看商品信息、新闻资讯、我的、跳转到后台、购物车等内容，如图5-17所示。

![](/md/blog.023.png)

图5-17系统首页界面图

登录、注册，通过注册填写用户账号、用户姓名、密码、联系电话、电子邮箱等信息进行注册操作，如图5-18所示。

![](/md/blog.024.png)

![](/md/blog.025.png)

图5-18登录、注册界面图

商品信息，在商品信息页面可以查看商品编号、价格、数量、品牌、规格等信息进行立即购买，如图5-19所示。 

图5-19商品信息界面图

个人中心，在个人中心页面可以查看用户账号、用户姓名、密码、性别、联系电话、电子邮箱等如图5-20所示。

![](/md/blog.026.png)

图5-20个人中心界面图

收货地址添加，在收货地址添加页面可以查看个人中心、我的订单、我的地址、我的收藏等如图5-21所示。

![](/md/blog.027.png)

图5-21收货地址添加界面图


确认下单，在确认下单页面可以查看选择收货地址、清单列表等信息进行支付如图5-22所示。

![](/md/blog.028.png)

图5-22确认下单界面图






















