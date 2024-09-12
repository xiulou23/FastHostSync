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
140.82.114.26			alive.github.com
185.199.111.154			docs.github.com
140.82.113.26			live.github.com
140.82.112.13			uploads.github.com
185.199.111.153			training.github.com
185.199.111.133			objects.githubusercontent.com
185.199.110.153			metamask.github.io
185.199.111.153			pages.github.com
13.107.42.16			pipelines.actions.githubusercontent.com
185.199.108.153			customer-stories-feed.github.com
185.199.109.154			github.githubassets.com
140.82.114.21			central.github.com
140.82.114.22			viewscreen.githubusercontent.com
185.199.108.133			desktop.githubusercontent.com
185.199.109.133			raw.github.com
185.199.110.133			repository-images.githubusercontent.com
185.199.109.153			assets-cdn.github.com
185.199.110.133			github.map.fastly.net
3.5.27.73			github-production-release-asset-2e65be.s3.amazonaws.com
52.217.175.9			github-production-repository-file-5c1aeb.s3.amazonaws.com
52.217.204.129			github-production-user-asset-6210df.s3.amazonaws.com
185.199.109.133			camo.githubusercontent.com
185.199.108.133			github.map.fastly.net
151.101.193.194			github.global.ssl.fastly.net
185.199.108.133			gist.githubusercontent.com
140.82.112.30			githubapp.com
192.0.66.2			github.blog
54.231.133.41			github-cloud.s3.amazonaws.com
185.199.109.153			githubstatus.com
185.199.109.153			guides.github.com
140.82.114.17			help.github.com
140.82.112.17			github.community
140.82.112.3			gist.github.com
185.199.111.153			github.io
140.82.112.4			github.com
192.0.66.2			github.blog
140.82.114.6			api.github.com
185.199.109.133			raw.githubusercontent.com
185.199.108.153			archiveprogram.github.com
185.199.110.153			assets-cdn.github.com
185.199.111.133			user-images.githubusercontent.com
185.199.110.133			favicons.githubusercontent.com
185.199.109.133			avatars5.githubusercontent.com
185.199.111.133			avatars4.githubusercontent.com
185.199.111.133			avatars3.githubusercontent.com
185.199.110.133			avatars2.githubusercontent.com
185.199.108.133			avatars6.githubusercontent.com
185.199.109.133			avatars7.githubusercontent.com
185.199.110.133			avatars8.githubusercontent.com
185.199.108.133			avatars1.githubusercontent.com
185.199.109.133			avatars0.githubusercontent.com
185.199.109.133			avatars.githubusercontent.com
185.199.108.133			cloud.githubusercontent.com
140.82.114.22			central.github.com
140.82.114.10			codeload.github.com
52.216.97.171			github-cloud.s3.amazonaws.com
3.5.29.73			github-com.s3.amazonaws.com
52.216.240.68			github-production-release-asset-2e65be.s3.amazonaws.com
52.217.171.145			github-production-user-asset-6210df.s3.amazonaws.com
52.217.121.137			github-production-repository-file-5c1aeb.s3.amazonaws.com
185.199.108.153			githubstatus.com
140.82.113.17			community.github.com
52.224.38.193			github.dev
185.199.109.133			media.githubusercontent.com
#github End
# Last Update Time : 2024-09-12 11:37:41 

#steam Start
23.210.138.105			steamcommunity.com
23.62.69.145			www.steamcommunity.com
23.60.147.153			steampowered.com
23.62.69.145			steamgames.com
23.8.65.235			steamcommunity.com
23.48.37.166			steamcommunity-a.akamaihd.net
96.17.77.178			store.steampowered.com
23.8.65.235			api.steampowered.com
23.8.65.235			help.steampowered.com
23.48.37.197			store.akamai.steamstatic.com
23.54.76.44			steamcdn-a.akamaihd.net
23.48.37.197			steamstore-a.akamaihd.net
23.48.37.225			cdn.akamai.steamstatic.com
23.60.147.153			steam-chat.com
23.48.37.166			community.akamai.steamstatic.com
23.48.37.221			cdn.steamcommunity.com
23.54.76.18			cdn.steampowered.com
23.48.37.197			cdn.store.steampowered.com
23.48.37.225			media.steampowered.com
#steam End
# Last Update Time : 2024-09-12 11:37:42 

#Ubisoft_download Start
23.6.204.239			static3.cdn.Ubi.com
23.54.41.206			static2.cdn.Ubi.com
184.85.248.65			static1.cdn.Ubi.com
#Ubisoft_download End
# Last Update Time : 2024-09-12 11:37:43 

