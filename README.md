

# 多个项目集合
### https://github.com/shufflewzc/faker2
### https://github.com/JDHelloWorld/jd_scripts
### https://github.com/he1pu/JDHelp



# 青龙拉取常用京东脚本库

## 说明

- 更新一个整库脚本

```
ql repo <repourl> <path> <blacklist> <dependence> <branch>

 # <repourl>  仓库url
 # <path>  下载文件
 # <blacklist> 排除文件
 # <dependence> 依赖文件及文件夹 
 # <branch> 分支

```

- 更新单个脚本文件

```
ql raw <fileurl>
```



## 示例

1. `JDHelloWorld`

   ```
   ql repo https://github.com/JDHelloWorld/jd_scripts.git "jd_|jx_|getJDCookie" "activity|backUp|Coupon|enen|update|test" "^jd[^_]|USER|^TS|utils|notify|env|package|ken.js"
   ```

   

2. `he1pu`（自动提交助力码-京喜工厂、种豆得豆、东东工厂、东东农场、健康社区、京喜财富岛、东东萌宠、闪购盲盒，随机从数据库中选取助力码互助）

   ```
   ql repo https://github.com/he1pu/JDHelp.git "jd_|jx_|getJDCookie" "Coupon|update" "^jd[^_]|USER|^sign|^ZooFaker|utils"
   ```

   

3. `shufflewzc`

   ```
   ql repo https://github.com/shufflewzc/faker2.git "jd_|jx_|gua_|jddj_|getJDCookie" "activity|backUp" "^jd[^_]|USER|utils|^JS|^TS|^JDJRValidator_Pure|^ZooFaker|^sign"
   ```

   



# 集合表示

```
# https://ghproxy.com/ 表示git下载加速 

ql repo https://ghproxy.com/https://github.com/simple11618/jd_script.git "jd_|jx_|gua_|jddj_|getJDCookie" "activity|backUp|Coupon|enen|update|test" "^jd[^_]|USER|^TS|utils|notify|env|package|ken.js|^sign|^ZooFaker|^JS|^JDJRValidator_Pure"
```

