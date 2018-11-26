### linux 查询创建时间超过60分钟文件并删除

```sh
find /root/text -type f -name "*.html" -mmin +60 -exec rm  {} \;
```

### 统计文件目录文件数量

```sh
ls -l |grep "^-"|wc -l
```

### 查找指定进程并kill

```sh
ps -ef | grep -v grep | grep "cron"  | cut -c 9-15 | xargs kill -9
```

### 本地复制到远程

```sh
#scp 本地文件 远程ip:远程目录
scp test.txt 127.0.0.1:/home/text.txt
```



