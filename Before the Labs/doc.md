# Wireshark安装

## 1.资料准备

**资料已经上传，需要自取，[官方下载网站](https://www.wireshark.org/#download)**

![pic1](Labs/picture/doc_picture/pic1.png)

## 2.安装步骤

**双击下载完成的应用**

![pic2](Labs/picture/doc_picture/pic2.png)

**点击Next**

![pic3](Labs/picture/doc_picture/pic3.png)

**点击Noted进入下一步**

![pic4](Labs/picture/doc_picture/pic4.png)

**在这里全部选择，之后点击Next。**

![pic5](C:\Users\Shawn\Desktop\pic\pic5.png)

**这一步也是全部选择，点击Next。**

![pic6](C:\Users\Shawn\Desktop\pic\pic6.png)

**选择安装程序的地址，点击Next。**

![pic7](C:\Users\Shawn\Desktop\pic\pic7.png)

**这一步，勾选的安装可以通过 `wireshark ` 软件分析 `USB` 报文，这里选择安装，点击Next。**

![pic8](C:\Users\Shawn\Desktop\pic\pic8.png)

**这一步开始安装过程，安装过程中会弹出下面界面。**

![pic9](C:\Users\Shawn\Desktop\pic\pic9.png)

点击选择`I Agree`，继续进行安装。**安装到后期阶段会提示安装WinPcap，直接点击下一步默认安装即可。**

![pic10](C:\Users\Shawn\Desktop\pic\pic10.png)

**同时下面会提示USBPcap的安装，勾选上同意协议后点击Next安装。**

![pic11](C:\Users\Shawn\Desktop\pic\pic11.png)

![pic13](C:\Users\Shawn\Desktop\pic\pic13.png)

![pic14](C:\Users\Shawn\Desktop\pic\pic14.png)

**安装完成后点击Next。安装完Wireshark后需要重启。这里第一选项是立即重启，第二选项是稍后重启，根据自己的需求选择重启。**

![pic12](C:\Users\Shawn\Desktop\pic\pic12.png)



# 安装Virtualbox

选择`Virtualbox`原因：1. `Virtualbox`是开源软件，`VMware` 不开源且收费。2. `Virtualbox`对`Linux` 虚拟机字符界面支持较好，`VMware` 对`Linux`虚拟机的字符界面支持很差，比如不能自动调整分辨率。

**[官方下载链接](https://www.virtualbox.org/wiki/Downloads)，选择`Windows hosts` 下载**

![pic15](C:\Users\Shawn\Desktop\pic\pic15.png)

**双击运行 `VirtualBox-6.1.38-153438-Win.exe` 进入安装界面：**

![pic16](C:\Users\Shawn\Desktop\pic\pic16.png)

**选择 VirtualBox Application 并修改安装位置，安装路径最好不要携带中文路径**

![pic17](C:\Users\Shawn\Desktop\pic\pic17.png)

**这里全部勾选**

![pic18](C:\Users\Shawn\Desktop\pic\pic18.png)

**点击是继续安装**

![pic19](C:\Users\Shawn\Desktop\pic\pic19.png)

**点击安装，进入安装程序**

![pic20](C:\Users\Shawn\Desktop\pic\pic20.png)

**这里安装过程中会提醒安装 `Oracle Corporation 通用串行总线控制器`，安装即可，不然后续不能打开 VirtualBox 软件，我这里可能是安装过的原因，没有出现提示。**

![pic22](C:\Users\Shawn\Desktop\pic\pic22.png)

![pic23](C:\Users\Shawn\Desktop\pic\pic23.png)

**安装完成界面**

![pic21](C:\Users\Shawn\Desktop\pic\pic21.png)

## 配置虚拟机默认安装位置

**打开全局设置，配置虚拟机安装地址，默认是存放到 C 盘，这里我改到了`D:\VirtualBox Vms`**

**其他配置按照需求修改![pic25](C:\Users\Shawn\Desktop\pic\pic25.png)**

![pic24](C:\Users\Shawn\Desktop\pic\pic24.png)

**即可，`VirtualBox` 只是一个虚拟机的供应者。**

## 下载Ubuntu镜像

**可以在中科大源下载http://mirrors.ustc.edu.cn/ubuntu-releases/18.04/，选择`ubuntu-18.04.6-desktop-amd64.ios`**

![pic26](C:\Users\Shawn\Desktop\pic\pic26.png)

## 配置虚拟机配置

**打开虚拟机软件`VirtualBox`，点击左上角“新建”按钮。输入虚拟机的名称，选择类型为`Linux`，点击版本下拉选框选择与已经下载的`Ubuntu`镜像对应的版本，64位的就选择`Ubuntu(64-bit)`，32位的就选择`Ubuntu(32-bit)`。点击“下一步”按钮。**

![pic27](C:\Users\Shawn\Desktop\pic\pic27.png)

**之后弹出的对话框中设置为虚拟机分配的内存，最好设置为物理内存的四分之一。我的是16GB内存，就可以给虚拟机分配4GB内存，也就是4096MB。（或者也可根据具体使用来适当增大，不必严格按照四分之一来设定，设定完后不可修改，建议设大些），设置完成之后点击“下一步”按钮。**

![pic28](C:\Users\Shawn\Desktop\pic\pic28.png)

**选择默认的选项“现在创建虚拟硬盘”，点击“创建按钮”，如果想要使用已有的虚拟硬盘文件可以选择第三个选项，选择对应路径的虚拟硬盘文件。**

![pic29](C:\Users\Shawn\Desktop\pic\pic29.png)

**在这一步设置虚拟硬盘的类型，选择默认选项`VDI`就好，然后点击“下一步”。**

![pic30](C:\Users\Shawn\Desktop\pic\pic30.png)

**在这一步设置虚拟硬盘的分配规则，选择动态分配，点击“下一步”。**

![pic31](C:\Users\Shawn\Desktop\pic\pic31.png)

**在这一步设置虚拟硬盘文件的保存位置，以及虚拟硬盘的大小（建议设置160G）。设置完成之后，点击“创建”按钮，进入下一步。**

![pic32](C:\Users\Shawn\Desktop\pic\pic32.png)

**在虚拟机软件的左侧边栏已经出现创建的虚拟机（还没有装系统）。
在虚拟机选项上单击右键，点击“设置”。
点击弹出框左侧的“系统”选项，勾选右侧“网络”，不勾选的话创建的虚拟机不能连接网络!!!!**

![pic34](C:\Users\Shawn\Desktop\pic\pic34.png)

**点击左侧“网络”选项，在右侧的下拉选项中选择“桥接网卡”。点击右下角“ok”按钮，完成并保存对虚拟机系统的设置。**

![pic33](C:\Users\Shawn\Desktop\pic\pic33.png)

**在虚拟机选项上单击鼠标右键，选择“启动”，再选择“正常启动”。**

![pic35](C:\Users\Shawn\Desktop\pic\pic35.png)

**由于没有设置ISO镜像，所以会弹出这样的对话框，点击文件夹图标，然后选择已经下载好的Ubuntu镜像。**

![pic36](C:\Users\Shawn\Desktop\pic\pic36.png)

![pic37](C:\Users\Shawn\Desktop\pic\pic37.png)

**点击选择，之后进行安装**

![pic38](C:\Users\Shawn\Desktop\pic\pic38.png)

![pic39](C:\Users\Shawn\Desktop\pic\pic39.png)

**左边界面选择自己喜欢的语言，点击`Install Ubuntu`开始安装**

![pic40](C:\Users\Shawn\Desktop\pic\pic40.png)

**选择键盘模式，选择喜欢语言即可，点击`Continue`**

![pic41](C:\Users\Shawn\Desktop\pic\pic41.png)

**默认即可，尽量不要选择`Download updates while installing Ubuntu`，这需要消耗很多时间，点击`Continue`。**

![pic42](C:\Users\Shawn\Desktop\pic\pic42.png)

**默认即可，点击`Install Now`**

![pic43](C:\Users\Shawn\Desktop\pic\pic43.png)

**在弹出的界面，点击`Continue`**

![pic44](C:\Users\Shawn\Desktop\pic\pic44.png)

**在地图上找到shanghai，如下图所示，点击`Continue`**

![pic45](C:\Users\Shawn\Desktop\pic\pic45.png)

**设置用户名和密码，点击`Continue`**

![pic46](C:\Users\Shawn\Desktop\pic\pic46.png)

**开始安装,这个过程需要等待好长一段时间**

![pic47](C:\Users\Shawn\Desktop\pic\pic47.png)

**安装完成后，点击`Restart Now`**

![pic48](C:\Users\Shawn\Desktop\pic\pic48.png)

**进入敲击回车进入系统**

![pic49](C:\Users\Shawn\Desktop\pic\pic49.png)

**选择自己设置的账号，并且输入密码**

![pic50](C:\Users\Shawn\Desktop\pic\pic50.png)

**整个安装过程到此完成，开始进入`Ubuntu`系统玩耍吧**

**打开terminal，ping下百度看看是不是网络连接正常**

# 配置dig/iperf3/curl/tc

## dig

**进入terminal界面，输入命令`apt update -y` 更新软件列表。如果没有权限，加入`sudo`进入超级权限**

![pic52](C:\Users\Shawn\Desktop\pic\pic52.png)

**在ubuntu18中，直接有dig，使用命令`dig baidu.com`**

![pic53](C:\Users\Shawn\Desktop\pic\pic53.png)

简明使用，只会输出A记录(写脚本的时候容易获取ip地址)

```javascript
dig jpuyy.com +short
```

只输出mx记录，简明使用

```javascript
dig mx jpuyy.com +short
```

只输出NS记录

```javascript
dig ns jpuyy.com
```

查询SOA( Start of Autority ) 返回主DNS[服务器](https://cloud.tencent.com/product/cvm?from=10680)

```javascript
dig soa jpuyy.com
```

指定dns，例如查询8.8.8.8中的jpuyy.com记录

```javascript
dig +short @8.8.8.8 jpuyy.com
```

大部分的时候dig最下面显示了查询所用的时间及DNS服务器，时间，数据大小。DNS超时时间为30秒，查询时间对于排查DNS问题很有用。

```javascript
;; Query time: 48 msec
;; SERVER: 10.202.72.118#53(10.202.72.118)
;; WHEN: Sun Oct 12 21:41:47 2014
;; MSG SIZE  rcvd: 225
```

DNS的解析是递规解析，那么用dig可以加+trace参数，会显示完整的，无缓存，递规的查询，显示的是完整的trace记录。 可以发现本地DNS(10.202.72.118)返回了根服务器列表，在一台根服务器(199.7.91.13)查到com.的记录，在其中一台com.中查到了jpuyy.com并返回了NS记录，在NS中找到了A记录。

```javascript
dig jpuyy.com +trace

; <<>> DiG 9.8.2rc1-RedHat-9.8.2-0.23.rc1.el6_5.1 <<>> jpuyy.com +trace
;; global options: +cmd
.			493573	IN	NS	i.root-servers.net.
.			493573	IN	NS	e.root-servers.net.
.			493573	IN	NS	k.root-servers.net.
.			493573	IN	NS	c.root-servers.net.
.			493573	IN	NS	f.root-servers.net.
.			493573	IN	NS	d.root-servers.net.
.			493573	IN	NS	m.root-servers.net.
.			493573	IN	NS	j.root-servers.net.
.			493573	IN	NS	g.root-servers.net.
.			493573	IN	NS	b.root-servers.net.
.			493573	IN	NS	h.root-servers.net.
.			493573	IN	NS	a.root-servers.net.
.			493573	IN	NS	l.root-servers.net.
;; Received 496 bytes from 10.202.72.118#53(10.202.72.118) in 1 ms

com.			172800	IN	NS	b.gtld-servers.net.
com.			172800	IN	NS	i.gtld-servers.net.
com.			172800	IN	NS	f.gtld-servers.net.
com.			172800	IN	NS	m.gtld-servers.net.
com.			172800	IN	NS	l.gtld-servers.net.
com.			172800	IN	NS	e.gtld-servers.net.
com.			172800	IN	NS	k.gtld-servers.net.
com.			172800	IN	NS	g.gtld-servers.net.
com.			172800	IN	NS	a.gtld-servers.net.
com.			172800	IN	NS	j.gtld-servers.net.
com.			172800	IN	NS	d.gtld-servers.net.
com.			172800	IN	NS	h.gtld-servers.net.
com.			172800	IN	NS	c.gtld-servers.net.
;; Received 487 bytes from 199.7.91.13#53(199.7.91.13) in 162 ms

jpuyy.com.		172800	IN	NS	f1g1ns1.dnspod.net.
jpuyy.com.		172800	IN	NS	f1g1ns2.dnspod.net.
;; Received 209 bytes from 192.5.6.30#53(192.5.6.30) in 298 ms

jpuyy.com.		600	IN	A	114.215.158.48
;; Received 43 bytes from 112.90.143.29#53(112.90.143.29) in 38 ms
```

服务器上很多时候是双线或三线，如果有智能解析的话要测试从某一个 ip 去请求 dns，加 -b 参数

## iperf3

```
sudo apt-get install iperf3
```

![pic54](C:\Users\Shawn\Desktop\pic\pic54.png)

**iperf3就是一个网络链路质量检测的一个工具。说到网络链路这就涉及到两端，顾名思义就是要部署两台。数据中心A和数据中心B都部署相同版本的iperf3工具，当然也可以使用不同版本的。**

### iperf3命令介绍

```bash
network@iperf:~$ iperf3 -help   #-help查看所有命令集
Usage: iperf [-s|-c host] [options]
       iperf [-h|--help] [-v|--version]

Server or Client:
  -p, --port      #         server port to listen on/connect to
  -f, --format    [kmgKMG]  format to report: Kbits, Mbits, KBytes, MBytes
  -i, --interval  #         seconds between periodic bandwidth reports
  -F, --file name           xmit/recv the specified file
  -A, --affinity n/n,m      set CPU affinity
  -B, --bind      <host>    bind to a specific interface
  -V, --verbose             more detailed output
  -J, --json                output in JSON format
  --logfile f               send output to a log file
  -d, --debug               emit debugging output
  -v, --version             show version information and quit
  -h, --help                show this message and quit
Server specific:
  -s, --server              run in server mode
  -D, --daemon              run the server as a daemon
  -I, --pidfile file        write PID file
  -1, --one-off             handle one client connection then exit
Client specific:
  -c, --client    <host>    run in client mode, connecting to <host>
  -u, --udp                 use UDP rather than TCP
  -b, --bandwidth #[KMG][/#] target bandwidth in bits/sec (0 for unlimited)
                            (default 1 Mbit/sec for UDP, unlimited for TCP)
                            (optional slash and packet count for burst mode)
  -t, --time      #         time in seconds to transmit for (default 10 secs)
  -n, --bytes     #[KMG]    number of bytes to transmit (instead of -t)
  -k, --blockcount #[KMG]   number of blocks (packets) to transmit (instead of -t or -n)
  -l, --len       #[KMG]    length of buffer to read or write
                            (default 128 KB for TCP, 8 KB for UDP)
  --cport         <port>    bind to a specific client port (TCP and UDP, default: ephemeral port)
  -P, --parallel  #         number of parallel client streams to run
  -R, --reverse             run in reverse mode (server sends, client receives)
  -w, --window    #[KMG]    set window size / socket buffer size
  -C, --congestion <algo>   set TCP congestion control algorithm (Linux and FreeBSD only)
  -M, --set-mss   #         set TCP/SCTP maximum segment size (MTU - 40 bytes)
  -N, --no-delay            set TCP/SCTP no delay, disabling Nagle's Algorithm
  -4, --version4            only use IPv4
  -6, --version6            only use IPv6
  -S, --tos N               set the IP 'type of service'
  -L, --flowlabel N         set the IPv6 flow label (only supported on Linux)
  -Z, --zerocopy            use a 'zero copy' method of sending data
  -O, --omit N              omit the first n seconds
  -T, --title str           prefix every output line with this string
  --get-server-output       get results from server
  --udp-counters-64bit      use 64-bit counters in UDP test packets
  --no-fq-socket-pacing     disable fair-queuing based socket pacing
                            (Linux only)
```

## curl

执行命令`sudo apt install curl`

![pic55](C:\Users\Shawn\Desktop\pic\pic55.png)

## tc

**安装brctl命令**

`sudo apt install bridge-utils`

# 安装gcc python3

## gcc

`sudo apt install gcc`

### 查看版本号

`gcc --version`

## python3

`sudo apt install python3`

### 查看版本号

`python3 -V`

# mininet安装

**安装mininet**

```
sudo apt install mininet
```

**查看完成命令**

```
sudo mn
```

**命令**

```
#网络构建启动参数
--topo
--custom
--switch
--controller
--max
#内部交互命令
dump
net
nodes
links
dpctl
iperf
#外部运行参数
-c #清除配置信息
-h #帮助
```

