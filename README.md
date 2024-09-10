# SteamHostSync
第一次用go写的项目，写的比较烂，欢迎大佬指出错误。

## 1. 实现
对Hosts进行一个新的更  
解决Steam、github访问问题

## 2. 使用方法
## 自动方法(使用工具)
推荐使用Hosts管理工具[SwitchHosts](https://github.com/oldj/SwitchHosts) 
[SwitchHosts备用下载源](https://nas.iaimi.info/s/nT5pb8jMQp32QwB)
### 开机自启动SwitchHosts
win + R 后执行 `shell:startup`    
![](/img/1.png)  
将快捷方式复制进去即可  
![](/img/2.png)  
### 配置SwitchHosts实现自动更新  
可选的URL有:
如果访问不到GitHub可以尝试将`github.com`替换为`hub.fastgit.xyz`(国内镜像)
1. ALL: `https://raw.githubusercontent.com/Clov614/SteamHostSync/main/Hosts`  
2. Steam: `https://raw.githubusercontent.com/Clov614/SteamHostSync/main/Hosts_steam`  
3. github: `https://raw.githubusercontent.com/Clov614/SteamHostSync/main/Hosts_github`    
`镜像地址:`
4. All: `https://raw.sevencdn.com/Clov614/SteamHostSync/main/Hosts`  
5. Steam: `https://raw.sevencdn.com/Clov614/SteamHostSync/main/Hosts_steam`  
6. github: `https://raw.sevencdn.com/Clov614/SteamHostSync/main/Hosts_github`  

![](/img/3.png)

## 手动方式
#### 1. hosts 文件在每个系统的位置不一，详情如下:
- Windows 系统：`C:\Windows\System32\drivers\etc\hosts`
- Linux 系统：`/etc/hosts`
- Mac（苹果电脑）系统：`/etc/hosts`

#### 2. 修改方法
复制下面的内容至hosts尾部(追加在文本末尾)

```
#github Start
140.82.113.26			alive.github.com
140.82.113.25			live.github.com
185.199.108.154			github.githubassets.com
140.82.114.21			central.github.com
185.199.111.133			desktop.githubusercontent.com
185.199.109.153			assets-cdn.github.com
185.199.111.133			camo.githubusercontent.com
185.199.110.133			github.map.fastly.net
151.101.65.194			github.global.ssl.fastly.net
140.82.112.3			gist.github.com
185.199.110.153			github.io
140.82.114.3			github.com
192.0.66.2			github.blog
140.82.113.5			api.github.com
185.199.108.133			raw.githubusercontent.com
185.199.110.133			user-images.githubusercontent.com
185.199.109.133			favicons.githubusercontent.com
185.199.110.133			avatars5.githubusercontent.com
185.199.111.133			avatars4.githubusercontent.com
185.199.111.133			avatars3.githubusercontent.com
185.199.111.133			avatars2.githubusercontent.com
185.199.110.133			avatars1.githubusercontent.com
185.199.110.133			avatars0.githubusercontent.com
185.199.111.133			avatars.githubusercontent.com
140.82.114.10			codeload.github.com
3.5.27.99			github-cloud.s3.amazonaws.com
3.5.28.165			github-com.s3.amazonaws.com
52.216.136.139			github-production-release-asset-2e65be.s3.amazonaws.com
54.231.169.233			github-production-user-asset-6210df.s3.amazonaws.com
52.217.49.20			github-production-repository-file-5c1aeb.s3.amazonaws.com
185.199.111.153			githubstatus.com
140.82.114.18			github.community
52.224.38.193			github.dev
185.199.109.133			media.githubusercontent.com
#github End
# Last Update Time : 2024-09-10 17:51:09 

#steam Start
23.47.27.74			steamcommunity.com
104.94.121.98			www.steamcommunity.com
23.50.124.114			store.steampowered.com
23.47.27.74			api.steampowered.com
23.47.27.74			help.steampowered.com
104.96.221.59			store.akamai.steamstatic.com
23.215.0.136			steamcdn-a.akamaihd.net
104.96.221.59			steamstore-a.akamaihd.net
104.96.221.66			cdn.akamai.steamstatic.com
104.94.121.98			steam-chat.com
104.96.221.66			community.akamai.steamstatic.com
#steam End
# Last Update Time : 2024-09-10 17:51:09 

#Ubisoft_download Start
23.62.160.240			static3.cdn.Ubi.com
23.62.165.107			static2.cdn.Ubi.com
193.108.91.206			static1.cdn.Ubi.com
#Ubisoft_download End
# Last Update Time : 2024-09-10 17:51:09 

#docker Start
141.193.213.20			docker.com
44.193.181.103			hub.docker.com
18.160.10.58			docs.docker.com
104.19.167.24			login.docker.com
34.226.69.105			registry.hub.docker.com
3.224.227.198			docker.io
54.196.99.49			registry-1.docker.io
3.219.239.5			index.docker.io
#docker End
# Last Update Time : 2024-09-10 17:51:09 

#Brave browser Start
3.167.56.82			brave.com
151.101.65.32			laptop-updates.brave.com
#Brave browser End
# Last Update Time : 2024-09-10 17:51:09 

#Tor browser Start
116.202.120.165			www.torproject.org
204.8.99.146			community.torproject.org
204.8.99.146			blog.torproject.org
#Tor browser End
# Last Update Time : 2024-09-10 17:51:10 

#Tails OS Start
204.13.164.63			tails.net
204.13.164.63			download.tails.net
#Tails OS End
# Last Update Time : 2024-09-10 17:51:10 

#Encrypt DNS Start
217.160.156.119			dns.oszx.co
104.21.88.221			0ms.dev
45.90.28.0			anycast.dns.nextdns.io
104.16.132.229			dns.cloudflare.com
146.112.41.2			doh.opendns.com
158.64.1.29			kaitain.restena.lu
137.66.7.89			max.rethinkdns.com
76.76.2.11			freedns.controld.com
149.248.217.117			dns.dnswarden.com
#Encrypt DNS End
# Last Update Time : 2024-09-10 17:51:10 

#EA Start
23.39.184.174			www.ea.com
23.218.216.141			origin-a.akamaihd.net
23.62.165.14			pl.ea.com
23.13.164.104			media.contentapi.ea.com
23.62.165.14			nds-network-nav.ea.com
#EA End
# Last Update Time : 2024-09-10 17:51:10 

#Github: https://github.com/xiulou23/FastHostSync

```

## 激活生效
大部分情况下是直接生效，如未生效可尝试下面的办法，刷新 DNS：
1. Windows：在 CMD 窗口输入：`ipconfig /flushdns`
2. Linux 命令：`sudo nscd restart`
3. Mac 命令：`sudo killall -HUP mDNSResponder`  

## 手动配置Source.yaml文件添加新hosts  
手动下载可执行文件第一次执行后会在目录生成Source.yaml文件，可手动配置。  

```
ua : Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/100.0.4896.127 Safari/537.36
platforms:
  -
    #github :
    - github            #数组的第一个值为对应平台
    - alive.github.com  #后续值为需要解析ip地址的域名
    - live.github.com
    - github.githubassets.com
    - central.github.com
    - desktop.githubusercontent.com
    - assets-cdn.github.com
    - camo.githubusercontent.com
    - github.map.fastly.net
    - github.global.ssl.fastly.net
    - gist.github.com
    - github.io
    - github.com
    - github.blog
    - api.github.com
    - raw.githubusercontent.com
    - user-images.githubusercontent.com
    - favicons.githubusercontent.com
    - avatars5.githubusercontent.com
    - avatars4.githubusercontent.com
    - avatars3.githubusercontent.com
    - avatars2.githubusercontent.com
    - avatars1.githubusercontent.com
    - avatars0.githubusercontent.com
    - avatars.githubusercontent.com
    - codeload.github.com
    - github-cloud.s3.amazonaws.com
    - github-com.s3.amazonaws.com
    - github-production-release-asset-2e65be.s3.amazonaws.com
    - github-production-user-asset-6210df.s3.amazonaws.com
    - github-production-repository-file-5c1aeb.s3.amazonaws.com
    - githubstatus.com
    - github.community
    - github.dev
    - media.githubusercontent.com
  -
    #steam:
    - steam
    - steamcommunity.com
    - www.steamcommunity.com
    - store.steampowered.com
    - api.steampowered.com
    - help.steampowered.com
    - store.akamai.steamstatic.com
    - steamcdn-a.akamaihd.net
    - cdn.akamai.steamstatic.com
    - steam-chat.com
    - community.akamai.steamstatic.com
```
