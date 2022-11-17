# 学生实习管理系统的设计与实现

# Student Internship Management System

# 数据库设计

## 前置需求数据表

### sex

性别表，存储性别信息

| 字段 |  类型   | 长度 |    备注    |
| :--: | :-----: | :--: | :--------: |
|  id  |   int   |      | 唯一标识符 |
| sex  | varchar |  4   |    性别    |

|  1   |  男  |
| :--: | :--: |
|  2   |  女  |
|  3   | 保密 |



## 实体表

### student

| 字段 | 类型   | 长度 | 备注 |
| :--: | ------ | ---- | ---- |
|  id  | Intger |      |      |
|      |        |      |      |
|      |        |      |      |

# 功能模块

## 新增学生信息

前台：sa添加学生（姓名、学院、专业、班级、身份证号码、入学年份）信息

后台：学生（性别、年龄）由（身份证号码）生成，（学号）由（学院代码、专业代码、入学年份）综合生成

# 技术实现

Vue3+Node.js+uview-plus

# 系统实现

## 环境部署

### 1.在Hbuiderx创建StudentInternship项目

#### （1）创建StudentInternship项目



#### （2）安装uview-plus

官网：[uview-plus](https://uiadmin.net/uview-plus/)

安装地址：https://ext.dcloud.net.cn/plugin?name=uview-plus

```js
// 如果您的根目录没有package.json文件的话，请先执行如下命令：
// npm init -y

npm install uview-plus

// 更新
// npm update uview-plus

//版本查询
// 通过`console.log`打印的形式
console.log(uni.$u.config.v);

// 可以查阅uview-plus的配置文件得知当前版本号，具体位置为：
/uview-plus/libs/config/config.js
```

关于SCSS

uview-plus依赖SCSS，您必须要安装此插件，否则无法正常运行。

如果您的项目是由`HBuilder X`创建的，相信已经安装scss插件，如果没有，请在HX菜单的 工具->插件安装中找到"scss/sass编译"插件进行安装， 如不生效，重启HX即可

如果您的项目是由vue-cli创建的，请通过以下命令安装对sass(scss)的支持，如果已安装，请略过。

```js
// 安装sass
npm i sass -D

// 安装sass-loader，注意需要版本10，否则可能会导致vue与sass的兼容问题而报错
npm i sass-loader@10 -D
```

