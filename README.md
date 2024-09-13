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
140.82.112.26			live.github.com
140.82.116.13			uploads.github.com
185.199.111.153			training.github.com
185.199.109.133			objects.githubusercontent.com
185.199.109.153			metamask.github.io
185.199.109.153			pages.github.com
13.107.42.16			pipelines.actions.githubusercontent.com
185.199.111.153			customer-stories-feed.github.com
185.199.109.154			github.githubassets.com
140.82.114.22			central.github.com
140.82.114.21			viewscreen.githubusercontent.com
185.199.109.133			desktop.githubusercontent.com
185.199.110.133			raw.github.com
185.199.108.133			repository-images.githubusercontent.com
185.199.109.153			assets-cdn.github.com
185.199.109.133			github.map.fastly.net
52.217.235.193			github-production-release-asset-2e65be.s3.amazonaws.com
3.5.28.203			github-production-repository-file-5c1aeb.s3.amazonaws.com
3.5.22.26			github-production-user-asset-6210df.s3.amazonaws.com
185.199.109.133			camo.githubusercontent.com
185.199.108.133			github.map.fastly.net
151.101.193.194			github.global.ssl.fastly.net
185.199.108.133			gist.githubusercontent.com
140.82.112.29			githubapp.com
192.0.66.2			github.blog
52.216.207.171			github-cloud.s3.amazonaws.com
185.199.109.153			githubstatus.com
185.199.109.153			guides.github.com
140.82.113.17			help.github.com
140.82.114.18			github.community
140.82.116.3			gist.github.com
185.199.110.153			github.io
140.82.116.4			github.com
192.0.66.2			github.blog
140.82.116.6			api.github.com
185.199.110.133			raw.githubusercontent.com
185.199.109.153			archiveprogram.github.com
185.199.110.153			assets-cdn.github.com
185.199.109.133			user-images.githubusercontent.com
185.199.111.133			favicons.githubusercontent.com
185.199.109.133			avatars5.githubusercontent.com
185.199.108.133			avatars4.githubusercontent.com
185.199.111.133			avatars3.githubusercontent.com
185.199.109.133			avatars2.githubusercontent.com
185.199.110.133			avatars6.githubusercontent.com
185.199.109.133			avatars7.githubusercontent.com
185.199.111.133			avatars8.githubusercontent.com
185.199.110.133			avatars1.githubusercontent.com
185.199.108.133			avatars0.githubusercontent.com
185.199.108.133			avatars.githubusercontent.com
185.199.109.133			cloud.githubusercontent.com
140.82.112.21			central.github.com
140.82.116.9			codeload.github.com
54.231.227.81			github-cloud.s3.amazonaws.com
3.5.22.165			github-com.s3.amazonaws.com
16.182.66.233			github-production-release-asset-2e65be.s3.amazonaws.com
52.217.160.17			github-production-user-asset-6210df.s3.amazonaws.com
3.5.28.203			github-production-repository-file-5c1aeb.s3.amazonaws.com
185.199.108.153			githubstatus.com
140.82.113.17			community.github.com
20.99.227.183			github.dev
185.199.111.133			media.githubusercontent.com
#github End
# Last Update Time : 2024-09-14 07:48:21 

#steam Start
104.68.104.163			steamcommunity.com
104.68.112.116			www.steamcommunity.com
104.68.112.116			steampowered.com
104.68.112.116			steamgames.com
96.16.55.10			cdn.steamstatic.com
23.67.33.225			clientconfig.akamai.steamstatic.com
103.28.54.162			ext3-hkg1.steamserver.net
96.16.55.23			test.steampowered.com
47.88.36.142			steamcloud-hkg.oss-accelerate.aliyuncs.com
84.53.139.129			ipv6check-udp.steamserver.net
45.121.184.21			ext2-tyo3.steamserver.net
103.10.124.125			ext4-sgp1.steamserver.net
103.10.124.124			ext3-sgp1.steamserver.net
45.121.184.23			ext4-tyo3.steamserver.net
103.28.54.165			ext1-hkg1.steamserver.net
103.28.54.181			ext2-hkg1.steamserver.net
103.28.54.173			ext7-hkg1.steamserver.net
45.121.184.21			ext2-tyo3.steamserver.net
####			ipv6check-http.steamserver.net
106.42.232.174			dl.steam.clngaa.com
157.185.156.117			cdn-ws.content.steamchina.com
104.68.104.163			steamcommunity.com
96.16.55.23			steamcommunity-a.akamaihd.net
23.44.73.180			store.steampowered.com
104.68.104.163			api.steampowered.com
198.185.159.145			steampoweredmedia.com
104.68.104.163			help.steampowered.com
96.16.55.6			store.akamai.steamstatic.com
23.67.33.209			steamcdn-a.akamaihd.net
96.16.55.7			steamstore-a.akamaihd.net
96.16.55.37			cdn.akamai.steamstatic.com
104.68.112.116			steam-chat.com
96.16.55.23			community.akamai.steamstatic.com
96.16.55.36			cdn.steamcommunity.com
23.67.33.218			cdn.steampowered.com
96.16.55.6			cdn.store.steampowered.com
96.16.55.37			media.steampowered.com
#steam End
# Last Update Time : 2024-09-14 07:48:23 

