# CourseSelect [![Build Status](https://travis-ci.org/PENGZhaoqing/CourseSelect.svg?branch=master)](https://travis-ci.org/PENGZhaoqing/CourseSelect)

### [中文教程1](http://blog.csdn.net/ppp8300885/article/details/52594839) [中文教程2](http://blog.csdn.net/ppp8300885/article/details/52601560)


这个样本系统是基于国科大研究生课程 (高级软件工程) 开发的项目,目的是帮助入门者学习RoR (Ruby on Rails) 

适合新学者的入手的第一个项目 ([演示Demo戳这里](https://courseselect.herokuapp.com/ ))，入门者可以在这个样本系统上增加更多的功能:

*	多角色登陆（学生，老师，管理员）
*	学生动态选课，退课
*	老师动态增加，删除课程（使用Heroku的sendgrid服务）
*	老师对课程下的学生添加、修改成绩
*	处理选课冲突、控制选课人数
*	统计选课学分，学位课等
*	Excel格式的数据导入
*	绑定用户邮箱（实现注册激活，忘记密码等）
*	站内查找检索 （课程按分类查找，过滤等）
*	学生注册选课系统
*	学生查看个人课表
*	选课打印


### 截图

<img src="/lib/MainPage.png" width="700">  

<img src="/lib/SumSocres.png" width="700">

<img src="/lib/Schedule.png" width="700">   

<img src="/lib/Save.png" width="700">

## 说明

目前使用的库和数据库：

* 使用[Bootstrap](http://getbootstrap.com/)作为前端库
* 使用[Rails_admin Gem](https://github.com/sferik/rails_admin)作为后台管理
* 使用[Postgresql](http://postgresapp.com/)作为数据库

使用前需要安装Bundler，Gem，Ruby，Rails等依赖环境。

请根据本地系统下载安装[postgresql](https://devcenter.heroku.com/articles/heroku-postgresql#local-setup)数据库，并运行`psql -h localhost`检查安装情况。


## 安装

在终端（MacOS或Linux）中执行以下代码

```
$ git clone https://github.com/PENGZhaoqing/CourseSelect
$ cd CourseSelect
$ bundle install
$ rake db:migrate
$ rake db:seed
$ rails s 
```

在浏览器中输入`localhost:3000`访问主页

##使用

1.学生登陆：

账号：`student1@test.com`

密码：`password`

2.老师登陆：

账号：`teacher1@test.com`

密码：`password`


3.管理员登陆：

账号：`admin@test.com`

密码：`password`

账号中数字都可以替换成2,3...等等


## 外网访问

外网访问链接：
http://111.230.236.207:3000/ 


## 测试

本项目包含了部分的测试（integration/fixture/model test），测试文件位于/test目录下。运行测试：

```

# Running:
.........

Finished in 2.33169s, 9.4123 runs/s, 18.34535 assertions/s.

7 runs, 0 assertions, 0 failures, 7 errors, 0 skips
```


## How to Contribute

先fork此项目，在分支修改后，pull request到主分支

提问请到issues里创建，欢迎contributor！

如果觉得好，给项目点颗星吧～


