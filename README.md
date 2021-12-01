# windows 10 Penetration Testing Suite Toolkit With Kali Linux inSide

**`2021.12.01补充说明`**

    - 1、系统修改了调用默认cmd为新版terminal，在terminal近期更新后更改了原来的wt.exe的路径，导致.bat文件无法直接打开
         可参照https://www.cnblogs.com/hupo376787/p/14632196.html 修改wt.exe的路径即可正常使用。
    - 2、由于Chrome安装了SwitchyOmega代理插件，导致Acunetix无法打开。
         解决方法为使用SwitchyOmega的直连模式或者系统代理模式即可正常使用。

**`Windows10 渗透测试套件`**

    - 基于Win10 Workstation 21H1 x64 MSDN原版镜像制作
    - 完整安装Kali Linux 2021.2，并配置图形化模式
    - 精简系统自带软件，美化字体及部分图标，适度优化
    - 镜像容量62.4G，使用单磁盘文件存储，提升性能
    - 建议运行环境：
      * vmware：16.0
      * 运行内存：8G
      * 固态硬盘：100G

**`写在前面的话：`**

    1. 所有的安装类软件均下载自软件对应的官方网站。
    2. 所有的绿色类软件均下载自果核剥壳。（https://www.ghxi.com/）
    3. 所有的脚本类工具均下载自github。（https://github.com/）
    4. 部分授权类工具（破解版）及优秀的渗透工具来自微信公众号分享
       * 排名不分先后，有未列举到的请见谅。
         潇湘信安、学蚁致用、谢公子学安全、雾晓安全、无尾熊安全、
         T00ls、渗透攻击红队、零组攻防实验室、洛米唯熊、雷石安全实验室、
         酒仙桥六号部队、InBug实验室、鸿鹄实验室、黑白之道、HACK之道、
         GobySec、Gcow安全团队、Gamma实验室、CobaltStrike实战、冰河技术
    5. 本项目制作的初衷是帮助渗透新手快速搭建工作环境，工欲善其事，必先利其器。
    6. 本项目由于后期调试原因可能会遗留部分本人的信息，请直接忽视。
    7. 本项目坚决不接受也从未曾接受任何形式的赞助。
    
**`免责声明：`**

    本镜像仅面向合法授权的企业安全建设行为，如您需要测试本镜像的可用性，请自行搭建靶机环境。
    在使用本镜像进行检测时，您应确保该行为符合当地的法律法规，并且已经取得了足够的授权。
    如您在使用本镜像的过程中存在任何非法行为，您需自行承担相应后果，作者将不承担任何法律及连带责任。
    
**`软件及工具介绍：`**

**`1. 系统环境类：`**
    
    - Directx
    - Net Framework
    - Visual basic virtual machine     
    - Microsoft C runtime library   
    - Microsoft visual C++ 2005-2019     
    - 集成常用字库

**`2. WindowsApp类：`**

    - 极速pdf
    - kali linux
    - 清理君lite
    - Windows Terminal（已替换默认cmd）

**`3. 其他工具类 （C:\Softwares）：`**

    - aact: 激活工具（一键激活windows & office）
    - bandicam: 视频录制工具（注册版）
    - bandizip: 压缩工具
    - chrome: 92.0 shuax 绿色修改版
      * 主要集成插件:
        - adblock: 广告拦截工具
        - adobe acrobat：pdf工具
        - charset：修改网页编码工具
        - chrome 清理大师: chrome清理工具
        - editthiscookie: cookie编辑工具
        - fofa pro view：fofa工具
        - funnel search：google搜索工具
        - hackbar：hackbar
        - infinity：标签页工具
        - ip address and domain inf: ip&domain探测工具
        - ip whois: whois 探测工具
        - neater bookmarks: 书签管理工具
        - octotree: github资源树查看工具
        - onetab：标签管理工具
        - postwoman：接口调试工具
        - proxy switchyomega：代理切换工具
        - seoquake：网页统计工具
        - supercopy：超级复制
        - toolbox 常用工具: 集成常用小工具
        - wappalyzer：网页技术分析工具
        - whatruns：网页技术分析工具
        - yet another drag and go: 超链接拖拽新窗口打开
    - contextmenumanager：右键菜单管理工具
    - defender：禁用defender工具
    - dism++: 系统调节工具
    - everything: 搜索工具（已禁用windows自带搜索）
    - fdm：下载工具
    - honeyview: 看图工具
    - huorong: 杀毒工具（c:\penetration 为白名单）
    - icon：第三方图标包
    - iobit:
      * uninstaller: 卸载工具（注册版）
      * advanced systemcare: 优化清理工具（注册版）
      * smart defrag: 磁盘碎片整理工具（注册版）
    - mactype：字体管理工具（已修改系统默认字体为Mac苹方体）
    - maye: 快捷启动工具
    - oldnewexplorer: 资源管理器调节工具
    - pcmaster: 系统调整工具
      * 已创建右键快捷菜单：
        - 在此处打开terminal终端
        - 在此处打开kali linux终端
        - 在此处打开notepad
        - 控制面板
        - 计算器
        - 注册表
    - potplayer: 视频播放工具
    - snipaste: 截图工具

