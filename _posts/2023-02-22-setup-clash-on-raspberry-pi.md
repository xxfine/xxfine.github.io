下载 (`arch`查看树莓派架构,对应 armv7 版本)
```
wget https://github.com/Dreamacro/clash/releases/download/v1.13.0/clash-linux-armv7-v1.13.0.gz
gunzip clash-linux-armv7-v1.13.0.gz
mv clash-linux-armv7-v1.13.0 clash
sudo mv clash /usr/local/bin/
sudo chmod a+x /usr/local/bin/clash
```
配置文件
```
wget -O Country.mmdb https://www.sub-speeder.com/client-download/Country.mmdb # 下载全球IP库
wget -O config.yaml [代理商提供的订阅链接] # 下载到本地
```
设置环境变量
```
sudo vi /etc/environment
export http_proxy="http://127.0.0.1:7890"
export https_proxy="http://127.0.0.1:7890"
export no_proxy="localhost, 127.0.0.1, *edu.cn"
```
