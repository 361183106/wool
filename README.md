﻿## 使用教程

【拉库】

    ql repo https://github.com/Yiov/wool.git "" "COOKIE"




## 小米刷步 xmsb.py

请第1次拉完库，自己新建一个py文件，不然每次都会覆盖！

例：
原本Yiov_wool_xmsb.py，新建一个xmsb.py，代码复制进去，再青龙重新task，原本的禁用


### 注册好小米运动账号，绑定第三方微信

手动修改py里面的数据

账号user = "138****8888"

密码passwd = "******"

直接输入想要修改的步数值，留空为随机步数

step = "23333"

step = str(random.randint(20000, 21000))

这个是随机的范围，自己改




## 机场签到 jcCheck.js

请第1次拉完库，自己新建一个py文件，不然每次都会覆盖！

例：
原本Yiov_wool_jcCheck.js，新建一个jcCheck.js

代码复制进去，再青龙重新task，原本的禁用




## 滴滴果园 ddgy.js

ddgyCOOKIE.js是CK文件，自己改


## 晶彩天气 jctq_daily.js

每小时2到3次


### 转发页定时宝箱/时段转发/刷福利视频/抽奖5次

抓GET包，点开福利页即可获取jctqCookie

https://tq.xunsl.com/v17/NewTask/getTaskListByWeather.json

链接转换：http://www.songluyi.com/ChangeHeaderToDict/

export jctqCookie=''


### 福利页定时宝箱

抓get包，点开福利页浮窗宝箱和观看翻倍视频获取body

https://tq.xunsl.com/v17/Weather/getBoxByweather.json

链接转换：http://www.songluyi.com/ChangeHeaderToDict/

export jctqGiveBoxBody=''



### 首页气泡红包

抓POST包，点开首页气泡红包和观看翻倍视频获取body

https://tq.xunsl.com/v5/weather/giveTimeInterval.json

链接转换：http://www.songluyi.com/ChangeHeaderToDict/

注：删除每个 : 后的空格后，再去转换。结尾处的User-Agent参数补完整，不然无效

export jctqBubbleBody=''


## 晶彩天气 jctq_reward.js

每天一次，放在其他脚本完成之后

签到和翻倍，任务奖励领取，统计今日收益，自动提现

https://tq.xunsl.com/v5/CommonReward/toGetReward.json -- 签到，和福利页任务奖励
https://tq.xunsl.com/v5/CommonReward/toDouble.json -- 领取签到翻倍奖励后可获取
https://tq.xunsl.com/v5/wechat/withdraw2.json -- 提现一次对应金额获取body

export jctqWithdraw=''
export jctqWithdrawFlag=''
export jctqBoxbody=''
export jctqQdBody=''
export jctqSignDoubleBody=''



## 晶彩天气 jctq_kkz.js

每天一到两次

抓POST包，点开看看赚，刷新闻，获取body

https://tq.xunsl.com/v5/nameless/adlickstart.json

链接转换：http://www.songluyi.com/ChangeHeaderToDict/

注：删除每个 : 后的空格后，再去转换。结尾处的User-Agent参数补完整，不然无效

export jctqLookStartbody=''




## 晶彩天气 jctq_read.js

每天一到两次

抓POST包，阅读文章或者看视频一段时间后可以获取到时长body

https://tq.xunsl.com/v5/user/stay.json

链接转换：http://www.songluyi.com/ChangeHeaderToDict/

注：删除每个 : 后的空格后，再去转换。结尾处的User-Agent参数补完整，不然无效

export jctqTimeBody=''

抓get，点开文章/视频获取文章body

https://tq.xunsl.com/v5/article/info.json

https://tq.xunsl.com/v5/article/detail.json

链接转换：http://www.songluyi.com/ChangeHeaderToDict/

export jctqWzBody=''



## 中青听歌 zq_music.js


建议运行时间  19 10-18 * * *

有的版本APP没有听歌

抓POST包，点击音频就我能获取ck

https://kandian.wkandian.com/V17/Ximalaya/setCompleteSec.json

export zqmusic=''


## 特别鸣谢:


* [@xl2101200](https://github.com/xl2101200/-/)「Tom」
* [@YaphetS0903](https://github.com/YaphetS0903/JStest/)「YaphetS」
* [@WindFgg](https://github.com/WindFgg/QuantumultX_Conf/)「WindFgg」
* [@wx13069](https://github.com/wx13069/JD/)「wx13069」
* [@LubooC](https://github.com/LubooC/Script/)「萝卜」
* [@leafxcy](https://github.com/leafxcy/JavaScript/)「leaf」
* [@shaolin-kongfu](https://github.com/shaolin-kongfu/js_scripts/)「少林大佬」
