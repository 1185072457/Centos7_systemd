Unit介绍
==========================

-    Systemctl –t help 查看unit类型
-    Service unit: 文件扩展名为.service, 用于定义系统服务
-    Target unit: 文件扩展名为.target，用于模拟实现运行级别
-    Device unit: .device, 用于定义内核识别的设备
-    Mount unit: .mount, 定义文件系统挂载点
-    Socket unit: .socket, 用于标识进程间通信用的socket文件，也可在系统启动时，延迟启动服务，实现按需启动
-    Snapshot unit: .snapshot, 管理系统快照
-    Swap unit: .swap, 用于标识swap设备
-    Automount unit: .automount，文件系统的自动挂载点
-    Path unit: .path，用于定义文件系统中的一个文件或目录使用,常用于当文件系统变化时，延迟激活服务，如：spool 目录