#Ubisoft_download Start
23.36.21.63			static3.cdn.Ubi.com
23.36.21.209			static2.cdn.Ubi.com
84.53.139.65			static1.cdn.Ubi.com
#Ubisoft_download End
# Last Update Time : 2024-09-14 07:48:23 

#docker Start
141.193.213.20			docker.com
3.219.239.5			auth.docker.io
3.224.227.198			hub.docker.com
18.155.202.90			docs.docker.com
104.19.168.24			login.docker.com
3.219.239.5			registry.hub.docker.com
44.193.181.103			docker.io
54.196.99.49			registry-1.docker.io
34.226.69.105			index.docker.io
#docker End
# Last Update Time : 2024-09-14 07:48:23 

#Brave browser Start
108.138.246.94			brave.com
151.101.129.32			laptop-updates.brave.com
#Brave browser End
# Last Update Time : 2024-09-14 07:48:23 

#Tor browser Start
95.216.163.36			www.torproject.org
116.202.120.166			community.torproject.org
204.8.99.146			blog.torproject.org
#Tor browser End
# Last Update Time : 2024-09-14 07:48:23 

#Tails OS Start
94.142.244.34			tails.net
204.13.164.63			download.tails.net
#Tails OS End
# Last Update Time : 2024-09-14 07:48:23 

#Encrypt DNS Start
217.160.156.119			dns.oszx.co
172.67.153.195			0ms.dev
45.90.30.0			anycast.dns.nextdns.io
104.16.133.229			dns.cloudflare.com
146.112.41.2			doh.opendns.com
158.64.1.29			kaitain.restena.lu
137.66.7.89			max.rethinkdns.com
76.76.2.11			freedns.controld.com
149.248.217.117			dns.dnswarden.com
#Encrypt DNS End
# Last Update Time : 2024-09-14 07:48:23 

#EA Start
23.195.144.188			www.ea.com
23.192.228.149			origin-a.akamaihd.net
23.36.21.91			pl.ea.com
184.84.194.53			media.contentapi.ea.com
23.36.21.91			nds-network-nav.ea.com
#EA End
# Last Update Time : 2024-09-14 07:48:23 

#gitlab Start
172.65.251.78			gitlab.com
172.65.251.78			www.gitlab.com
104.17.70.206			page.gitlab.com
104.18.39.11			packages.gitlab.com
104.18.249.37			support.gitlab.com
104.18.39.11			customers.gitlab.com
172.65.216.50			staging.gitlab.com
216.198.54.1			federal-support.gitlab.com
35.227.35.254			registry.gitlab.com
172.64.35.157			evelup.gitlab.com
104.18.39.11			chef.gitlab.com
#gitlab End
# Last Update Time : 2024-09-14 07:48:23 

#debian Start
146.75.94.132			deb.debian.org
#debian End
# Last Update Time : 2024-09-14 07:48:23 

#iwara Start
172.67.71.154			iwara.tv
104.26.12.96			i.iwara.tv
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
104.26.13.96			api.iwara.tv
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
# Last Update Time : 2024-09-14 07:48:24 

#EPIC Start
108.138.246.124			download2.epicgames.com
18.155.192.37			download3.epicgames.com
18.155.202.55			download4.epicgames.com
18.239.199.15			download.epicgames.com
23.192.228.143			epicgames-download1.akamaized.net
3.168.86.8			epic-social-social-modules-prod.ol.epicgames.com
34.231.44.82			eulatracking-public-service-prod06.ol.epicgames.com
18.155.192.113			media-cdn.epicgames.com
23.36.21.134			static-assets-prod.epicgames.com
23.203.209.213			store-content.ak.epicgames.com
3.232.178.59			tracking.epicgames.com
#EPIC End
# Last Update Time : 2024-09-14 07:48:24 

