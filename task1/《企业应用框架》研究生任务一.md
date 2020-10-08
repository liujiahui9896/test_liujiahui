#           《企业应用框架》研究生任务一 

1. ##  Git/Github的基本操作

   （1）建立一个Repository ，命名规则 test_姓名拼音（全拼） 

   （2）复制repository的地址，并通过git命令下载到本地 

   （3）在本地添加一个文件 ，并添加一段文字，通过add,commit ,push上传到github.

   步骤已录视频。

   <video src="C:\Users\Qoo\Desktop\企业应用开发框架作业一\任务1.1操作步骤.wmv"></video>

2. ## 安装JDK1.8与IDEA 2019 ，配置Maven，能够运行一个基于Springboot简单的程序。

   ### （1）安装JDK1.8

   ​      1）去Oracle官网下载JDK1.8。

   地址为https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html

   ![image-20201008105704712](img/image-20201008105704712.png)

   选择下图的版本进行下载。

    ![image-20201008105713528](img/image-20201008105713528.png)

   ​    2）下载完后，点击.exe文件，进行安装。因写文档前已安装完，故不再粘贴图片。

   安装后，需要配置环境变量。桌面“我的电脑”右击，选择“属性”打开“系统控制面板”选择“高级系统设置”。

   ![image-20201008105729011](img/image-20201008105729011.png)

      3）配置JAVA_HOME，选择新建，输入变量名和jdk安装路径；

   ![image-20201008105739575](img/image-20201008105739575.png)

   ![image-20201008105748390](img/image-20201008105748390.png)

   ​    4）配置PATH，变量值填写JDK的安装目录下的bin目录。

   ​    5）配置CLASSPATH，变量值填写JDK相关的jar包，也是通过JAVA_HOME变量来设置，可直接写 %JAVA_HOME%\lib\dt.jar;%JAVA_HOME%\lib\tools.jar。

   ### （2）配置Maven

   ​      1）从官网直接下载，地址为：http://maven.apache.org/download.cgi。

   ![image-20201008105758795](img/image-20201008105758795.png)

   ​    2）下载完，解压即可。

   ​    3）解压后，配置环境变量。添加系统变量，变量名为M2_HOME, 变量值为Maven的解压目录。在Path环境变量处，增加新的变量值：%M2_HOME%\bin。

   ![image-20201008105808117](img/image-20201008105808117.png)

   ​    4）在自己选定的位置创建文件夹，作为本地仓库，来存放jar包。

   ![image-20201008105819424](img/image-20201008105819424.png)

   ​    5）用IDEA打开Maven目录下conf下的settings.xml文件，在settings标签下添加本地仓库的绝对路径和增加国内镜像的相关代码。

   ![image-20201008105828534](img/image-20201008105828534.png)

   ### （3）运行一个基于Springboot简单的程序

   ​     1）新建一个project，选择Spring Initializr，选择SDK为1.8，点击Next。

   ![image-20201008105845238](img/image-20201008105845238.png)

   ​     2）进行如下设置，将Java version选择为8，点击Next。

   ![image-20201008105905973](img/image-20201008105905973.png)

   ​     3）选择Web选项后，在选取Spring Web后，点击next。

   ![image-20201008105916986](img/image-20201008105916986.png)

   ​    4）然后在com.example.demo的目录下，添加新的package controller，并添加.java文件helloworld。

   ![image-20201008105924179](img/image-20201008105924179.png)

      5）编写helloworld.java。代码如下

   ![image-20201008105936145](img/image-20201008105936145.png) 

     6）运行项目启动类DemoApplication.java 。

   ![image-20201008105946713](img/image-20201008105946713.png) 

   ​    7）在浏览器中输入http://localhost:8080/hello，即可查看运行结果。

   ![image-20201008105955827](img/image-20201008105955827.png)

