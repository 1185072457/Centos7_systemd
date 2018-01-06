================
CentOS7启动
================

POST --> Boot Sequence --> Bootloader --> kernel +initramfs(initrd) --> rootfs --> /sbin/init
    init - CentOS 5: SysV init
         - CentOS 6: Upstart
         - CentOS 7: Systemd

Systemd：系统启动和服务器守护进程管理器，负责在系统启动或运行时，激活系统资源，服务器进程和其它进程

Systemd新特性:

- 系统引导时实现服务并行启动
- 按需启动守护进程
- 自动化的服务依赖关系管理 
- 同时采用socket式与D-Bus总线式激活服务 
- 系统状态快照

配置文件：
    /usr/lib/systemd/system:每个服务最主要的启动脚本设置，类似于之前的/etc/init.d/
    /run/systemd/system：系统执行过程中所产生的服务脚本，比上面目录优先运行
    /etc/systemd/system：管理员建立的执行脚本，类似于/etc/rc.d/rcN.d/Sxx类的功能，比上面目录优先运行