#google Start
142.251.32.35			update.googleapis.com
142.250.191.42			translate-pa.googleapis.com
142.251.46.174			translate.google.com
172.217.164.106			firebaseinstallations.googleapis.com
142.250.72.202			infinitedata-pa.googleapis.com
142.251.46.234			geller-pa.googleapis.com
108.177.104.188			alt1.mobile-gtalk.l.google.com
74.125.126.188			alt2.mobile-gtalk4.l.google.com
172.253.113.188			alt3.mobile-gtalk.l.google.com
173.194.77.188			alt4.mobile-gtalk4.l.google.com
173.194.219.188			alt5.mobile-gtalk.l.google.com
142.250.112.188			alt6.mobile-gtalk4.l.google.com
172.217.197.188			alt7.mobile-gtalk.l.google.com
108.177.12.188			alt8.mobile-gtalk4.l.google.com
142.251.46.234			translate.googleapis.com
142.251.46.174			www3.l.google.com
172.217.12.99			services.googleapis.cn
142.250.189.206			play-fe.googleapis.com
142.251.46.214			play-lh.googleusercontent.com
216.239.34.223			play.googleapis.com
108.177.104.188			alt1-mtalk.google.com
74.125.126.188			alt2-mtalk.google.com
172.253.113.188			alt3-mtalk.google.com
173.194.77.188			alt4-mtalk.google.com
173.194.219.188			alt5-mtalk.google.com
142.250.112.188			alt6-mtalk.google.com
172.217.197.188			alt7-mtalk.google.com
108.177.12.188			alt8-mtalk.google.com
142.251.32.42			content-autofill.googleapis.com
142.250.189.163			googlecn-lopri.l.google.com
142.251.32.35			www.googleapis.cn
#google End
# Last Update Time : 2024-09-14 07:48:25 

#xbox Start
23.36.20.9			gameclipscontent-d2009.xboxlive.com
23.67.33.105			images-eds.xboxlive.com
23.192.228.143			xbl-smooth.xboxlive.com
23.36.20.9			titlehub.xboxlive.com
23.67.33.105			compass.xboxlive.com
23.36.20.9			xnotify.xboxlive.com
13.66.204.157			activityhub.xboxlive.com
23.36.20.9			images-eds-ssl.xboxlive.com
199.46.35.127			rta.xboxlive.com
23.44.72.9			peoplehub.xboxlive.com
52.242.98.79			editorial.xboxlive.com
23.50.8.192			assets1.xboxlive.cn
23.50.8.227			assets2.xboxlive.cn
20.70.246.20			xboxlive.com
13.107.246.69			da.xboxservices.com
52.156.99.28			device.auth.xboxlive.com
#xbox End
# Last Update Time : 2024-09-14 07:48:25 

#Apkpure Start
104.22.8.141			download.pureapk.com
172.67.20.93			api.pureapk.com
172.67.11.98			t.apkpure.net
104.22.8.141			tapi.pureapk.com
104.22.9.141			rdelivery.pureapk.com
104.26.13.136			tapi.upload.app
45.33.36.159			api.sve.cc
#Apkpure End
# Last Update Time : 2024-09-14 07:48:25 

#Microsoft Start
40.126.62.130			login.microsoftonline.com
13.85.23.206			fe3cr.delivery.mp.microsoft.com
20.97.190.217			fe2cr.update.microsoft.com
13.85.23.86			slscr.update.microsoft.com
40.74.166.188			nav-edge.smartscreen.microsoft.com
20.190.132.40			graph.microsoft.com
23.36.21.215			go.microsoft.com
13.107.246.69			static.edge.microsoftapp.net
204.79.197.203			oneocsp.microsoft.com
13.91.96.185			nf.smartscreen.microsoft.com
20.81.62.55			wdcp.microsoft.com
52.109.8.89			officeclient.microsoft.com
40.82.255.97			api-edge.cognitive.microsofttranslator.com
204.79.197.239			edge.microsoft.com
23.36.22.100			storeedgefd.dsx.mp.microsoft.com
152.195.19.97			msedgeextensions.sf.tlu.dl.delivery.mp.microsoft.com
#Microsoft End
# Last Update Time : 2024-09-14 07:48:26 

#spotify Start
104.199.241.202			ap-gae2.spotify.com
104.154.127.247			ap-guc3.spotify.com
104.199.65.9			ap-gew1.spotify.com
34.158.1.133			ap-gew4.spotify.com
34.158.255.62			ap-gue1.spotify.com
35.186.224.24			spclient.wg.spotify.com
35.186.224.24			wg.spotify.com
35.186.224.22			gae-spclient.spotify.com
23.212.62.94			audio4-ak-spotify-com.akamaized.net
23.212.62.85			heads4-ak-spotify-com.akamaized.net
23.212.62.94			audio-ak-spotify-com.akamaized.net
23.212.62.86			audio-akp-quic-spotify-com.akamaized.net
#spotify End
# Last Update Time : 2024-09-14 07:48:26 

#scdn Start
199.232.210.248			audio-fa.scdn.co
23.212.62.85			misc.scdn.co
23.212.62.85			i.scdn.co
199.232.210.248			newjams-images.scdn.co
199.232.210.248			dailymix-images.scdn.co
199.232.210.248			thisis-images.scdn.co
199.232.214.248			charts-images.scdn.co
199.232.210.248			seeded-session-images.scdn.co
199.232.214.248			download.scdn.co
####			
#scdn End
# Last Update Time : 2024-09-14 07:48:27 

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