3. ## 通过开发环境IDEA配置Git和GitHub，通过IDEA实现仓库的fork,  add，commit, push。

   ## （1）通过开发环境IDEA配置Git和GitHub

   ​       1）在Settings中设置git.exe路径。File-->Settings-->Version Control-->Git/GitHub。

   ​                            ![image-20201008110014610](img/image-20201008110014610.png)

   ​      2）登录Github账户

   ![image-20201008110029159](img/image-20201008110029159.png)

    

   

   ## （2）通过IDEA实现仓库的fork, add,commit,push

    1）fork  

   从GitHub上clone项。点击File ->New->Project from Version Control。然后设置GitHub地址以及存储路径。最后点击Clone。

   ![image-20201008110047301](img/image-20201008110047301.png)

   2）add

      新建两个.java文件（test1.java和test2.java）。添加完后会弹出：

   ![image-20201008110103546](img/image-20201008110103546.png)

    点击add后，两个文件变绿：

   ![image-20201008110110590](img/image-20201008110110590.png)

   3）commit

   提交文件按 VCS-->Git-->Commit Changes。

   ![image-20201008110128190](img/image-20201008110128190.png)

   4）push

   ![image-20201008110134872](img/image-20201008110134872.png)

   点击push。结果如下图，push成功。

   ![image-20201008110142028](img/image-20201008110142028.png)

4. # 学习搭建虚拟机，利用VMWare搭建CentOS环境，能够和Windows机器共享资源，掌握基本命令的使用，能够搭建Docker服务器

   ## （1）利用VMWare搭建CentOS环境，能够和Windows机器共享资源，掌握基本命令的使用。

   1）首先就是下载安装VMWare和下载CentOS，我下载的版本是VMWare15和CentOS7。

   ![image-20201008110207104](img/image-20201008110207104.png)

   2）然后是搭建CentOS环境。点击主页中的“创建新的虚拟机”。

   ![image-20201008110211722](img/image-20201008110211722.png)

   3）选择自定义类型的配置，然后点击下一步。

   ![image-20201008110216605](img/image-20201008110216605.png)

   4）硬件兼容性选择Workstation 15.x，然后点击下一步。

   ![image-20201008110227946](img/image-20201008110227946.png)

   5）选择“稍后安装操作系统”，点击下一步。

   ![image-20201008110233246](img/image-20201008110233246.png)

   6）选择客户机操作系统为“Linux”，版本为“CentOS 7 64 位”。

   ![image-20201008110238572](img/image-20201008110238572.png)

   7）命名虚拟机名称，并选择存放位置。

   ​                                            ![image-20201008110247087](img/image-20201008110247087.png)

   8）进行处理器配置。

   ![image-20201008110324777](img/image-20201008110324777.png)

   9）选择此虚拟机的内存。

   ![image-20201008110331377](img/image-20201008110331377.png)

   10）选择网络类型。

   ![image-20201008110337400](img/image-20201008110337400.png)

   11）选择I/O控制器类型。

   ![image-20201008110344251](img/image-20201008110344251.png)

   12）选择磁盘类型。

   ![image-20201008110349367](img/image-20201008110349367.png)

   13）选择使用的磁盘。

   ​                                             ![image-20201008110355657](img/image-20201008110355657.png)

   14）指定磁盘容量。

   ![image-20201008110408142](img/image-20201008110408142.png)

   15）指定磁盘文件。

   ![image-20201008110414625](img/image-20201008110414625.png)

   16）在虚拟机设置中，选择使用的的ISO映像文件。

   ![image-20201008110420629](img/image-20201008110420629.png)

   ## （2）能够搭建Docker服务器

   1）先使用yum进行简单的安装

   2）修改主机名：

   ![image-20201008110430915](img/image-20201008110430915.png)

   3）使用yum安装 Docker

   ![image-20201008110457119](img/image-20201008110457119.png)

   ![image-20201008110502735](img/image-20201008110502735.png)

   4）鉴于国内网络问题，后续拉取 Docker 镜像十分缓慢，我们可以需要配置加速器来解决，我使用的是阿里的镜像地址：

   ![image-20201008110508837](img/image-20201008110508837.png)

   ![image-20201008110518345](img/image-20201008110518345.png)

   5）启动 Docker 后台服务

   ![image-20201008110526946](img/image-20201008110526946.png)

5. ## 学习MarkDown 文档的使用，建议通过MarkDown整理自己的资料信息，并上传到Github。





