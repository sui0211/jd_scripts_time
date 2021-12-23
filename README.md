# jd_scripts_time
京东活动脚本及时更新版，从几个仓库的watch中整理，会自动更新到车上

## 注意事项
1. 店铺和商品关注收藏有上限，需要定期手动取消店铺和商品关注

# 脚本监控列表
https://github.com/shufflewzc/faker2  
https://github.com/JDWXX/jd_job.git （脚本群大佬全量库）  
https://github.com/wsn888/jd.git （脚本群大佬临时活动库）  

## 脚本list
高价值（引入代理ip）
1. 京喜签到【完成】            -jx_sign.js
2. 东东农场水果【完成】        -jd_fruits.js
3. 种豆得豆【完成】            -jd_plantBean.js
4. 东东世界+兑换200豆【完成】  -jd_ddworld.js jd_dddh.js

中价值（京豆较少）
1. 首页领京豆【完成】          -jd_bean_home.js
2. 送豆得豆【完成】            -jd_sendBeans.js

低价值（无需变更和引入代理ip的）
1. 京东价保【完成】            -jd_price.js
2. 资产变动通知【完成】        -jd_bean_change.js
3. 获取互助码【完成】          -jd_get_share_code.js

个人修改版
1. 删除过期ck【完成】          -jd_CheckCK.js


### 新脚本增加代理ip设置
将env开头替换如下，即可以支持代理ip访问
```
const name = new Env('脚本名称');  // 拉取脚本时定时任务命名
const myEnv = require('./myEnv.js')
const $ = new myEnv.Env('京喜领88元红包');
```
