# 自用脚本
- 1、电信营业厅  
原脚本作者：[**limoruirui**](https://github.com/limoruirui/misaka)  
增加多用户运行、多线程获取直播间  
    - 环境变量：  
        - TELECOM_USERPASS = '手机号1@密码1换行手机号2@密码2 或者 手机号1@密码1&手机号2@密码2'
        - TELECOM_FOOD='给宠物喂食次数 默认为0 不喂食 根据用户在网时长 每天可以喂食5-10次'  
    - 安装依赖
  ```
  打开面板-依赖管理-新建依赖 依赖类型选 python3
  安装requests、pycryptodome这2个依赖
  
  安装 pycryptodome 依赖时失败时 如果日志内有提示 gcc not found 的关键字 则进入docker容器中 依次执行
  $ apk update
  $ apk add build-base 
  此时在docker容器内执行 gcc --version 若正确显示版本信息 则可继续安装 pycryptodome
  

