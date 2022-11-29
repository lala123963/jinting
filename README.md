# 瞎吉尔脚本
- 1、电信 china_telecom.py、telecom_live_lotter.py  
原脚本作者：[**limoruirui**](https://github.com/limoruirui/misaka)  
    - 环境变量：  
        - TELECOM_USERPASS = '手机号1@密码1换行手机号2@密码2 或者 手机号1@密码1&手机号2@密码2'
        - TELECOM_FOOD  : 给宠物喂食次数 默认为0 不喂食 根据用户在网时长 每天可以喂食5-10次
        - TELECOM_LIVEINFO='直播间获取链接'  选填，若出现内置的获取链接404，则需填入该变量，自己抓包或询问大佬  
    - 安装依赖
  ```
  _安装依赖时失败时 如果日志内有提示 gcc not found 的关键字 则进入docker容器中 依次执行
  $ apk update
  $ apk add build-base 
  此时在docker容器内执行 gcc --version 若正确显示版本信息 则可继续安装_
  
  第一种方法: 在github复制requirements.txt内的所有东西 
  打开面板-依赖管理-新建依赖 依赖类型选 python3 自动拆分选 是 把复制的东西粘贴在名称内 确定即可
  
  第二种方法: 进入容器中 依次执行
  $ cd data/scripts/limoruirui_misaka
  $ wget https://raw.githubusercontent.com/limoruirui/misaka/master/requirements.txt
  $ pip3 install -r requirements.txt
