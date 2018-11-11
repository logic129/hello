# PHP开发实践教程

https://git.dev.tencent.com/hoybin/learnphp.git

PHP是世界上最好的语言

## 一、入门基础

### 1. 动态网页原理

![PHP动态网页原理](http://www.surfphpseo.com/d/file/webjsn/2013-09-12/2371c5d3b86aaf75512d4a60886fa9dd.jpg)

- 浏览器 B
- 服务器 S
- URL http://vip.book.sina.com.cn:81/weibobook/book/5352242.html?pos=202068&id=123
    + 协议 http, https
    + 主机 域名: localhost ip地址: 127.0.0.1
    + 端口 80, 443
    + 路径
    + 文件 
    + 参数

### 2. LA(N)MP技术架构

- Linux           操作系统
- Apache/Nginx    WEB服务器
- Mysql           数据库服务器
- PHP             脚本解析器

### 3. 本地开发环境搭建

- PHPStudy 
    + [官网下载](http://www.phpstudy.net/download.html)

### 4. 开发工具

- Sublime_Text
    + [官网下载](http://www.sublimetext.com/)
    + [流风清音优化版](http://haojian138.blog.163.com/blog/static/212643110201393010438357/)

- PHPStorm
    + [官网下载](https://www.jetbrains.com/phpstorm/download/#section=windows)

### 5. 自修技能

- Markdown
    + [语法教程](https://www.baidu.com/s?ie=utf-8&f=8&rsv_bp=0&rsv_idx=1&tn=baidu&wd=markdown%20%E8%AF%AD%E6%B3%95%E6%95%99%E7%A8%8B&rsv_pq=92bcdacc000076c5&rsv_t=3c24fwgtKKclOa9QBRPvFPeMJ6v6bO%2BOmG1IKQKYpjkp3J7lqJhdTj%2Broog&rqlang=cn&rsv_enter=1&rsv_sug3=26&rsv_sug1=18&rsv_sug7=100)
    + [推荐工具](https://www.zybuluo.com/mdeditor)

- Git
    + 基本命令
        git clone  复制一个远程库到本地
        git status 查看状态
        git add 添加更改
        git commit 提交更改
        git push  推送代码到远程
        git pull  拉取远程代码
    + 软件下载
        * [Git: https://git-scm.com/](https://git-scm.com/)
        * [TortoiseGit: https://tortoisegit.org/](https://tortoisegit.org/)
    + 在线教程
        - [史上最浅显易懂的Git教程](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/)
    + 命令速查    
        ![Git命令速查](https://static.oschina.net/uploads/img/201412/07180843_cbKA.jpg)
    + 代码托管平台
        * [github（国外）: https://github.com/](https://github.com/)
        * [coding（国内）: https://coding.net/](https://coding.net/)
    + 配置账号（引号中的内容替换为自己的信息）
        1. 配置用户名 `git config user.name "Your name"`
        2. 配置邮箱 `git config user.email "Your youremail@example.com"`
        3. 生成SSH秘钥，命令 `ssh-keygen -t rsa -C "youremail@example.com"`
        4. 上传公钥匙，默认存储路径 `C:\Users\Administrator\.ssh\id_rsa.pub`

### 6. PHP简介

> PHP（全称：PHP：Hypertext Preprocessor，即“PHP：超文本预处理器”）是一种开源的通用计算机脚本语言，尤其适用于网络开发并可嵌入HTML中使用。PHP的语法借鉴吸收C语言、Java和Perl等流行计算机语言的特点，易于一般程序员学习。PHP的主要目标是允许网络开发人员快速编写动态页面，但PHP也被用于其他很多领域。  ---【[维基百科](https://zh.wikipedia.org/zh/PHP)】

中文手册：[http://php.net/manual/zh/](http://php.net/manual/zh/)

#### 1) PHP语言特点

__解释型语言__：解释型语言的运行方式是边解释边执行，PHP解释器会在第一时间发现代码中的错误，对程序猿来说，这种方式更容易调试错误及修复漏洞，开发效率比较高。

__开放源代码__：PHP本身的代码是开放的，任何人都可以免费获取和使用，因此在WEB领域，PHP已经成为低成本解决方案的首选语言，这也成为PHP语言如此流行的一个重要原因。

__跨平台__：PHP程序由运行在服务器端的PHP解释器解释并执行，而PHP解释器可以运行在UNIX、LINUX、WINDOWS、Mac OS等各种操作平台上，因此可以说用PHP编写的脚本不受特定平台限制。

__易用性__：由于PHP的设计初衷是作为一个处理个人主页的脚本工具，因此语言本身的架构没有被设计的很复杂，所以相对其他编程语言，PHP学习起来也相对容易很多，很容易上手。

#### 2) PHP版本历程

__1.0__ [1995-06-08] 正式名称为"Personal Home Page Tools (PHP Tools)"，第一次使用了"PHP"的名字。

__2.0__ [1996-04-16] 针对PHP 1.0的改进版，速度更快、体积更小，更容易产生动态网页。

__3.0__ [1998-06-06] 开发方式改成多人共同参与。Zeev Suraski和Andi Gutmans为了这个版本重写了剖析引擎。

__4.0__ [2000-05-22] 改成以Zend引擎作为语法分析器，具有两阶段剖析/标签剖析系统等先进功能。

__5.0__ [2004-07-13] 推出有着新的对象模型的Zend Engine II。

__5.3__ [2009-06-30] 支持命名空间;使用XMLReader和XMLWriter增强XML支持;支持SOAP ,延迟静态绑定，跳转标签（有限的goto）, 闭包，Native PHP archives。

__5.4__ [2012-03-01] 支持Trait、简短数组表达式。移除了register_globals, safe_mode, allow_call_time_pass_reference, session_register(), session_unregister(), magic_quotes以及session_is_registered()。加入了内建的Web服务器。增强了性能，减小内存使用量。

__5.5__ [2013-06-20] 支持generators，用于异常处理的finally ，将OpCache（基于 Zend Optimizer+）加入官方发布中。

__5.6__ [2014-08-28] 支持常量标量表达式、可变参数函数、指数运算符，增加phpdbg SAPI、统一的默认字符集。

__7.0__ [2015-12-03] Zend Engine 3 (性能提升并在Windows上支持 64-bit 整数)，统一的变量语法， 基于抽象语法树编译过程。

#### 3) 开源项目

__框架__

- [ThinkPHP - http://www.thinkphp.cn](http://www.thinkphp.cn)
- [Yii - http://www.yiichina.com](http://www.yiichina.com)
- [Laravel - https://laravel.com](https://laravel.com)

__应用__

- 【博客】[wordpress - https://cn.wordpress.org](https://cn.wordpress.org)
- 【论坛】[discuz - http://www.discuz.net/forum.php](http://www.discuz.net/forum.php)
- 【商城】[ecshop - http://www.ecshop.com](http://www.ecshop.com)

__其他项目__

- [生成二维码 - https://github.com/t0k4rt/phpqrcode](https://github.com/t0k4rt/phpqrcode)
- [解析RSS订阅 - https://github.com/simplepie/simplepie](https://github.com/simplepie/simplepie)
- [生成PDF - https://github.com/tecnickcom/tcpdf](https://github.com/tecnickcom/tcpdf)
- [解析DOM - https://github.com/TobiaszCudnik/phpquery](https://github.com/TobiaszCudnik/phpquery)
- [电子邮件 - https://github.com/PHPMailer/PHPMailer](https://github.com/PHPMailer/PHPMailer)
- [过滤HTML - https://github.com/ezyang/htmlpurifier](https://github.com/ezyang/htmlpurifier)

## 二、PHP语言基础

### 1. 脚本

> 动态程序一般有两种实现方式，一是二进制方式，一是脚本方式。二进制方式是先将我们编写的程序进行编译，变成机器可识别的指令代码（如.exe文件），然后再执行。这种编译好的程序我们只能执行、使用，却看不到他的程序内容。脚本简单地说就是一条条的文字命令，这些文字命令是我们可以看到的（如可以用记事本打开查看、编辑），脚本程序在执行时，是由系统的一个解释器，将其一条条的翻译成机器可识别的指令，并按程序顺序执行。因为脚本在执行时多了一道翻译的过程，所以它比二进制程序执行效率要稍低一些。

> 这样就不难理解，在计算机中，脚本执行就好像戏剧里的演员在“演绎”已经写好的剧本，把它渲染出来。程序脚本就是程序读出这些文字并把它执行出结果来。   ---【[知乎](https://www.zhihu.com/question/19901542/answer/20163098)】

### 2. 第一个问候

```
<?php
    echo 'Hello world!';
?>
```

- 代码标记：`<?php ... ?>`
- 文件扩展名：`.php`
- 文件保存位置：WEB服务器目录
- 运行程序：必须通过浏览器URL地址访问

### 3. 基本语法

- 每条语句以分号结尾
- 一行可写多条语句
- 多条语句可用`{}`包围组成语句块

### 4. 输出语句

- echo
- print

### 5. 注释

- 单行注释 `// ...`    ctrl + /
- 多行注释 `/* ... */` ctrl + shift + /

### 6. 基本数据类型

- 整数
- 浮点数
- 字符串
- 布尔

### 7. 变量

- 变量名
    + 以$开头，一个或多个字母、数字、下划线字符组成
    + $后不能紧跟数字
    + 变量名中的字母区分大小写
- 创建变量
- 显示变量内容
- 销毁变量

### 8. 运算符

- 字符串运算符：`.`
- 算数运算符：`+ - * / %`
- 赋值运算符：`= += -= *= /= %= .=`
- 递增递减运算符：`++ --`
- 比较运算符：`== === != <> !== < > <= >=`
- 逻辑运算符：`&& || !`
- 条件运算符：`? :`
- 运算符的优先级：【[PHP手册 / 运算符的优先级](http://php.net/manual/zh/language.operators.precedence.php)】
    1. `++ --`
    2. `!`
    3. `* / %`
    3. `+ - .`
    4. `< <= > >=`
    5. `== != === !== <> <=>`
    6. `&&`
    7. `||`
    8. `? :`
    9. `= += -= *= /= %= .=`

### 9. 流程控制

- if
- if else
- swicth
- while
- do while
- for

### 10. 数组

- 数组的键和值
- 索引数组, 键是数字 从零开始 自动增长
- 关联数组, 键是字符串
- 创建数组, `array()`, `[]`
- 查看数组内容, `print_r()`
- 元素操作
    + 添加数组元素
    + 访问数组元素
    + 修改数组元素
    + 删除数组元素
    + 遍历数组元素, `foreach(){}`
- 二维数组
    + 二维数组的遍历
    + 嵌入HTML
        <?=...;?>
        <?php echo ...;?>

### 11. 函数

- 函数的定义
- 函数的调用
- 函数的参数
- 参数的默认值
- 函数的返回值
- 变量的作用域