**`4. 渗透测试类（C:\Penetration）：`**
    
    - 常用的python及csharp脚本类工具均配有start.bat。
      * 注明工具版本及更新时间
      * 注明依赖环境
      * 注明主要参数
      * 注明简要用法
 
**`[+] AndroidTools 安卓工具:`**
    
    - apktool：apk反编译工具
    - dex2jar：dex打包工具
    - ldplayer：雷电安卓模拟器

**`[+] AntivirusTools 免杀工具：`**
    
    - avevasion：https://github.com/1y0n/av_evasion_tool
    - charlotte：https://github.com/9emin1/charlotte
    - crossnet：https://github.com/dr0op/crossnet-beta
    - darkarmour：https://github.com/bats3c/darkarmour
    - eva2：https://github.com/orca666/eva2
    - foureye：https://github.com/lengjibo/foureye
    - sharperner：https://github.com/aniqfakhrul/sharperner
    - shellcodeloader：https://github.com/knownsec/shellcodeloader
    - shellter：https://github.com/parrotsec/shellter
    - vmprotect: 加壳工具（商业加壳，生成exe体积大）
    - vprotect: 加壳工具（商业加壳，生成exe体积较大）
    
**`[+] ConnectTools 连接工具:`**
    
    - anydesk
    - filezilla
    - finalshell
    - remotedesktopmanager：远程桌面管理工具
    - teamviewer
    - xshellplus

**`[+] CrackTools 破解工具:`**
    
    - accesscrack: access密码破解工具
    - advanced office password recovery: office密码破解工具
    - advanced zip password recovery: zip密码破解工具
    - advanced archive password recovery: zip & rar密码破解工具
    
**`[+] DatabaseTools 数据库工具:`**
    
    - navicat premium: 数据库连接管理工具
    - sharpsqltools：csharp版本mssql管理工具
    - sqlite：sqlite管理工具
    - sqlknife：csharp版本mssql管理工具
    - sqlmap: 注入工具

**` [+] DictionaryTools 字典工具:`**
    
    - fuzzdicts：https://github.com/thekingofduck/fuzzdicts
    - mutoudic：木头字典生成工具（注册版）
    - pentestdicts：https://github.com/ppbibo/pentesterspecialdict

**` [+] DiskTools 磁盘工具:`**
    
    - diskgenius: disk genius 专业版（可恢复硬盘数据）
    - ssdfresh：ssd优化工具

**`[+] EditTools 编辑工具:`**
    
    - 010editor: 十六进制编辑工具（注册版）
    - batchren: 批量重命名工具
    - ctfcrack: 米斯特安全团队工具
    - findstr: 文本检索工具
    - jd-gui: java查看编辑工具
    - jsonview: json查看编辑工具
    - notepad++: 编辑工具
      * 添加右键菜单：使用Notepad编辑
    - rapidenv: 环境变量编辑工具
    - sharpsword：csharp版本word查看工具
    - sublime: 编辑工具（注册版）
      * 添加右键菜单：使用Sublime编辑

**`[+] ExpolitTools 漏洞工具:`**
    
    - cms hunter:https://github.com/SecWiki/CMS-Hunter
    - exphub：https://github.com/zhzyker/exphub
    - middleware-vulnerability-detection：https://github.com/mai-lang-chai/middleware-vulnerability-detection
    - system-vulnerability：https://github.com/mai-lang-chai/system-vulnerability
    - vulmap：web漏扫验证工具（https://github.com/zhzyker/vulmap）
    - vulnerability：https://github.com/edgesecurityteam/vulnerability
    - 更多漏洞exp见 c:\penetration\expolittools