#docker Start
141.193.213.21			docker.com
54.196.99.49			auth.docker.io
44.193.181.103			hub.docker.com
18.160.200.81			docs.docker.com
104.19.168.24			login.docker.com
34.226.69.105			registry.hub.docker.com
3.224.227.198			docker.io
54.196.99.49			registry-1.docker.io
34.226.69.105			index.docker.io
#docker End
# Last Update Time : 2024-09-12 11:37:43 

#Brave browser Start
18.64.183.24			brave.com
151.101.1.32			laptop-updates.brave.com
#Brave browser End
# Last Update Time : 2024-09-12 11:37:43 

#Tor browser Start
204.8.99.144			www.torproject.org
116.202.120.165			community.torproject.org
116.202.120.166			blog.torproject.org
#Tor browser End
# Last Update Time : 2024-09-12 11:37:43 

#Tails OS Start
94.142.244.34			tails.net
204.13.164.63			download.tails.net
#Tails OS End
# Last Update Time : 2024-09-12 11:37:43 

#Encrypt DNS Start
217.160.156.119			dns.oszx.co
172.67.153.195			0ms.dev
45.90.28.0			anycast.dns.nextdns.io
104.16.133.229			dns.cloudflare.com
146.112.41.2			doh.opendns.com
158.64.1.29			kaitain.restena.lu
137.66.7.89			max.rethinkdns.com
76.76.2.11			freedns.controld.com
149.248.217.117			dns.dnswarden.com
#Encrypt DNS End
# Last Update Time : 2024-09-12 11:37:44 

#EA Start
23.198.32.174			www.ea.com
104.123.153.171			origin-a.akamaihd.net
23.54.41.93			pl.ea.com
23.60.30.171			media.contentapi.ea.com
23.54.41.93			nds-network-nav.ea.com
#EA End
# Last Update Time : 2024-09-12 11:37:44 

#gitlab Start
172.65.251.78			gitlab.com
172.65.251.78			www.gitlab.com
104.17.71.206			page.gitlab.com
172.64.148.245			packages.gitlab.com
104.18.249.37			support.gitlab.com
172.64.148.245			customers.gitlab.com
172.65.216.50			staging.gitlab.com
216.198.54.1			federal-support.gitlab.com
35.227.35.254			registry.gitlab.com
173.245.58.97			evelup.gitlab.com
172.64.148.245			chef.gitlab.com
#gitlab End
# Last Update Time : 2024-09-12 11:37:44 

#debian Start
199.232.98.132			deb.debian.org
#debian End
# Last Update Time : 2024-09-12 11:37:44 

#iwara Start
104.26.12.96			iwara.tv
172.67.71.154			i.iwara.tv
104.26.12.96			www.iwara.tv
66.165.237.254			hime.iwara.tv
163.172.40.145			aku.iwara.tv
163.172.42.175			sukone.iwara.tv
163.172.81.17			xin.iwara.tv
163.172.40.123			uta.iwara.tv
192.211.62.190			mikoto.iwara.tv
163.172.42.175			sukone.iwara.tv
66.165.240.196			service.iwara.tv
163.172.44.153			miki.iwara.tv
104.26.12.96			api.iwara.tv
66.165.240.194			files.iwara.tv
151.115.97.15			bronya.iwara.tv
151.115.97.14			blade.iwara.tv
151.115.90.15			clara.iwara.tv
51.158.63.130			swan.iwara.tv
163.172.57.37			piko.iwara.tv
163.172.62.89			momo.iwara.tv
163.172.39.227			cul.iwara.tv
151.115.90.24			robin.iwara.tv
62.210.95.208			bailu.iwara.tv
62.210.173.23			himeko.iwara.tv
151.115.89.180			firefly.iwara.tv
151.115.97.4			lynx.iwara.tv
51.159.223.77			silverwolf.iwara.tv
62.210.173.43			pela.iwara.tv
151.115.89.253			jade.iwara.tv
151.115.97.11			welt.iwara.tv
151.115.96.228			asta.iwara.tv
151.115.90.6			sparkle.iwara.tv
151.115.90.3			yukong.iwara.tv
163.172.40.81			tei.iwara.tv
151.115.97.13			topaz.iwara.tv
151.115.90.14			kafka.iwara.tv
151.115.90.4			herta.iwara.tv
151.115.97.5			hook.iwara.tv
163.172.80.31			uni.iwara.tv
151.115.90.5			hanya.iwara.tv
#iwara End
# Last Update Time : 2024-09-12 11:37:46 

