## :memo: a simple project for Spring Boot ~

### 项目概述  (:speech_balloon: pause update)
:+1:*一个简单的,基于Spring Boot的好友备忘录小项目,通过本项目可以学习`Spring Boot`与`MyBatis`的整合及CURD操作的基本思路,同时也可以帮助你学习`Thylemeaf`模板引擎使用哟(`请根据所需选择分支`)~ 这可能是流程最清晰、代码最干净、注释最详细、最具扩展性的 SpringBoot 入门项目啦~ 可以说非常适合初学Sping Boot的同学哟(っ•̀ω•́)っ✎⁾⁾~*


### 分支介绍
- :arrows_clockwise: *`master` : 基本的Spring Boot整合MyBatis (该代码的优化请参考`refactor-190823`分支)*
- :arrows_clockwise: *`v2.0-redis` : 在master分支上简单集成Redis*
- :arrows_clockwise: *`refactor-190823` : 重构并优化master分支代码,提高程序的可扩展性*

:heart:*为了让更多同学快速地体验该项目,已通过`mvn package`将`master`分支打包,并将其作为`v1.0`上传到了`release`中~*


### 项目截图
- *项目主页*

![](https://raw.githubusercontent.com/YUbuntu0109/SpringBoot-CURD-Memo/master/demonstration_picture/SpringBoot-CURD-Memo_MainView.PNG)

- *好友信息管理页*

![](https://raw.githubusercontent.com/YUbuntu0109/SpringBoot-CURD-Memo/master/demonstration_picture/SpringBoot-CURD-Memo_FriendListView.PNG)

![](https://raw.githubusercontent.com/YUbuntu0109/SpringBoot-CURD-Memo/master/demonstration_picture/SpringBoot-CURD-Memo_FriendListView2.PNG)


### 项目结构(`master branch`)
```
│  .gitattributes
│  LICENSE
│  README.md
│
├─database file
│      memo.sql
│
├─demonstration_picture
│      SpringBoot-CURD-Memo_FriendListView.PNG
│      SpringBoot-CURD-Memo_FriendListView2.PNG
│      SpringBoot-CURD-Memo_MainView.PNG
│
└─memo
    │  .gitignore
    │  pom.xml
    │
    └─src
        └─main
            ├─java
            │  └─pers
            │      └─haungyuhui
            │          └─memo
            │              │  MemoApplication.java
            │              │
            │              ├─bean
            │              │      Friend.java
            │              │
            │              ├─controller
            │              │      StudentController.java
            │              │
            │              ├─dao
            │              │      FriendMapper.java
            │              │      FriendMapper.xml
            │              │
            │              ├─service
            │              │  │  FriendService.java
            │              │  │
            │              │  └─impl
            │              │          FriendServiceImpl.java
            │              │
            │              └─util
            │                      UploadFile.java
            │
            └─resources
                │  application.properties
                │
                ├─static
                │  ├─easyui
                │  │  │  jquery.easyui.min.js
                │  │  │  jquery.min.js
                │  │  │
                │  │  ├─css
                │  │  │      default.css
                │  │  │      demo.css
                │  │  │
                │  │  ├─js
                │  │  │      outlook2.js
                │  │  │      validateExtends.js
                │  │  │
                │  │  └─themes
                │  │      │(略..)
                │  │        
                │  │      
                │  │      
                │  └─image
                │          default_portrait.png
                │
                └─templates
                        friendList.html
                        intro.html
                        main.html
```

#### 项目文件说明-`数据库文件`
```
memo.sql
```

#### 项目文件说明-`EasyUI 前端框架`
```
easyui/
```

#### 项目文件说明-`用户默认头像`
```
default_portrait.png
```



*:books:更多有趣项目及详细学习笔记请前往我的个人博客哟（づ￣3￣）づ╭❤～ : https://yubuntu0109.github.io/*

*👩‍💻学习笔记已全部开源 : https://github.com/YUbuntu0109/YUbuntu0109.github.io*
 
*:coffee: Look forward to your contribution, if you need any help, please contact me~ QQ : 3083968068*
