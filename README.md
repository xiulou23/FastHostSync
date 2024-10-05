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
140.82.113.26			alive.github.com
185.199.108.154			docs.github.com
140.82.113.25			live.github.com
140.82.114.13			uploads.github.com
185.199.111.153			training.github.com
185.199.111.133			objects.githubusercontent.com
185.199.110.153			metamask.github.io
185.199.109.153			pages.github.com
13.107.42.16			pipelines.actions.githubusercontent.com
185.199.108.153			customer-stories-feed.github.com
185.199.110.154			github.githubassets.com
140.82.113.22			central.github.com
140.82.113.22			viewscreen.githubusercontent.com
185.199.108.133			desktop.githubusercontent.com
185.199.110.133			raw.github.com
185.199.110.133			repository-images.githubusercontent.com
185.199.109.153			assets-cdn.github.com
185.199.109.133			github.map.fastly.net
52.216.60.241			github-production-release-asset-2e65be.s3.amazonaws.com
52.217.71.28			github-production-repository-file-5c1aeb.s3.amazonaws.com
3.5.27.113			github-production-user-asset-6210df.s3.amazonaws.com
185.199.109.133			camo.githubusercontent.com
185.199.111.133			github.map.fastly.net
151.101.1.194			github.global.ssl.fastly.net
185.199.110.133			gist.githubusercontent.com
140.82.114.29			githubapp.com
192.0.66.2			github.blog
54.231.139.81			github-cloud.s3.amazonaws.com
185.199.110.153			githubstatus.com
185.199.108.153			guides.github.com
140.82.113.17			help.github.com
140.82.113.18			github.community
140.82.114.3			gist.github.com
185.199.111.153			github.io
140.82.113.4			github.com
192.0.66.2			github.blog
140.82.113.6			api.github.com
185.199.108.133			raw.githubusercontent.com
185.199.110.153			archiveprogram.github.com
185.199.108.153			assets-cdn.github.com
185.199.109.133			user-images.githubusercontent.com
185.199.110.133			favicons.githubusercontent.com
185.199.110.133			avatars5.githubusercontent.com
185.199.111.133			avatars4.githubusercontent.com
185.199.111.133			avatars3.githubusercontent.com
185.199.109.133			avatars2.githubusercontent.com
185.199.108.133			avatars6.githubusercontent.com
185.199.108.133			avatars7.githubusercontent.com
185.199.111.133			avatars8.githubusercontent.com
185.199.110.133			avatars1.githubusercontent.com
185.199.108.133			avatars0.githubusercontent.com
185.199.110.133			avatars.githubusercontent.com
185.199.108.133			cloud.githubusercontent.com
140.82.112.22			central.github.com
140.82.112.10			codeload.github.com
54.231.229.25			github-cloud.s3.amazonaws.com
52.216.221.33			github-com.s3.amazonaws.com
52.217.133.241			github-production-release-asset-2e65be.s3.amazonaws.com
16.182.36.129			github-production-user-asset-6210df.s3.amazonaws.com
54.231.229.25			github-production-repository-file-5c1aeb.s3.amazonaws.com
185.199.108.153			githubstatus.com
140.82.113.18			community.github.com
52.224.38.193			github.dev
185.199.108.133			media.githubusercontent.com
#github End
# Last Update Time : 2024-10-06 00:27:39 

#steam Start
23.214.234.105			steamcommunity.com
23.213.69.147			www.steamcommunity.com
23.213.69.147			steampowered.com
23.213.69.147			steamgames.com
23.215.0.145			clientconfig.akamai.steamstatic.com
103.28.54.162			ext3-hkg1.steamserver.net
104.96.221.81			test.steampowered.com
47.252.96.19			steamcloud-hkg.oss-accelerate.aliyuncs.com
####			ipv6check-udp.steamserver.net
104.96.221.83			steamuserimages-a.akamaihd.net
117.148.191.10			steamuserimages-a.xxghh.biz
219.152.87.117			dl.steam.clngaa.com
23.214.234.105			steamcommunity.com
104.96.221.51			steamcommunity-a.akamaihd.net
23.45.149.185			store.steampowered.com
23.214.234.105			api.steampowered.com
198.49.23.145			steampoweredmedia.com
23.214.234.105			help.steampowered.com
104.96.221.59			store.akamai.steamstatic.com
23.215.0.133			steamcdn-a.akamaihd.net
104.96.221.59			steamstore-a.akamaihd.net
23.213.69.147			steam-chat.com
104.96.221.66			community.akamai.steamstatic.com
104.96.221.74			shared.steamstatic.com
104.96.221.58			clan.steamstatic.com
104.96.221.51			cdn.steamcommunity.com
23.215.0.136			cdn.steampowered.com
104.96.221.59			cdn.store.steampowered.com
104.96.221.65			media.steampowered.com
#steam End
# Last Update Time : 2024-10-06 00:27:40 