**`[+] IntranetTools 内网工具:`**
    
    - add user: 添加用户工具
    - earth worm: 内网穿透工具
    - frp: 内网穿透工具（https://github.com/fatedier/frp）
    - stowaway：内网穿透工具（https://github.com/ph4ntonn/Stowaway）
    - revsh：内网穿透工具（https://github.com/emptymonkey/revsh）
    - mimikatz：密码抓取工具（文件夹下集成下列密码抓取工具）
      * gosecretsdump
      * hklm
      * kekeo
      * lazagne
      * mimipenguin
      * ntdsdumpex
      * procdump
      * pwdump8
      * quarkspw dump
    - impacket：内网协议工具（https://github.com/SecureAuthCorp/impacket）
    - k8 ladon：内网扫描工具（8.6版本）
    - fscan：内网扫描工具（https://github.com/shadow1ng/fscan）
    - kscan：内网扫描工具（https://github.com/lcvvvv/kscan）
    - darkeye：内网扫描工具（https://github.com/b1gcat/DarkEye）
    - dismap：内网扫描工具（https://github.com/zhzyker/dismap）
    - hydra: 口令爆破工具
    - nc: 监听工具
    - openrdp：开启远程桌面工具
    - regeorg: web流量转发工具（https://github.com/sensepost/reGeorg）
      * neo-regeorg：regeorg改良版（https://github.com/L-codes/Neo-reGeorg）
    - sharpdecryptpwd：密码破解工具
    - wmihacker：wmi渗透工具
    - powershdll：powershell工具
    - invoke-obfuscation：powershell工具（https://github.com/danielbohannon/Invoke-Obfuscation）
    - reverseshell：反弹shell工具
    - 更多内网工具见 C:\Penetration\IntranetTools

**`[+] OfficeTools 办公工具：`**
    
    - office 六件套: （word + excel + powerpoint + access + onenote + outlook）
    - xmind: 思维导图工具
    - telegram: 电报客户端
    - 0-sec documents：零组文档库

**`[+] ProgramTools 编程工具：`**
   
    - elanguage：易语言5.9.2（注册版）
    - java：
      * jre1.8.0：安装版，无需配置环境变量，系统默认调用java8
      * openjdk15.0.2：绿色版，如有特殊软件需要java8以上环境运行可直接调用/bin/java.exe即可
    - microsoft visual studio 2013
    - python2：python2命令启动（python2 test.py）
    - python3：python3命令启动（python3 test.py）
      * 已集成本镜像所有python3工具的pip依赖库
      * 使用pip命令调用python3 pip
    - tdm gcc

**`[+] ReverseTools 逆向工具：`**
    
    - battoexe：bat转exe工具
    - dnspy：csharp逆向工具
    - exescope：exe编辑工具
    - greenhelper：exe绿化工具
    - ollydebug：exe调试工具
    - peidtool：查壳工具
    - signtool：签名伪造工具
    - upxshell：upx加壳工具
    - vbstoexe：vbs转exe工具
    - x64dbg：exe调试工具

**`[+] ScanTools 扫描工具:`**
    
    - acunetix: web vulnerability scanner 14.3.2（注册版）
      * user: admin@awvs.com
      * pass: Admin@awvs.com
    - goby：内网扫描器（已集成插件）
    - router scan: c段扫描工具
    - snet cracker: 弱口令扫描工具
    - scan box:
      * avscan 杀毒软件检测工具：
        - checkav
      * joomscan joomla扫描工具:
        - joomscan-perl: 基于perl
        - joomscan-python: 基于python
      * leakscan 敏感文件扫描工具：	
        - dirmap：https://github.com/H4ckForJob/dirmap
        - dirsearch：https://github.com/maurosoria/dirsearch
        - packerfuzzer：https://github.com/rtcatc/Packer-Fuzzer
        - scantools：https://gitee.com/windyjxx/ScanTools
        - yujian
        - githack
        - ...
      * portscan 端口扫描工具：
        - nmapsingle：nmap单文件版
        - portscan2：端口扫描工具
        - s：端口扫描工具
      * subdomain 子域名探测工具 ：
        - sublist3r：https://github.com/aboul3la/Sublist3r
        - subfinder：https://github.com/projectdiscovery/subfinder
        - oneforall：https://github.com/shmilylty/OneForAll
        - securitytrails
        - webtitle
        - domaininfo
        - webbatchrequest
        - ...
    - 更多扫描工具见 C:\Penetration\ScanTools\ScanBox（其中scanbox项目 https://github.com/we5ter/scanners-box）

