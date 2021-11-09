## readme
CSS /home/iasf/CSS/product-sns-4.6.6   这个是绿色版的
tomcat 安装在 download 里的那个9.0.54  目录~/Download/apache-tomcat9.0.54
java  是系统自带的
synapp  /home/iasf/synapps/
archiver appliance   /home/iasf/
mysql 用的是downloaded里的那个 的那个里头的。jar文件
mysql 是用yum安装,root密码123456
最后AA的输入命令是这个。
--user=root --password=123456 --database=new

archvier appliance  选择是在/home/iasf/EpicsAA/tomcat_instance
选择的tomcat.jar 是downloaded里
选择的是在mysql_j文件里的  jar文件
需要创建阮连接



css 如果更新java版本后，看打印出的输出，sudo dnf install libcanberra-gtk-module*

tomcat-native 解压缩在/home/iasf/tomcat-native里（解决openssh的问题）
opensh如果说出版本错误，但是实际上版本满足条件，马么可以安装openssh-devel解决问题。
这个有最低版本要求，要求最低1.2.30,这个是1.2.23,太低了
https://www.cnblogs.com/it-bt/p/14864366.html  当时是用这个安装的
不过可以参考别的   https://blog.csdn.net/yeqiyugood/article/details/106060442
这个web后面需要修改catlinash文件，但是我们美妆apache 所以直接修改环境变量，记得source
但是，这一步我还每座，就张昌了




java 17   安装在/USR/jdk-17.0.1里，但是里面没有jre 米有原来环境变量里的一切，后面验证以下。 这个貌似是没有的。

Tomcat    这个电脑使用的是9.0.54
可以打开localhost:8080 即表示ok（即使更新了JAVA版本，重新开关服务即可）
开关服务命令在Apache tomcat的安装目录/bin/start.sh   shutdown.sh

AA如果更新了java的版本,先将sample start 的那个启动脚本的JAVA——HOME 修改一下，如果不幸，再重新用install里面的安装脚本安装

AA如果说启动不了
报错
Unrecognized VM option 'MaxPermSize=128M'
 Cannot create Java VM
那么修改文件，MaxmetaspacemSize=即可



AA answer:
Done with the installation. Please use /home/iasf/EpicsAA/tomcat_instances/sampleStartup.sh to start and stop the appliance and /home/iasf/EpicsAA/tomcat_instances/deployRelease.sh to deploy a new release.




------------------
以上阶段的AA放弃了
参照https://github.com/jeonghanlee/epicsarchiverap-env/blob/master/docs/README.centos8.md
进行下一次的开始
AA那个，参考这个网站 https://blog.csdn.net/weixin_43767046/article/details/112163534
主要的描述是需要修改vim configure/CONFIG_COMMON 里的文件地

mysql
最好用脚本一次性安装，如果重复安装，最好先关服务，
比如先装mysql，没关服务，脚本在安装mairadb 容易出错，部分解决方法：/var/lib/mysql    rm -rf ib_logfile*


css github 安装，执完了第一条命令，但是第二条的出问题了。

## motorsim
/home/iasf/synApps/motor-R7-2-2/modules/motorMotorSim/iocs/motorSimIOC/iocBoot/iocMotorSim
../../bin/linux-x86_64/motorSim st.cmd.unix 





