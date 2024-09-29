# FastHostSync


## 1. 实现
对Hosts进行更新  
解决Steam、github、Apkpure 、docker、EPIC、EA、gitlab、xbox、spotify、Brave Browser、TailsOS、Tor Browser等访问问题

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
1. ALL: `https://raw.githubusercontent.com/Shura23/FastHostSync/refs/heads/main/Hosts`  
2. Steam: `https://raw.githubusercontent.com/Shura23/FastHostSync/refs/heads/main/Hosts_steam`  
3. github: `https://raw.githubusercontent.com/Shura23/FastHostSync/refs/heads/main/Hosts_github`
4. gitlab: `https://raw.githubusercontent.com/Shura23/FastHostSync/refs/heads/main/Hosts_gitlab`
5. EPIC: `https://raw.githubusercontent.com/Shura23/FastHostSync/refs/heads/main/Hosts_EPIC`
6. Apkpure: `https://raw.githubusercontent.com/Shura23/FastHostSync/refs/heads/main/Hosts_Apkpure`
7. TailsOS：`https://raw.githubusercontent.com/Shura23/FastHostSync/refs/heads/main/Hosts_Tails%20OS`
8. Tor Browser: `https://raw.githubusercontent.com/Shura23/FastHostSync/refs/heads/main/Hosts_Tor%20browser`
9. docker: `https://raw.githubusercontent.com/Shura23/FastHostSync/refs/heads/main/Hosts_docker`
10. onedrive: `https://raw.githubusercontent.com/Shura23/FastHostSync/refs/heads/main/Hosts_onedrive`
11. iwara: `https://raw.githubusercontent.com/Shura23/FastHostSync/refs/heads/main/Hosts_iwara`
12. spotify: `https://raw.githubusercontent.com/Shura23/FastHostSync/refs/heads/main/Hosts_spotify`
13. xbox: `https://raw.githubusercontent.com/Shura23/FastHostSync/refs/heads/main/Hosts_xbox`


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
140.82.112.25			alive.github.com
185.199.111.154			docs.github.com
140.82.113.26			live.github.com
140.82.114.14			uploads.github.com
185.199.108.153			training.github.com
185.199.110.133			objects.githubusercontent.com
185.199.110.153			metamask.github.io
185.199.111.153			pages.github.com
13.107.42.16			pipelines.actions.githubusercontent.com
185.199.111.153			customer-stories-feed.github.com
185.199.109.154			github.githubassets.com
140.82.114.21			central.github.com
140.82.114.21			viewscreen.githubusercontent.com
185.199.108.133			desktop.githubusercontent.com
185.199.108.133			raw.github.com
185.199.108.133			repository-images.githubusercontent.com
185.199.111.153			assets-cdn.github.com
185.199.110.133			github.map.fastly.net
52.216.101.115			github-production-release-asset-2e65be.s3.amazonaws.com
54.231.129.65			github-production-repository-file-5c1aeb.s3.amazonaws.com
3.5.30.192			github-production-user-asset-6210df.s3.amazonaws.com
185.199.108.133			camo.githubusercontent.com
185.199.108.133			github.map.fastly.net
151.101.129.194			github.global.ssl.fastly.net
185.199.110.133			gist.githubusercontent.com
140.82.114.30			githubapp.com
192.0.66.2			github.blog
52.217.86.4			github-cloud.s3.amazonaws.com
185.199.108.153			githubstatus.com
185.199.110.153			guides.github.com
140.82.114.18			help.github.com
140.82.113.18			github.community
140.82.113.3			gist.github.com
185.199.109.153			github.io
140.82.114.4			github.com
192.0.66.2			github.blog
140.82.113.5			api.github.com
185.199.108.133			raw.githubusercontent.com
185.199.108.153			archiveprogram.github.com
185.199.108.153			assets-cdn.github.com
185.199.111.133			user-images.githubusercontent.com
185.199.110.133			favicons.githubusercontent.com
185.199.109.133			avatars5.githubusercontent.com
185.199.110.133			avatars4.githubusercontent.com
185.199.110.133			avatars3.githubusercontent.com
185.199.109.133			avatars2.githubusercontent.com
185.199.111.133			avatars6.githubusercontent.com
185.199.108.133			avatars7.githubusercontent.com
185.199.108.133			avatars8.githubusercontent.com
185.199.111.133			avatars1.githubusercontent.com
185.199.108.133			avatars0.githubusercontent.com
185.199.111.133			avatars.githubusercontent.com
185.199.111.133			cloud.githubusercontent.com
140.82.114.21			central.github.com
140.82.113.9			codeload.github.com
16.182.66.25			github-cloud.s3.amazonaws.com
3.5.2.202			github-com.s3.amazonaws.com
52.217.112.209			github-production-release-asset-2e65be.s3.amazonaws.com
3.5.25.174			github-production-user-asset-6210df.s3.amazonaws.com
3.5.2.202			github-production-repository-file-5c1aeb.s3.amazonaws.com
185.199.110.153			githubstatus.com
140.82.114.17			community.github.com
52.224.38.193			github.dev
185.199.109.133			media.githubusercontent.com
#github End
# Last Update Time : 2024-09-29 22:30:02 

