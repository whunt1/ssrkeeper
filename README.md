# SSR 进程守护
首先 `cd` 到 SSR 安装目录下，执行
```bash
wget -N --no-check-certificate https://raw.githubusercontent.com/whunt1/ssrkeeper/master/runssr.sh && chmod +x runssr.sh && bash runssr.sh
```
正常执行后，运行 `crontab -e` 添加如下定时任务，"/usr/local/shadowsocksr" 为 Shadowsocksr 安装目录   
`* * * * * /bin/bash /usr/local/shadowsocksr/runssr.sh`
