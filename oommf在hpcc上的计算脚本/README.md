###  如何在计算集群上运行脚本

   使用SFTP 登录已经安装配置好的OOMMF环境的远程计算机，   
   上传自己修改后的 .mif OOMMF任务脚本和 .zsub QSUB计算脚本
   进入 工作目录
      $ cd ~/your-workplace-dir/
      $ ls  #查看当前目录下文件
用zsub命令执行计算脚本，此处 zsub 实际上是qsub的变种，各位可以搜索查看相关qsub的使用教程      
      $ zsub your-jobname.zsub

      
###  查看计算任务运行情况

      $ zstat -f
      
   会有如下显示   
      queuename                      qtype resv/used/tot. load_avg arch          states
      #---------------------------------------------------------------------------------
      serial@c0211.local             BI    0/0/16         0.34     linux-x64     
      #---------------------------------------------------------------------------------
      serial@c0212.local             BI    0/0/16         1.33     linux-x64     
      $ 

      
      