#steam Start
23.47.27.74			steamcommunity.com
104.94.121.98			www.steamcommunity.com
104.94.121.98			steampowered.com
104.94.121.98			steamgames.com
23.215.0.139			clientconfig.akamai.steamstatic.com
103.28.54.162			ext3-hkg1.steamserver.net
23.54.127.117			test.steampowered.com
47.252.96.19			steamcloud-hkg.oss-accelerate.aliyuncs.com
84.53.139.129			ipv6check-udp.steamserver.net
23.54.127.120			steamuserimages-a.akamaihd.net
183.61.243.1			steamuserimages-a.xxghh.biz
106.42.232.104			dl.steam.clngaa.com
23.47.27.74			steamcommunity.com
23.54.127.104			steamcommunity-a.akamaihd.net
23.56.8.80			store.steampowered.com
23.47.27.74			api.steampowered.com
198.49.23.145			steampoweredmedia.com
23.47.27.74			help.steampowered.com
23.54.127.122			store.akamai.steamstatic.com
23.215.0.133			steamcdn-a.akamaihd.net
23.54.127.112			steamstore-a.akamaihd.net
104.94.121.98			steam-chat.com
23.54.127.104			community.akamai.steamstatic.com
23.54.127.113			shared.steamstatic.com
23.54.127.101			clan.steamstatic.com
23.54.127.104			cdn.steamcommunity.com
23.215.0.137			cdn.steampowered.com
23.54.127.122			cdn.store.steampowered.com
23.54.127.112			media.steampowered.com
#steam End
# Last Update Time : 2024-09-29 22:30:03 

#Ubisoft_download Start
23.62.160.240			static3.cdn.Ubi.com
23.210.1.110			static2.cdn.Ubi.com
####			static1.cdn.Ubi.com
#Ubisoft_download End
# Last Update Time : 2024-09-29 22:30:03 

#docker Start
141.193.213.21			docker.com
34.226.69.105			auth.docker.io
3.224.227.198			hub.docker.com
18.160.10.58			docs.docker.com
104.19.167.24			login.docker.com
3.219.239.5			registry.hub.docker.com
44.219.3.189			docker.io
54.196.99.49			registry-1.docker.io
3.219.239.5			index.docker.io
#docker End
# Last Update Time : 2024-09-29 22:30:03 

#Brave browser Start
3.167.56.82			brave.com
151.101.1.32			laptop-updates.brave.com
#Brave browser End
# Last Update Time : 2024-09-29 22:30:03 

#Tor browser Start
204.8.99.146			www.torproject.org
95.216.163.36			community.torproject.org
204.8.99.146			blog.torproject.org
#Tor browser End
# Last Update Time : 2024-09-29 22:30:03 

#Tails OS Start
204.13.164.63			tails.net
204.13.164.63			download.tails.net
#Tails OS End
# Last Update Time : 2024-09-29 22:30:04 

#Encrypt DNS Start
217.160.156.119			dns.oszx.co
172.64.41.4			mozilla.cloudflare-dns.com
104.21.88.221			0ms.dev
45.90.30.0			anycast.dns.nextdns.io
104.16.132.229			dns.cloudflare.com
146.112.41.2			doh.opendns.com
158.64.1.29			kaitain.restena.lu
137.66.7.89			max.rethinkdns.com
76.76.2.11			freedns.controld.com
149.248.217.117			dns.dnswarden.com
#Encrypt DNS End
# Last Update Time : 2024-09-29 22:30:04 

