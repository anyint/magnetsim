###  如何在计算集群上运行脚本

######   使用SFTP 登录已经安装配置好的OOMMF环境的远程计算机，   
######   上传自己修改后的 .mif OOMMF任务脚本和 .zsub QSUB计算脚本   
######   进入 工作目录   
   
	  $ cd ~/your-workplace-dir/
	  $ ls  #查看当前目录下文件
	
用zsub命令执行计算脚本，此处 zsub 实际上是qsub的变种，各位可以搜索查看相关qsub的使用教程      
      
	$ zsub your-jobname.zsub

      
###  查看计算任务运行情况

	$ zstat -f
      
   会显示任务的编号，运行时间等运行状态

      
      