# PythonFTP
2022年8月份接的单子，任务是做一个用Python Socket实现的文件同步工具，本质上就是一个FTP，
同步的思路是创建扫描线程，扫描当前share文件夹下的文件信息，将其与旧信息做一个对称差集，就得到了那些有变化的文件。

支持断点续传功能，实现思路是靠临时文件，只有临时文件写满了才会完成传输。

目前只支持两点之间的同步传输。

曾经这个东西是用来给我实验室的两台机器进行文件共享用的。

可以考虑完善一下，做成多点P2P共享类型。