#Ubisoft_download Start
23.222.201.62			static3.cdn.Ubi.com
23.62.165.107			static2.cdn.Ubi.com
193.108.91.206			static1.cdn.Ubi.com
#Ubisoft_download End
# Last Update Time : 2024-10-06 00:27:40 

#docker Start
141.193.213.20			docker.com
34.226.69.105			auth.docker.io
3.224.227.198			hub.docker.com
18.160.10.27			docs.docker.com
104.19.168.24			login.docker.com
3.219.239.5			registry.hub.docker.com
44.193.181.103			docker.io
3.219.239.5			registry-1.docker.io
54.196.99.49			index.docker.io
#docker End
# Last Update Time : 2024-10-06 00:27:40 

#Brave browser Start
3.167.56.104			brave.com
151.101.65.32			laptop-updates.brave.com
#Brave browser End
# Last Update Time : 2024-10-06 00:27:40 

#Tor browser Start
204.8.99.144			www.torproject.org
116.202.120.166			community.torproject.org
116.202.120.165			blog.torproject.org
#Tor browser End
# Last Update Time : 2024-10-06 00:27:40 

#Tails OS Start
204.13.164.63			tails.net
204.13.164.63			download.tails.net
#Tails OS End
# Last Update Time : 2024-10-06 00:27:41 

#Encrypt DNS Start
217.160.156.119			dns.oszx.co
162.159.61.4			mozilla.cloudflare-dns.com
104.21.88.221			0ms.dev
45.90.28.0			anycast.dns.nextdns.io
104.16.133.229			dns.cloudflare.com
146.112.41.2			doh.opendns.com
####			kaitain.restena.lu
137.66.7.89			max.rethinkdns.com
76.76.2.11			freedns.controld.com
149.248.217.117			dns.dnswarden.com
#Encrypt DNS End
# Last Update Time : 2024-10-06 00:27:41 

#EA Start
23.39.184.174			www.ea.com
23.54.127.81			origin-a.akamaihd.net
23.62.165.14			pl.ea.com
23.213.94.171			media.contentapi.ea.com
23.62.165.14			nds-network-nav.ea.com
#EA End
# Last Update Time : 2024-10-06 00:27:41 

#gitlab Start
172.65.251.78			gitlab.com
172.65.251.78			www.gitlab.com
104.17.73.206			page.gitlab.com
104.18.39.11			packages.gitlab.com
104.18.248.37			support.gitlab.com
104.18.39.11			customers.gitlab.com
172.65.216.50			staging.gitlab.com
216.198.54.1			federal-support.gitlab.com
35.227.35.254			registry.gitlab.com
172.64.32.97			evelup.gitlab.com
104.18.39.11			chef.gitlab.com
#gitlab End
# Last Update Time : 2024-10-06 00:27:41 

#debian Start
146.75.38.132			deb.debian.org
#debian End
# Last Update Time : 2024-10-06 00:27:41 

#iwara Start
172.67.71.154			iwara.tv
62.210.173.23			himeko.iwara.tv
104.26.13.96			i.iwara.tv
104.26.13.96			www.iwara.tv
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
# Last Update Time : 2024-10-06 00:27:42 

#EPIC Start
3.167.88.28			download2.epicgames.com
3.162.103.22			download3.epicgames.com
99.84.191.21			download4.epicgames.com
3.167.88.44			download.epicgames.com
23.54.127.74			epicgames-download1.akamaized.net
52.85.132.86			epic-social-social-modules-prod.ol.epicgames.com
54.92.235.248			eulatracking-public-service-prod06.ol.epicgames.com
3.162.112.109			media-cdn.epicgames.com
23.222.201.130			static-assets-prod.epicgames.com
23.49.189.95			store-content.ak.epicgames.com
35.170.29.122			tracking.epicgames.com
#EPIC End
# Last Update Time : 2024-10-06 00:27:42 

#google Start
172.253.115.94			update.googleapis.com
142.251.167.95			translate-pa.googleapis.com
64.233.180.101			translate.google.com
142.251.163.95			firebaseinstallations.googleapis.com
142.250.31.95			infinitedata-pa.googleapis.com
142.251.163.95			geller-pa.googleapis.com
209.85.202.188			alt1.mobile-gtalk.l.google.com
64.233.184.188			alt2.mobile-gtalk4.l.google.com
142.250.27.188			alt3.mobile-gtalk.l.google.com
142.250.153.188			alt4.mobile-gtalk4.l.google.com
142.251.9.188			alt5.mobile-gtalk.l.google.com
142.250.150.188			alt6.mobile-gtalk4.l.google.com
74.125.200.188			alt7.mobile-gtalk.l.google.com
142.250.157.188			alt8.mobile-gtalk4.l.google.com
172.253.115.95			translate.googleapis.com
64.233.180.100			www3.l.google.com
142.250.31.94			services.googleapis.cn
142.251.167.102			play-fe.googleapis.com
142.251.163.119			play-lh.googleusercontent.com
216.239.38.223			play.googleapis.com
209.85.202.188			alt1-mtalk.google.com
64.233.184.188			alt2-mtalk.google.com
142.250.27.188			alt3-mtalk.google.com
142.250.153.188			alt4-mtalk.google.com
142.251.9.188			alt5-mtalk.google.com
142.250.150.188			alt6-mtalk.google.com
74.125.200.188			alt7-mtalk.google.com
142.250.157.188			alt8-mtalk.google.com
142.251.179.95			content-autofill.googleapis.com
172.253.115.94			googlecn-lopri.l.google.com
142.251.16.94			www.googleapis.cn
#google End
# Last Update Time : 2024-10-06 00:27:42 

