# jd_scripts_time
京东临时库，从几个仓库的watch中整理，会自动更新到车上

# 脚本监控（添加watch或者删除本地后手动拉取）
https://github.com/shufflewzc/faker2
https://github.com/wsn888/jd.git（这个库只更新新活动）

### 新脚本增加代理ip设置
将env开头替换如下，即可以支持代理ip访问
```
const name = new Env('脚本名称');  // 拉取脚本时定时任务命名
const myEnv = require('./myEnv.js')
const $ = new myEnv.Env('京喜领88元红包');
```