**`[+] ShellTools 权限工具:`**
    
    - antsword: 蚁剑（https://github.com/AntSwordProject/AntSword-Loader）
    - behinder: 冰蝎（shell密码统一为cmd）（https://github.com/rebeyond/Behinder）
      * behinder 2.0
      * behinder 3.0 beta11
    - chopper: 菜刀
    - cknife: c刀
    - cobaltstrike: 4.3汉化版
      * 集成插件：
        - adcollection
        - bypassav
        - erebus
        - eval
        - eventlogmaster
        - ladon
        - mikasa
        - taowu
    - godzilla：哥斯拉（密码为哥斯拉默认pass + key）（https://github.com/BeichenDream/Godzilla）
    - kali：kali linux 2021.2
      * 用户：
        - user：kali pass：kali
        - user：root pass：root
      * 修改软件源为阿里云 + 清华大学
      * 完整安装kali linux所有软件包
      * 安装xrdp服务，可用rdp客户端打开kali linux图形化模式
	- kali命令行模式下运行/home/kali/start-xrdp.sh打开xrdp服务，即可使用rdp登录kali
	  rdp配置：127.0.0.1:3390
	- kali命令行模式下运行/home/kali/stop-xrdp.sh关闭xrdp服务
	  如果不需要使用图形化模式，建议关闭xrdp服务（非常占用资源）
    - skyscorpion：天蝎（https://github.com/shack2/skyscorpion）
    - webshellkill: webshell查杀工具
    - shell:免杀一句话木马（密码统一为cmd）
    - webshell: webshell收集项目（https://github.com/tennc/webshell）

**`[+] StegaTools 隐写工具：`**

    - beyond compare：对比工具
    - binwalk：分解工具
    - blind-watermark：盲水印工具
    - crc calculator：校验工具
    - f5：f5隐写工具
      * f5-steganography
      * lsb-steganography
      * steganography
    - foremost：分离工具
    - giftools：gif工具
    - gnuplot：
    - jphs：jpeg工具
    - mp3steno：mp3工具
    - namo gif animator：gif工具
    - openhashtab：hash工具
    - outguess：图片工具
    - pixrecovery：
    - pngcheck：png工具
    - qr_research：二维码工具
    - stegdetect：
    - steghide：捆绑工具
    - stegsolve：分离工具
    - tweakpng：png工具
    - wbstego：
    - ctf密码学知识点总结
    - ctf逆向知识点总结
    - ctf隐写术知识点总结

**`[+] TrafficTools 流量工具:`**

    - besttrace：ip追踪工具
    - burpsuite: 
      * burpsuite 2021.8.2汉化版（https://github.com/funkyoummp/burpsuitecn）
      * burpsuite 2020.11汉化版（https://github.com/funkyoummp/burpsuitecn）
      * 集成插件：
        - vulners scanner
        - changeu
        - chunked coding converter
        - domain hunter
        - fake ip
        - hackbar
        - sqlmap4burp
        - turbo intruder
    - fiddler: 流量抓包工具（汉化版）
    - ftpservers: ftp开启工具  
    - hack firefox: firefox 49.0 （集成插件版）
    - ie tester: ie各版本模拟工具  
    - ipchanger: ip代理工具  
    - nmap：端口扫描工具
    - phpstudy: 集成环境 
      * 集成thinkphp3.1.3 — 5.0.24全部版本
    - proxifier: 流量代理工具  
    - shadowsocks: socks代理工具 
    - torbrowser: 洋葱浏览器
    - wireshark: 流量抓包分析工具
    
**`下载链接：`**

https://pan.xunlei.com/s/VMidP-JSxBLLp54Vh2pGQ88eA1 
提取码：s6qb

**`截图预览：`**

![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/1.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/2.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/3.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/4.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/5.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/6.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/7.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/8.png)

**`壁纸推荐：`**

![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/black_lock.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/black_main.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/blue_lock.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/blue_main.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/kali-windows-red.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/kali-windows-white.png)