#EPIC Start
54.230.18.13			download2.epicgames.com
18.154.110.67			download3.epicgames.com
18.154.110.103			download4.epicgames.com
18.160.200.40			download.epicgames.com
104.123.153.185			epicgames-download1.akamaized.net
3.168.51.82			epic-social-social-modules-prod.ol.epicgames.com
34.231.44.82			eulatracking-public-service-prod06.ol.epicgames.com
18.160.225.105			media-cdn.epicgames.com
23.6.205.30			static-assets-prod.epicgames.com
23.223.181.152			store-content.ak.epicgames.com
54.81.72.205			tracking.epicgames.com
#EPIC End
# Last Update Time : 2024-09-12 11:37:46 

#google Start
172.217.2.35			update.googleapis.com
172.217.1.106			translate-pa.googleapis.com
142.250.191.110			translate.google.com
172.217.4.74			firebaseinstallations.googleapis.com
142.250.190.106			infinitedata-pa.googleapis.com
172.217.4.42			geller-pa.googleapis.com
108.177.12.188			alt1.mobile-gtalk.l.google.com
172.253.62.188			alt2.mobile-gtalk4.l.google.com
64.233.186.188			alt3.mobile-gtalk.l.google.com
209.85.202.188			alt4.mobile-gtalk4.l.google.com
64.233.184.188			alt5.mobile-gtalk.l.google.com
142.250.27.188			alt6.mobile-gtalk4.l.google.com
142.250.153.188			alt7.mobile-gtalk.l.google.com
142.251.9.188			alt8.mobile-gtalk4.l.google.com
142.250.191.202			translate.googleapis.com
142.250.191.110			www3.l.google.com
142.250.191.195			services.googleapis.cn
142.250.191.206			play-fe.googleapis.com
142.250.190.150			play-lh.googleusercontent.com
216.239.32.223			play.googleapis.com
108.177.12.188			alt1-mtalk.google.com
172.253.62.188			alt2-mtalk.google.com
64.233.186.188			alt3-mtalk.google.com
209.85.202.188			alt4-mtalk.google.com
64.233.184.188			alt5-mtalk.google.com
142.250.27.188			alt6-mtalk.google.com
142.250.153.188			alt7-mtalk.google.com
142.251.9.188			alt8-mtalk.google.com
172.217.5.10			content-autofill.googleapis.com
142.250.191.195			googlecn-lopri.l.google.com
142.250.191.163			www.googleapis.cn
#google End
# Last Update Time : 2024-09-12 11:37:47 

#xbox Start
23.54.40.9			gameclipscontent-d2009.xboxlive.com
23.215.15.156			images-eds.xboxlive.com
23.192.220.150			xbl-smooth.xboxlive.com
23.54.40.9			titlehub.xboxlive.com
23.215.15.218			compass.xboxlive.com
23.54.40.9			xnotify.xboxlive.com
52.165.145.141			activityhub.xboxlive.com
23.54.40.9			images-eds-ssl.xboxlive.com
199.46.35.121			rta.xboxlive.com
23.78.8.9			peoplehub.xboxlive.com
40.78.138.172			editorial.xboxlive.com
184.25.59.69			assets1.xboxlive.cn
184.25.59.70			assets2.xboxlive.cn
20.112.250.133			xboxlive.com
13.107.246.51			da.xboxservices.com
40.122.167.99			device.auth.xboxlive.com
#xbox End
# Last Update Time : 2024-09-12 11:37:47 

#Apkpure Start
172.67.20.93			download.pureapk.com
104.22.9.141			api.pureapk.com
104.22.43.111			t.apkpure.net
172.67.20.93			tapi.pureapk.com
172.67.20.93			rdelivery.pureapk.com
104.26.13.136			tapi.upload.app
45.33.36.159			api.sve.cc
104.233.133.90			wap.yushuwu.cloud
#Apkpure End
# Last Update Time : 2024-09-12 11:37:48 

#Microsoft Start
20.190.155.1			login.microsoftonline.com
20.166.126.56			fe3cr.delivery.mp.microsoft.com
52.252.198.176			fe2cr.update.microsoft.com
20.12.23.50			slscr.update.microsoft.com
40.118.171.167			nav-edge.smartscreen.microsoft.com
20.190.155.36			graph.microsoft.com
23.54.41.214			go.microsoft.com
13.107.246.51			static.edge.microsoftapp.net
204.79.197.203			oneocsp.microsoft.com
20.94.153.70			nf.smartscreen.microsoft.com
4.255.78.159			wdcp.microsoft.com
52.109.8.89			officeclient.microsoft.com
20.42.7.128			api-edge.cognitive.microsofttranslator.com
204.79.197.239			edge.microsoft.com
23.54.42.96			storeedgefd.dsx.mp.microsoft.com
#Microsoft End
# Last Update Time : 2024-09-12 11:37:48 

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