#EA Start
23.56.10.146			www.ea.com
23.54.127.79			origin-a.akamaihd.net
23.210.1.13			pl.ea.com
23.13.164.104			media.contentapi.ea.com
23.210.1.13			nds-network-nav.ea.com
#EA End
# Last Update Time : 2024-09-29 22:30:04 

#gitlab Start
172.65.251.78			gitlab.com
172.65.251.78			www.gitlab.com
104.17.72.206			page.gitlab.com
104.18.39.11			packages.gitlab.com
104.18.248.37			support.gitlab.com
104.18.39.11			customers.gitlab.com
172.65.216.50			staging.gitlab.com
216.198.53.1			federal-support.gitlab.com
35.227.35.254			registry.gitlab.com
173.245.58.97			evelup.gitlab.com
172.64.148.245			chef.gitlab.com
#gitlab End
# Last Update Time : 2024-09-29 22:30:04 

#debian Start
146.75.38.132			deb.debian.org
#debian End
# Last Update Time : 2024-09-29 22:30:04 

#iwara Start
104.26.12.96			iwara.tv
62.210.173.23			himeko.iwara.tv
172.67.71.154			i.iwara.tv
104.26.12.96			www.iwara.tv
66.165.237.254			hime.iwara.tv
163.172.40.145			aku.iwara.tv
163.172.42.175			sukone.iwara.tv
151.115.90.2			acheron.iwara.tv
163.172.81.17			xin.iwara.tv
163.172.40.123			uta.iwara.tv
192.211.62.190			mikoto.iwara.tv
163.172.42.175			sukone.iwara.tv
66.165.240.196			service.iwara.tv
163.172.44.153			miki.iwara.tv
172.67.71.154			api.iwara.tv
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
# Last Update Time : 2024-09-29 22:30:04 

#EPIC Start
18.165.98.60			download2.epicgames.com
3.162.103.16			download3.epicgames.com
99.84.191.92			download4.epicgames.com
18.154.227.40			download.epicgames.com
23.54.127.75			epicgames-download1.akamaized.net
52.85.132.6			epic-social-social-modules-prod.ol.epicgames.com
3.212.80.104			eulatracking-public-service-prod06.ol.epicgames.com
3.162.112.37			media-cdn.epicgames.com
23.62.161.36			static-assets-prod.epicgames.com
23.1.60.248			store-content.ak.epicgames.com
44.207.148.140			tracking.epicgames.com
#EPIC End
# Last Update Time : 2024-09-29 22:30:04 

#google Start
172.253.122.94			update.googleapis.com
172.253.122.95			translate-pa.googleapis.com
142.250.31.138			translate.google.com
142.250.31.95			firebaseinstallations.googleapis.com
172.253.122.95			infinitedata-pa.googleapis.com
142.250.31.95			geller-pa.googleapis.com
209.85.202.188			alt1.mobile-gtalk.l.google.com
64.233.184.188			alt2.mobile-gtalk4.l.google.com
142.250.27.188			alt3.mobile-gtalk.l.google.com
142.250.153.188			alt4.mobile-gtalk4.l.google.com
142.251.9.188			alt5.mobile-gtalk.l.google.com
142.250.150.188			alt6.mobile-gtalk4.l.google.com
74.125.200.188			alt7.mobile-gtalk.l.google.com
142.250.157.188			alt8.mobile-gtalk4.l.google.com
142.251.111.95			translate.googleapis.com
142.250.31.138			www3.l.google.com
142.251.167.94			services.googleapis.cn
64.233.180.139			play-fe.googleapis.com
172.253.63.119			play-lh.googleusercontent.com
216.239.36.223			play.googleapis.com
209.85.202.188			alt1-mtalk.google.com
64.233.184.188			alt2-mtalk.google.com
142.250.27.188			alt3-mtalk.google.com
142.250.153.188			alt4-mtalk.google.com
142.251.9.188			alt5-mtalk.google.com
142.250.150.188			alt6-mtalk.google.com
74.125.200.188			alt7-mtalk.google.com
142.250.157.188			alt8-mtalk.google.com
64.233.180.95			content-autofill.googleapis.com
172.253.122.94			googlecn-lopri.l.google.com
142.251.163.94			www.googleapis.cn
#google End
# Last Update Time : 2024-09-29 22:30:05 