#xbox Start
23.62.164.9			gameclipscontent-d2009.xboxlive.com
23.218.218.138			images-eds.xboxlive.com
23.215.0.234			xbl-smooth.xboxlive.com
23.62.164.9			titlehub.xboxlive.com
23.218.218.133			compass.xboxlive.com
23.62.164.9			xnotify.xboxlive.com
52.165.145.141			activityhub.xboxlive.com
23.62.164.9			images-eds-ssl.xboxlive.com
199.46.35.121			rta.xboxlive.com
23.45.148.9			peoplehub.xboxlive.com
52.242.98.79			editorial.xboxlive.com
23.218.218.191			assets1.xboxlive.cn
23.218.218.180			assets2.xboxlive.cn
20.70.246.20			xboxlive.com
13.107.246.41			da.xboxservices.com
20.109.105.194			device.auth.xboxlive.com
#xbox End
# Last Update Time : 2024-10-06 00:27:42 

#Apkpure Start
172.67.20.93			download.pureapk.com
104.22.8.141			api.pureapk.com
104.22.43.111			t.apkpure.net
104.22.9.141			tapi.pureapk.com
104.22.8.141			rdelivery.pureapk.com
104.26.13.136			tapi.upload.app
45.33.36.159			api.sve.cc
#Apkpure End
# Last Update Time : 2024-10-06 00:27:43 

#Microsoft Start
20.190.151.69			login.microsoftonline.com
13.85.23.206			fe3cr.delivery.mp.microsoft.com
20.97.190.214			fe2cr.update.microsoft.com
4.245.163.56			slscr.update.microsoft.com
23.54.127.49			dl.delivery.mp.microsoft.com
4.249.200.148			nav-edge.smartscreen.microsoft.com
20.190.151.38			graph.microsoft.com
23.62.166.208			go.microsoft.com
13.107.246.41			static.edge.microsoftapp.net
204.79.197.203			oneocsp.microsoft.com
52.228.161.161			nf.smartscreen.microsoft.com
20.253.175.208			wdcp.microsoft.com
52.109.8.89			officeclient.microsoft.com
20.42.7.128			api-edge.cognitive.microsofttranslator.com
204.79.197.239			edge.microsoft.com
23.62.165.205			storeedgefd.dsx.mp.microsoft.com
152.195.19.97			msedgeextensions.sf.tlu.dl.delivery.mp.microsoft.com
#Microsoft End
# Last Update Time : 2024-10-06 00:27:43 

#spotify Start
104.199.241.202			ap-gae2.spotify.com
104.154.127.247			ap-guc3.spotify.com
104.199.65.9			ap-gew1.spotify.com
34.158.1.133			ap-gew4.spotify.com
34.158.255.62			ap-gue1.spotify.com
35.186.224.24			spclient.wg.spotify.com
35.186.224.24			wg.spotify.com
35.186.224.22			gae-spclient.spotify.com
23.205.105.36			audio4-ak-spotify-com.akamaized.net
184.25.127.87			heads4-ak-spotify-com.akamaized.net
23.205.105.18			audio-ak-spotify-com.akamaized.net
23.205.105.7			audio-akp-quic-spotify-com.akamaized.net
#spotify End
# Last Update Time : 2024-10-06 00:27:43 

#scdn Start
199.232.210.248			audio-fa.scdn.co
23.205.105.26			misc.scdn.co
23.205.105.26			i.scdn.co
199.232.214.248			newjams-images.scdn.co
199.232.210.248			dailymix-images.scdn.co
199.232.210.248			thisis-images.scdn.co
199.232.210.248			charts-images.scdn.co
199.232.214.248			seeded-session-images.scdn.co
199.232.210.248			download.scdn.co
#scdn End
# Last Update Time : 2024-10-06 00:27:43 

#onedrive Start
13.107.139.11			onedrive.live.com
13.107.42.12			skyapi.onedrive.live.com
23.9.161.55			api.onedrive.live.com
#onedrive End
# Last Update Time : 2024-10-06 00:27:43 

#other Start
35.174.192.160			www.ghostery.com
35.174.192.160			ghostery.com
104.233.133.90			wap.yushuwu.cloud
#other End
# Last Update Time : 2024-10-06 00:27:43 

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
