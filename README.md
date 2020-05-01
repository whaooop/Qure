[URL Rewrite]
# Redirect Google Search Service
^https?:\/\/(www.)?(g|google)\.cn https://www.google.com 302
# Redirect HTTP to HTTPS
^https?:\/\/(www.)?taobao\.com\/ https://taobao.com/ 302
^https?:\/\/(www.)?jd\.com\/ https://www.jd.com/ 302
^https?:\/\/(www.)?mi\.com\/ https://www.mi.com/ 302
^https?:\/\/you\.163\.com\/ https://you.163.com/ 302
^https?:\/\/(www.)?suning\.com/ https://suning.com/ 302
^https?:\/\/(www.)?yhd\.com https://yhd.com/ 302
# Redirect False to True
# > IGN China to IGN Global
^https?:\/\/(www.)?ign\.xn--fiqs8s\/ http://cn.ign.com/ccpref/us 302
# > Fake Website Made By C&J Marketing
^https?:\/\/(www.)?abbyychina\.com\/ https://www.abbyy.cn/ 302
^https?:\/\/(www.)?bartender\.cc\/ https://www.macbartender.com/ 302
^https?:\/\/(www.)?(betterzipcn|betterzip)\.(com|net)\/ https://macitbetter.com/ 302
^https?:\/\/(www.)?beyondcompare\.cc\/ https://www.scootersoftware.com/ 302
^https?:\/\/(www.)?bingdianhuanyuan\.cn\/ https://www.faronics.com/zh-hans/products/deep-freeze 302
^https?:\/\/(www.)?chemdraw\.com\.cn\/ https://www.perkinelmer.com.cn/ 302
^https?:\/\/(www.)?codesoftchina\.com\/ https://www.teklynx.com/ 302
^https?:\/\/(www.)?coreldrawchina\.com\/ https://www.coreldraw.com/cn/ 302
^https?:\/\/(www.)?crossoverchina\.com\/ https://www.codeweavers.com/ 302
^https?:\/\/(www.)?dongmansoft\.com\/ https://www.udongman.cn/ 302
^https?:\/\/(www.)?earmasterchina\.cn\/ https://www.earmaster.com/ 302
^https?:\/\/(www.)?easyrecoverychina\.com\/ https://www.ontrack.com/ 302
^https?:\/\/(www.)?ediuschina\.com\/ https://www.grassvalley.com/ 302
^https?:\/\/(www.)?flstudiochina\.com\/ https://www.image-line.com/ 302
^https?:\/\/(www.)?formysql\.com\/ https://www.navicat.com.cn/ 302
^https?:\/\/(www.)?guitarpro\.cc\/ https://www.guitar-pro.com/ 302
^https?:\/\/(www.)?huishenghuiying\.com\.cn\/ https://www.coreldraw.com/cn/ 302
^https?:\/\/hypersnap\.mairuan\.com\/ https://www.hyperionics.com/ 302
^https?:\/\/(www.)?iconworkshop\.cn\/ https://www.axialis.com/ 302
^https?:\/\/(www.)?imindmap\.cc\/ https://www.ayoa.com/previously-imindmap/ 302
^https?:\/\/(www.)?jihehuaban\.com\.cn\/ https://www.chartwellyorke.com/sketchpad/x24795.html header
^https?:\/\/hypersnap\.mairuan\.com\/ https://www.keyshot.com/ 302
^https?:\/\/(www.)?kingdeecn\.cn\/ http://www.kingdee.com/ 302
^https?:\/\/(www.)?logoshejishi\.com https://www.sothink.com/product/logo-design-software/ 302
^https?:\/\/logoshejishi\.mairuan\.com\/ https://www.sothink.com/product/logo-design-software/ 302
^https?:\/\/(www.)?luping\.net\.cn\/ https://www.techsmith.com/ 302
^https?:\/\/(www.)?mathtype\.cn\/ https://www.dessci.com/ 302
^https?:\/\/(www.)?mindmanager\.(cc|cn)\/ https://www.mindjet.com/cn/ 302
^https?:\/\/(www.)?mindmapper\.cc\/ https://www.mindmapper.com/ 302
^https?:\/\/(www.)?mycleanmymac\.com\/ https://macpaw.com/ 302
^https?:\/\/(www.)?nicelabel\.cc\/ https://www.nicelabel.com/zh/ 302
^https?:\/\/(www.)?ntfsformac\.cc\/ https://www.tuxera.com/products/tuxera-ntfs-for-mac-cn/ 302
^https?:\/\/(www.)?ntfsformac\.cn\/ https://china.paragon-software.com/home-mac/ntfs-for-mac/ 302
^https?:\/\/(www.)?overturechina\.com\/ https://sonicscores.com/ 302
^https?:\/\/(www.)?passwordrecovery\.cn\/ https://cn.elcomsoft.com/aopr.html 302
^https?:\/\/(www.)?pdfexpert\.cc\/ https://pdfexpert.com/zh 302
^https?:\/\/(www.)?photozoomchina\.com\/ https://www.benvista.com/ 302
^https?:\/\/(www.)?shankejingling\.com\/ https://www.sothink.com/product/flashdecompiler/ 302
^https?:\/\/cn\.ultraiso\.net\/ https://cn.ezbsystems.com/ultraiso/ 302
^https?:\/\/(www.)?vegaschina\.cn\/ https://www.vegascreativesoftware.com/ 302
^https?:\/\/(www.)?xshellcn\.com\/ https://www.netsarang.com/zh/xshell/ 302
^https?:\/\/(www.)?yuanchengxiezuo\.com\/ https://www.teamviewer.com/ 302
^https?:\/\/(www.)?zbrushcn.com/ https://pixologic.com/ 302
# TikTok (By Choler & Paris ^_^)
(.*video_id=\w{32})(.*watermark=)(.*) $1 302
(?<=(carrier|account|sys)_region=)CN JP 307
# (?<=version_code=)\d{1,}.\d{1}\.\d{1} 8.4.0 307
# Resso (By JO2EY)
(?<=(carrier|account|sys|sim)_region=)cn in 307
# Advertising Block
# 0~9
# > 21经济
^https?:\/\/api\.21jingji\.com\/ad\/ - reject
# > 360doc
^https?:\/\/mobi\.360doc\.com\/v\d{2}\/Ajax\/festival\.ashx\?op=getfestivaltheme - reject
# > 58同城
^https?:\/\/app\.58\.com\/api\/home\/(advertising|appadv)\/ - reject
^https?:\/\/app\.58\.com\/api\/home\/invite\/popupAdv - reject
^https?:\/\/app\.58\.com\/api\/log\/ - reject
^https?:\/\/.+\.58cdn\.com\.cn\/brandads\/ - reject
# A
# > 阿里巴巴
# >> 闲鱼
^https?:\/\/acs\.m\.taobao\.com\/gw\/mtop\.taobao\.idle\.home\.welcome\/ - reject
# >> 飞猪
^https?:\/\/acs\.m\.taobao\.com\/gw\/mtop\.trip\.activity\.querytmsresources\/ - reject
# >> 淘票票
^https?:\/\/acs\.m\.taobao\.com\/gw\/mtop\.film\.mtopadvertiseapi\.queryadvertise\/ - reject
# >> 口碑
^https?:\/\/render\.alipay\.com\/p\/s\/h5data\/prod\/spring-festival-2019-h5data\/popup-h5data\.json - reject
^https?:\/\/acs\.m\.taobao\.com\/gw\/mtop\.o2o\.ad\.gateway\.get\/ - reject
^https?:\/\/guide-acs\.m\.taobao\.com\/gw\/mtop\.taobao\.wireless\.home\.splash\.awesome\.get\/ - reject
# >> 高德地图
^https?:\/\/m\d\.amap\.com\/ws\/valueadded\/alimama\/splash_screen\/ - reject
# >> 优酷
^https?:\/\/.+\.mp4\?ccode=0902 - reject
^https?:\/\/.+\.mp4\?sid= - reject
^https?:\/\/vali\.cp31\.ott\.cibntv\.net\/youku\/.+\.mp4\?sid= - reject
# > AcFun
^https?:\/\/aes\.acfun\.cn\/s\?adzones - reject
# > 爱回收
^https?:\/\/gw\.aihuishou\.com\/app-portal\/home\/getadvertisement - reject
# > APICloud
^https?:\/\/a\.apicloud\.com\/start_page\/ - reject
# B
# > 百度
# >> 百度网盘
^https?:\/\/pan\.baidu\.com\/rest\/2.0\/pcs\/adx - reject
^https?:\/\/pan\.baidu\.com\/act\/api\/activityentry - reject
^https?:\/\/issuecdn\.baidupcs\.com\/issue\/netdisk\/guanggao\/ - reject
# >> 百度贴吧
^https?:\/\/c\.tieba\.baidu\.com\/c\/s\/splashSchedule - reject
^https?:\/\/c\.tieba\.baidu\.com\/c\/f\/forum\/getAdInfo - reject
^https?:\/\/c\.tieba\.baidu\.com\/\w+\/\w+\/(sync|newRnSync|mlog) - reject
# >> 百度地图
# ^https?:\/\/.+\/client\/phpui2\/ - reject
^https?:\/\/ss0\.bdstatic\.com/.+_\d{3}_\d{4}\.jpg - reject
# >> 爱奇艺
^https?:\/\/iface\.iqiyi\.com\/api\/getNewAdInfo - reject
^https?:\/\/.+\/(mixer|track2)\? - reject
^https?:\/\/act\.vip\.iqiyi\.com\/interact\/api\/show.do - reject
^https?:\/\/act\.vip\.iqiyi\.com\/interact\/api\/v2\/show - reject
# > 哔哩哔哩
^https?:\/\/app\.bilibili\.com\/x\/v\d\/splash\/ - reject
^https?:\/\/manga\.bilibili\.com\/twirp\/comic\.v\d\.Comic\/Flash - reject
# > 抱抱
^https?:\/\/www\.myhug\.cn\/ad\/ - reject
# > 百词斩
^https?:\/\/7n\.bczcdn\.com\/launchad\/ - reject
# > 贝太厨房
^https?:\/\/channel\.beitaichufang\.com\/channel\/api\/v\d\/promote\/ios\/start\/page - reject
# > 币世界
^https?:\/\/iapi\.bishijie\.com\/actopen\/advertising\/ - reject
# > 贝壳找房
^https?:\/\/app\.api\.ke\.com\/config\/config\/bootpage - reject
# > 薄荷
^https?:\/\/status\.boohee\.com\/api\/v\d\/app_square\/start_up_with_ad - reject
# C
# > CNTV
^https?:\/\/cntv\.hls\.cdn\.myqcloud\.com\/.+\?maxbr=850 - reject
^https?:\/\/asp\.cntv\.myalicdn\.com\/.+\?maxbr=850 - reject
^https?:\/\/www\.cntv\.cn\/nettv\/adp\/ - reject
^https?:\/\/v\.cctv\.com\/.+850 - reject
# > 车来了
^https?:\/\/api\.chelaile\.net\.cn\/adpub\/ - reject
# ^https?:\/\/(api|atrace)\.chelaile\.net\.cn\/adpub\/ - reject
^https?:\/\/api\.chelaile\.net\.cn\/goocity\/advert\/ - reject
# ^https?:\/\/atrace\.chelaile\.net\.cn\/exhibit\?&adv_image - reject
^https?:\/\/pic\d\.chelaile\.net\.cn\/adv\/ - reject
# > 曹操出行
^https?:\/\/cap\.caocaokeji\.cn\/advert-bss\/ - reject
# > 财经
^https?:\/\/api\.caijingmobile\.com\/(ad|advert)\/ - reject
# > 超级课程表
^https?:\/\/.+/V\d\/splash\/getSplashV\d\.action - reject
# > 超级星饭团
^https?:\/\/g\.cdn\.pengpengla\.com\/starfantuan\/boot-screen-info\/ - reject
# D
# > 豆瓣 (154.8.131.* 自签证书不可用)
^https?:\/\/api\.douban\.com\/v\d\/app_ads\/ - reject
# > 斗鱼
^https?:\/\/rtbapi\.douyucdn\.cn\/japi\/sign\/app\/getinfo - reject
# > 当当
^https?:\/\/mapi\.dangdang\.com\/index\.php\?action=init - reject
^https?:\/\/e\.dangdang\.com\/.+getDeviceStartPage - reject
# > 蛋蛋赞
^https?:\/\/www\.dandanzan\.com\/res\/gdsefse\.js - reject
# > 叨鱼
^https?:\/\/daoyu\.sdo\.com\/api\/userCommon\/getAppStartAd - reject
# > 丁香医生
^https?:\/\/dxy\.com\/app\/i\/ask\/biz\/feed\/launch - reject
# > 嘀嗒出行
^https?:\/\/capis(-slb)?\.didapinche\.com\/ad\/ - reject
^https?:\/\/www\.didapinche\.com\/app\/adstat\/ - reject
# > 电视家
^https?:\/\/api\.gaoqingdianshi\.com\/api\/v\d\/ad\/ - reject
# E
# > 艺龙 (123.59.31.1,119.18.193.135)
# (仅 Surge 可用因其支持 force-http-engine-hosts)
^https?:\/\/((25[0-5]|2[0-4]\d|1\d{2}|[1-9]?\d)\.){3}(25[0-5]|2[0-4]\d|1\d{2}|[1-9]?\d)\/(adgateway|adv)\/ - reject
# > e代驾
^https?:\/\/pic\.edaijia\.cn\/adsplash\/ - reject
# F
# > Foodie
^https?:\/\/foodie-api\.yiruikecorp\.com\/v\d\/(banner|notice)\/overview - reject
# > FOTOABLE
^https?:\/\/cdn\.api\.fotoable\.com\/Advertise\/ - reject
# > 飞客茶馆
^https?:\/\/www\.flyertea\.com\/source\/plugin\/mobile\/mobile\.php\?module=advis - reject
# > 飞常准
^https?:\/\/app\.variflight\.com\/ad\/ - reject
^https?:\/\/app\.variflight\.com\/v\d\/advert\/ - reject
# > 凤凰秀
^https:\/\/dsa-mfp\.fengshows\.cn\/mfp\/mfpMultipleDelivery\.do\?.+adunitid - reject
# G
# > Google
^https?:\/\/.+\.googlevideo\.com\/.+(&oad|ctier) - reject
^https?:\/\/youtubei\.googleapis\.com\/youtubei\/.+ad_ - reject
^https?:\/\/\w+\.youtube\.com\/api\/stats\/(ads|.+adformat) - reject
^https?:\/\/\w+\.youtube\.com\/(pagead|ptracking) - reject
# > Gofun
^https?:\/\/gateway\.shouqiev\.com\/fsda\/app\/bootImage\.json - reject
# > 国泰君安
^https?:\/\/dl\.app\.gtja\.com\/dzswem\/kvController\/.+\.jpg$ - reject
# H
# > 杭州公交
^https?:\/\/m\.ibuscloud.com\/v2\/app\/getStartPage - reject
# > 杭州市·市民卡
^https?:\/\/smkmp\.96225.com\/smkcenter\/ad/ - reject
# > 虎扑
^https?:\/\/games\.mobileapi\.hupu\.com\/.+\/(interfaceAdMonitor|interfaceAd)\/ - reject
^https?:\/\/business\.msstatic\.com\/advertiser\/ - reject
# > 韩剧社
^https?:\/\/47\.97\.20\.12\/ad\/ - reject
# > 火猫
^https?:\/\/api\.huomao\.com\/channels\/loginAd - reject
# > HiveBox
^https?:\/\/consumer\.fcbox\.com\/v\d\/ad\/ - reject
# > 好好住
^https?:\/\/api\.haohaozhu\.cn\/index\.php\/home\/AppInit\/getStartPhoto - reject
# > 花生地铁
^https?:\/\/cmsapi\.wifi8\.com\/v\d\/(emptyAd|adNew)\/ - reject
# I
# > 讯飞
^https?:\/\/imeclient\.openspeech\.cn\/adservice\/ - reject
# > 好体知
^https?:\/\/www\.bodivis\.com\.cn\/app\/splashAdvertise - reject
# J
# > 京东
^https?:\/\/api\.m\.jd.com\/client\.action\?functionId=(start|queryMaterialAdverts) - reject
^https?:\/\/(bdsp-x|dsp-x)\.jd\.com\/adx\/ - reject
^https?:\/\/ms\.jr\.jd\.com\/gw\/generic\/base\/na\/m\/adInfo - reject
^https?:\/\/ms\.jr\.jd\.com\/gw\/generic\/aladdin\/na\/m\/getLoadingPicture - reject
# > 界面新闻
^https?:\/\/img\.jiemian\.com\/ads\/ - reject
# > 驾校一点通
^https?:\/\/api\.jxedt\.com\/ad\/ - reject
^https?:\/\/richmanapi\.jxedt\.com\/api\/ad\/ - reject
# > 驾考宝典
^https?:\/\/.+\.kakamobi\.cn\/api\/open\/v\d\/advert-sdk\/ - reject
# > 金山 WPS
^https?:\/\/ios\.wps\.cn\/ad-statistics-service - reject
^https?:\/\/mobile-pic\.cache\.iciba\.com\/feeds_ad\/ - reject
^https?:\/\/\w+\.kingsoft-office-service\.com\/ad - reject
# > 金山词霸
^https?:\/\/dict-mobile\.iciba\.com\/interface\/index\.php\?.+(c=ad|collectFeedsAdShowCount|KSFeedsAdCardViewController) - reject
^https?:\/\/service\.iciba\.com\/popo\/open\/screens\/v\d\?adjson - reject
# K
# > Keep
^https?:\/\/api\.gotokeep\.com\/ads - reject
# > 快看漫画
^https?:\/\/api\.kkmh\.com\/.+(ad|advertisement)\/ - reject
# > 酷我 (122.14.246.33,175.102.178.52)
# (仅 Surge 可用因其支持 force-http-engine-hosts)
^https?:\/\/((25[0-5]|2[0-4]\d|1\d{2}|[1-9]?\d)\.){3}(25[0-5]|2[0-4]\d|1\d{2}|[1-9]?\d)\/MobileAdServer\/ - reject
^https?:\/\/((25[0-5]|2[0-4]\d|1\d{2}|[1-9]?\d)\.){3}(25[0-5]|2[0-4]\d|1\d{2}|[1-9]?\d)\/EcomResourceServer/AdPlayPage/adinfo - reject
# > 看理想
^https?:\/\/api\.vistopia\.com\.cn\/api\/v\d\/home\/advertisement - reject
# L
# > 乐视
^https?:\/\/.+\/letv-gug\/ - reject
# > 来疯直播
^https?:\/\/api\.laifeng\.com\/v\d\/start\/ads - reject
# > 懒投资
^https?:\/\/ios\.lantouzi\.com\/api\/startpage - reject
# M
# > 小米
^https?:\/\/api\.m\.mi\.com\/v\d\/app\/start - reject
^https?:\/\/api\.jr\.mi\.com\/v\d\/adv\/ - reject
^https?:\/\/api\.jr\.mi\.com\/jr\/api\/playScreen - reject
^https?:\/\/api-mifit.+\.huami\.com\/discovery\/mi\/discovery\/.+_ad\? - reject
# > 蘑菇租房
^https?:\/\/api\.mgzf\.com\/renter-operation\/home\/startHomePage - reject
# > 墨迹天气
^https?:\/\/cdn\.moji\.com\/(adoss|adlink)\/ - reject
# > 埋堆堆
^https?:\/\/mob\.mddcloud\.com\.cn\/api\/(ad|advert)\/ - reject
# > 漫画人
^https?:\/\/mangaapi\.manhuaren\.com\/v\d\/public\/getStartPageAds - reject
# > 美团
^https?:\/\/img\.meituan\.net\/(adunion|display|midas)\/.+\.(gif|jpg|jpg\.webp)$ - reject
^https?:\/\/p\d\.meituan\.net\/wmbanner\/[A-Za-z0-9]+\.jpg - reject
^https?:\/\/p\d\.meituan\.net\/movie\/[A-Za-z0-9]+\.jpg\?may_covertWebp - reject
^https?:\/\/s3plus\.meituan\.net\/.+\/linglong\/.+\.(gif|jpg|mp4) - reject
# > 美味不用等
^https?:\/\/capi.mwee.cn/app-api/V\d{2}/app/(ad|getstartad) - reject
# > 秒拍
^https?:\/\/b-api\.ins\.miaopai\.com\/\d\/ad/ - reject
# > 马蜂窝
^https?:\/\/mapi\.mafengwo\.cn\/ad\/ - reject
^https?:\/\/mapi\.mafengwo\.cn\/travelguide\/ad\/ - reject
# N
# > 爱南宁
^https?:\/\/nnapp\.cloudbae\.cn\/mc\/api\/advert/ - reject
# > NationalGeographic
^https?:\/\/dili\.bdatu\.com\/jiekou\/ad\/ - reject
# > NationalGeographicChina
^https?:\/\/wap\.ngchina\.cn\/news\/adverts\/ - reject
# O
# > ofo
^https?:\/\/supportda\.ofo\.com\/adaction\? - reject
^https?:\/\/ma\.ofo\.com\/ads\/ - reject
^https?:\/\/activity2\.api\.ofo\.com\/ofo\/Api\/v2\/ads - reject
^https?:\/\/ma\.ofo\.com\/adImage\/ - reject
# > Oray
^https?:\/\/slapi\.oray\.net\/client\/ad - reject
# P
# > 票根
^https?:\/\/pss\.txffp\.com\/piaogen\/images\/launchScreen/ - reject
# > 拼多多
^https?:\/\/api\.yangkeduo\.com\/api\/cappuccino\/splash - reject
# Q
# > Qdaily
^https?:\/\/app\d\.qdaily\.com\/app\d\/boot_advertisements\.json - reject
^https?:\/\/notch\.qdaily\.com\/api\/v\d\/boot_ad - reject
# > 穷游
^https?:\/\/open\.qyer\.com\/qyer\/startpage\/ - reject
^https?:\/\/open\.qyer\.com\/qyer\/config\/get - reject
^https?:\/\/media\.qyer\.com\/ad\/ - reject
# > 亲宝宝
^https?:\/\/api\.qbb6\.com\/ad\/ - reject
# R
# > 人人视频
^https?:\/\/msspjh\.emarbox\.com\/getAdConfig - reject
^https?:\/\/api\.videozhishi\.com\/api\/getAdvertising - reject
^https?:\/\/api\.rr\.tv\/ad\/ - reject
# > 人人影视
^https?:\/\/ctrl\.(playcvn|zmzapi)\.(com|net)\/app\/(ads|init) - reject
# > 日日煮
^https?:\/\/api\.daydaycook\.com\.cn\/daydaycook\/server\/ad\/ - reject
^https?:\/\/cms\.daydaycook\.com\.cn\/api\/cms\/advertisement\/ - reject
# S
# > 搜狐
^https?:\/\/api\.k\.sohu\.com\/api\/news\/adsense - reject
^https?:\/\/pic\.k\.sohu\.com\/img8\/wb\/tj\/ - reject
^https?:\/\/s1\.api\.tv\.itc\.cn\/v4\/mobile\/control\/switch\.json - reject
^https?:\/\/api\.tv\.sohu\.com\/agg\/api\/app\/config\/bootstrap - reject
# > 什么值得买
^https?:\/\/api\.smzdm\.com\/v\d\/util\/loading - reject
^https?:\/\/app-api\.smzdm\.com\/util\/loading - reject
^https?:\/\/s\d\.zdmimg\.com\/www\/api\/v\d\/api\/thirdAd\.php - reject
# > 四季線上影視4gTV
^https?:\/\/service\.4gtv\.tv\/4gtv\/Data\/(GetAD|ADLog) - reject
# > 肆客足球
^https?:\/\/api\.qiuduoduo\.cn\/guideimage - reject
# > 识货
^https?:\/\/www\.shihuo\.cn\/app\d\/saveAppInfo - reject
# > 首汽约车
^https?:\/\/gw-passenger\.01zhuanche\.com\/gw-passenger\/car-rest\/webservice\/passenger\/recommendADs - reject
^https?:\/\/gw-passenger\.01zhuanche\.com\/gw-passenger\/zhuanche-passenger-token\/leachtoken\/webservice\/homepage\/queryADs - reject
# > 苏宁
^https?:\/\/image\.suning\.cn\/uimg\/ma\/ad\/ - reject
# > 神舟专车
^https?:\/\/img01\.10101111cdn\.com\/adpos\/ - reject
# > 扫描全能王
^https?:\/\/api\.intsig\.net\/user\/cs\/operating\/app\/get_startpic\/ - reject
# > 省点
^https?:\/\/api\.waitwaitpay\.com\/\/api\/splash - reject
# > 搜狗
^https?:\/\/business-cdn\.shouji\.sogou\.com\/wapdl\/hole\/.+\.jpg - reject
# T
# > 腾讯
# >> 富途牛牛
^https?:\/\/api\d\.futunn\.com\/ad\/ - reject
# >> 腾讯游戏
^https?:\/\/ssl\.kohsocialapp\.qq\.com:10001\/game\/buttons - reject
^https?:\/\/qt\.qq\.com\/lua\/mengyou\/get_splash_screen_info - reject
# >> 腾讯地图
^https?:\/\/3gimg\.qq\.com\/tencentMapTouch\/app\/activity\/ - reject
^https?:\/\/3gimg\.qq\.com\/tencentMapTouch\/splash\/ - reject
^https?:\/\/4gimg\.map\.qq\.com\/mwaSplash\/ - reject
# >> 腾讯视频
^https?:\/\/btrace.qq.com - reject
^https?:\/\/vv\.video\.qq\.com\/getvmind\? - reject
# ^https?:\/\/.+\.mp4.+&sdtfrom=v3004 - reject
^https?:\/\/((25[0-5]|2[0-4]\d|1\d{2}|[1-9]?\d)\.){3}(25[0-5]|2[0-4]\d|1\d{2}|[1-9]?\d)\/.+\.tc\.qq\.com\/.+p201\.1\.mp4\? - reject
# >> 腾讯新闻
^https?:\/\/r\.inews\.qq\.com\/(adsBlacklist|getFullScreenPic|getQQNewsRemoteConfig) - reject
# >> 腾讯体育
^https?:\/\/news\.ssp\.qq\.com\/app - reject
# >> 微信
^https?:\/\/mp\.weixin\.qq\.com\/mp\/(ad_|advertisement|getappmsgad) - reject
# > 澎湃新闻
^https?:\/\/adpai\.thepaper\.cn\/.+&ad= - reject
# > 太平洋
^https?:\/\/agent-count\.pconline\.com\.cn\/counter\/adAnalyse\/ - reject
^https?:\/\/mrobot\.pconline\.com\.cn\/v\d\/ad2p - reject
^https?:\/\/mrobot\.pconline\.com\.cn\/s\/onlineinfo\/ad\/ - reject
^https?:\/\/mrobot\.pcauto\.com\.cn\/v\d\/ad2p - reject
^https?:\/\/mrobot\.pcauto\.com\.cn\/xsp\/s\/auto\/info\/preload\.xsp - reject
# > 途牛
^https?:\/\/m\.tuniu\.com\/api\/operation\/splash\/ - reject
# V
# > VUE
^https?:\/\/static\.vuevideo\.net\/styleAssets\/.+\/splash_ad - reject
^https?:\/\/static\.vuevideo\.net\/styleAssets\/advertisement\/ - reject
# W
# > 网易
# >> 网易邮箱
^https?:\/\/appconf\.mail\.163\.com\/mmad\/ - reject
# >> 网易新闻
^https?:\/\/c\.m\.163\.com\/nc\/gl\/ - reject
# >> 网易有钱
^https?:\/\/client\.mail\.163\.com\/apptrack\/confinfo\/searchMultiAds - reject
# >> 网易云音乐
^https?:\/\/.+\/eapi\/(ad|log)\/ - reject
# >> 网易考拉
^https?:\/\/sp\.kaola\.com\/api\/openad - reject
# >> 网易严选
^https?:\/\/support\.you\.163\.com\/xhr\/boot\/getBootMedia\.json - reject
# >> 网易蜗牛读书
^https?:\/\/easyreadfs\.nosdn\.127\.net\/ad-material\/ - reject
^https?:\/\/p\.du\.163\.com\/ad\/ - reject
# >> 有道词典
^https?:\/\/oimage([a-z])([0-9])\.ydstatic\.com\/.+adpublish - reject
^https?:\/\/dsp-impr2\.youdao\.com\/adload.s\? - reject
# > 微医
^https?:\/\/app\.wy\.guahao\.com\/json\/white\/dayquestion\/getpopad - reject
# > Weico
^https?:\/\/overseas\.weico\.cc/portal\.php\?a=get_coopen_ads - reject
# > 无他相机
^https?:\/\/api-release\.wuta-cam\.com\/ad_tree - reject
^https?:\/\/res-release\.wuta-cam\.com\/json\/ads_component_cache\.json - reject
# > 蜗牛睡眠
^https?:\/\/snailsleep\.net\/snail\/v\d\/screen\/qn\/get\? - reject
^https?:\/\/snailsleep\.net\/snail\/v\d\/adTask\/ - reject
# > WiFi共享大师
^https?:\/\/nochange\.ggsafe\.com\/ad\/ - reject
# > 微店
^https?:\/\/thor\.weidian\.com\/ares\/home\.splash\/ - reject
# > 华尔街见闻
^https?:\/\/api\.wallstreetcn\.com\/apiv\d\/advertising\/ - reject
# > 威锋
^https?:\/\/api\.feng\.com\/v\d\/advertisement\/.*Claunch - reject
# X
# > 新浪
^https?:\/\/edit\.sinaapp\.com\/ua\?t=adv - reject
# >> 新浪微博
^https?:\/\/sdkapp\.uve\.weibo\.com\/interface\/sdk\/(actionad|sdkad)\.php - reject
^https?:\/\/wbapp\.uve\.weibo\.com\/wbapplua\/wbpullad\.lua - reject
^https?:\/\/weibointl\.api\.weibo\.cn\/portal\.php\?a=get_coopen_ads - reject
# >> 新浪天气通
^https?:\/\/tqt\.weibo\.cn\/overall\/redirect\.php\?r=tqt_sdkad - reject
^https?:\/\/tqt\.weibo\.cn\/overall\/redirect\.php\?r=tqtad - reject
^https?:\/\/tqt\.weibo\.cn\/.+advert\.index - reject
^https?:\/\/tqt\.weibo\.cn\/api\/advert\/ - reject
# > 下厨房
^https?:\/\/api\.xiachufang\.com\/v\d\/ad/ - reject
# > 虾米
^https?:\/\/acs\.m\.taobao\.com\/gw\/mtop\.alimusic\.common\.mobileservice\.startinit\/ - reject
# > 小睡眠
^https?:\/\/api\.psy-1\.com\/cosleep\/startup - reject
# > 迅游加速器
^https?:\/\/portal-xunyou\.qingcdn\.com\/api\/v\d\/ios\/configs\/(splash_ad|ad_urls) - reject
^https?:\/\/portal-xunyou\.qingcdn\.com\/api\/v\d\/ios\/ads\/ - reject
# > 喜马拉雅
^https?:\/\/\w+\.ximalaya\.com\/api\/v\d\/adRealTime - reject
^https?:\/\/((25[0-5]|2[0-4]\d|1\d{2}|[1-9]?\d)\.){3}(25[0-5]|2[0-4]\d|1\d{2}|[1-9]?\d)\/ting\/preload\/ - reject
# > 小站
^https?:\/\/tiku\.zhan\.com\/Common\/newAd\/ - reject
# Y
# > Yahoo!
^https?:\/\/m\.yap\.yahoo\.com\/v\d{2}\/getAds\.do - reject
# > Youtube++
^https?:\/\/api\.catch\.gift\/api\/v\d\/pagead\/ - reject
# > 萤石云视频
^https?:\/\/i\.ys7\.com\/api\/ads - reject
# > 运动世界
^https?:\/\/.+\.iydsj\.com\/api\/.+\/ad - reject
# > 一点万象
^https?:\/\/app\.mixcapp\.com\/mixc\/api\/v\d\/ad - reject
# > 印象笔记
^https?:\/\/app\.yinxiang\.com\/ads\/ - reject
# > 云麦好轻
^https?:\/\/restapi\.iyunmai\.com\/api\/ios\/ad\/ - reject
# > 育学园
^https?:\/\/yxyapi\d\.drcuiyutao\.com\/yxy-api-gateway\/api\/json\/advert\/ - reject
# > 迅雷
^https?:\/\/images\.client\.vip\.xunlei\.com\/.+\/advert\/ - reject
# > 讯飞
^https?:\/\/imeclient\.openspeech\.cn\/adservice\/ - reject
# Z
# > 直播吧
^https?:\/\/a\.qiumibao\.com\/activities\/config\.php - reject
^https?:\/\/.+\/allOne\.php\?ad_name - reject
# > 知乎
^https?:\/\/www\.zhihu\.com\/api\/v4\/community-ad\/ - reject
^https?:\/\/api\.zhihu\.com\/(launch|real_time) - reject
^https?:\/\/api\.zhihu\.com\/commercial_api\/(launch|real_time) - reject
^https?:\/\/api\.zhihu\.com\/fringe\/ad - reject
^https?:\/\/api\.zhihu\.com\/ad- - reject
# > 追书神器
^https?:\/\/(api|b)\.zhuishushenqi\.com\/advert - reject
^https?:\/\/api\.zhuishushenqi\.com\/splashes\/ios - reject
^https?:\/\/api\.zhuishushenqi\.com\/notification\/shelfMessage - reject
^https?:\/\/api\.zhuishushenqi\.com\/user\/bookshelf-updated - reject
^https?:\/\/itunes\.apple\.com\/lookup\?id=575826903 - reject
# > 作业帮
^https?:\/\/www\.zybang\.com\/adx\/ - reject
# > 最右
^https?:\/\/api\.izuiyou\.com\/ad\/ - reject
# > 字节跳动
^https?:\/\/.+\.pstatp\.com\/img\/ad - reject
^https?:\/\/.+\.(amemv|musical|snssdk|tiktokv)\.(com|ly)\/(api|motor)\/ad\/ - reject
^https?:\/\/dsp\.toutiao\.com\/api\/xunfei\/ads\/ - reject
^https?:\/\/.+\.snssdk\.com\/motor\/operation\/activity\/display\/config\/V2\/ - reject
^https?:\/\/.+/img\/ad\.union\.api\/ - reject
# > 中国银行
^https?:\/\/mlife\.jf365\.boc\.cn\/AppPrj\/FirstPic\.do\? - reject
# > 中信银行
^https?:\/\/m\.creditcard\.ecitic\.com\/citiccard\/mbk\/.+\/appStartAdv - reject
# > 中国工商银行
^https?:\/\/v\.icbc\.com\.cn\/userfiles\/Resources\/WAP\/advertisement\/ - reject
# > 中国招商银行
^https?:\/\/mlife\.cmbchina\.com\/ClientFaceService\/preCacheAdvertise\.json - reject
^https?:\/\/mlife\.cmbchina\.com\/ClientFaceService\/getAdvertisement\.json - reject
^https?:\/\/pic1cdn\.cmbchina\.com\/appinitads\/ - reject
# > 中国民生银行
^https?:\/\/www\.cmbc\.com\.cn\/m\/image\/loadingpage\/ - reject
# > 中国广发银行
^https?:\/\/mps\.95508\.com\/mps\/club\/cardPortals\/adv\/.{25}\.jpg - reject
# > 中国移动
# >> 手机营业厅
^https?:\/\/clientaccess\.10086\.cn\/biz-orange\/DN\/init\/startInit - reject
# >> 江苏
^https?:\/\/wap\.js\.10086\.cn\/jsmccClient\/cd\/market_content\/api\/v\d\/market_content\.page\.query - reject
# >> 咪咕
^https?:\/\/gg\w+\.cmvideo\.cn\/v\d\/iflyad\/ - reject
^https?:\/\/ggic(\d)?\.cmvideo\.cn\/ad\/ - reject
^https?:\/\/ggx\.cmvideo\.cn\/request\/ - reject
^https?:\/\/.+\/cdn-adn\/ - reject
# > 中国联通
^https?:\/\/m\.client\.10010\.com\/mobileService\/customer\/accountListData\.htm - reject
^https?:\/\/m\.client\.10010\.com\/uniAdmsInterface\/getWelcomeAd - reject
# > 掌阅
^https?:\/\/ih2\.ireader\.com\/zyapi\/bookstore\/ad\/ - reject
^https?:\/\/ih2\.ireader\.com\/zyapi\/self\/screen\/ad - reject
^https?:\/\/ih2\.ireader\.com\/zycl\/api\/ad\/ - reject
# CUSTOM URL
# custom url rewrite
^http:\/\/115\.com\/\?ct=sign$ http://115.com/lx?taskdg=1 header

[Header Rewrite]
^https?://zhidao\.baidu\.com header-replace User-Agent "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_6) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/12.0.2 Safari/605.1.15"
# CUSTOM HEADER
# custom header rewrite