#xbox Start
23.210.0.10			gameclipscontent-d2009.xboxlive.com
23.55.176.235			images-eds.xboxlive.com
23.215.0.228			xbl-smooth.xboxlive.com
23.210.0.10			titlehub.xboxlive.com
23.55.176.233			compass.xboxlive.com
23.210.0.10			xnotify.xboxlive.com
13.66.204.157			activityhub.xboxlive.com
23.210.0.10			images-eds-ssl.xboxlive.com
199.46.35.126			rta.xboxlive.com
23.56.8.10			peoplehub.xboxlive.com
40.78.138.172			editorial.xboxlive.com
23.53.11.246			assets1.xboxlive.cn
23.53.11.244			assets2.xboxlive.cn
20.231.239.246			xboxlive.com
13.107.253.40			da.xboxservices.com
20.109.105.194			device.auth.xboxlive.com
#xbox End
# Last Update Time : 2024-09-29 22:30:05 

#Apkpure Start
172.67.20.93			download.pureapk.com
104.22.9.141			api.pureapk.com
172.67.11.98			t.apkpure.net
172.67.20.93			tapi.pureapk.com
104.22.9.141			rdelivery.pureapk.com
104.26.13.136			tapi.upload.app
45.33.36.159			api.sve.cc
#Apkpure End
# Last Update Time : 2024-09-29 22:30:05 

#Microsoft Start
20.190.151.67			login.microsoftonline.com
20.242.39.171			fe3cr.delivery.mp.microsoft.com
20.163.45.186			fe2cr.update.microsoft.com
20.114.59.183			slscr.update.microsoft.com
23.54.127.49			dl.delivery.mp.microsoft.com
13.91.96.185			nav-edge.smartscreen.microsoft.com
20.190.151.38			graph.microsoft.com
23.210.2.210			go.microsoft.com
13.107.246.40			static.edge.microsoftapp.net
204.79.197.203			oneocsp.microsoft.com
40.118.171.167			nf.smartscreen.microsoft.com
20.253.175.208			wdcp.microsoft.com
52.109.8.89			officeclient.microsoft.com
20.42.7.128			api-edge.cognitive.microsofttranslator.com
204.79.197.239			edge.microsoft.com
23.210.1.233			storeedgefd.dsx.mp.microsoft.com
152.195.19.97			msedgeextensions.sf.tlu.dl.delivery.mp.microsoft.com
#Microsoft End
# Last Update Time : 2024-09-29 22:30:05 

#spotify Start
104.199.241.202			ap-gae2.spotify.com
104.154.127.247			ap-guc3.spotify.com
104.199.65.9			ap-gew1.spotify.com
34.158.1.133			ap-gew4.spotify.com
34.158.255.62			ap-gue1.spotify.com
35.186.224.24			spclient.wg.spotify.com
35.186.224.24			wg.spotify.com
35.186.224.22			gae-spclient.spotify.com
23.215.0.132			audio4-ak-spotify-com.akamaized.net
23.46.150.72			heads4-ak-spotify-com.akamaized.net
23.215.0.139			audio-ak-spotify-com.akamaized.net
23.215.0.145			audio-akp-quic-spotify-com.akamaized.net
#spotify End
# Last Update Time : 2024-09-29 22:30:06 

#scdn Start
199.232.214.248			audio-fa.scdn.co
23.215.0.137			misc.scdn.co
23.215.0.142			i.scdn.co
199.232.210.248			newjams-images.scdn.co
199.232.210.248			dailymix-images.scdn.co
199.232.210.248			thisis-images.scdn.co
199.232.210.248			charts-images.scdn.co
199.232.210.248			seeded-session-images.scdn.co
199.232.214.248			download.scdn.co
#scdn End
# Last Update Time : 2024-09-29 22:30:06 

#onedrive Start
13.107.139.11			onedrive.live.com
13.107.42.12			skyapi.onedrive.live.com
184.27.1.55			api.onedrive.live.com
#onedrive End
# Last Update Time : 2024-09-29 22:30:06 

#other Start
184.73.18.241			www.ghostery.com
44.194.193.30			ghostery.com
#other End
# Last Update Time : 2024-09-29 22:30:06 

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
