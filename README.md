### Net

#### 项目描述  
>本项目为2015级计算机网络大实验作品  
>当前版本：V1.1  
>更新日志:
>* 收发线程分离，修复粘包问题
>* 修复客户端未选择文件时禁用按钮的问题
>* 修复用户登录验证码大小写问题
>* 修复客户端文件显示问题
>* 增加文件传输MD5校验功能
>* 增加用户名密码传输加密功能
>* 用户数据库从Mysql迁移至sqlite

联系邮箱：sangyunxin@gmail.com  
本项目Github地址：https://github.com/sangyunxin/Net  
Copyright 2017 - 2018 Sangyunxin. All Rights Reserved.   

---  

#### 实验目的
了解和掌握基于socket的网络编程技术，开发基于socket的网络应用。

#### 实验内容
了解应用编程接口API，掌握基于socket的网络编程的原理，开发利用socket的TCP文件传输应用程序。该应用需要具备的功能以及实现的要点描述如下：  
* 该程序应该包括服务器应用程序以及客户应用程序。
* 用户需要身份验证。即对于客户端来说，无论是上传文件，还是下载文件，首先需要做的事情是登陆服务器，得到服务器的验证。 若验证成功，即可与服务器之间开始传输文件。若验证失败，服务器则返回错误信息。错误信息包括，用户名错误，密码错误等。
* 理解文件传输的原理。所谓文件传输，对于发送端来说，实质是将数据读入发送缓存再将其发送。对于接收端来说，实质是从接收缓存里读取数据并将其写入到指定的位置。
* 请注意理解文件传输的含义。文件，指的是一切可以传输的信息，包括文本文件、图片文件、视频文件等。传输，指的是服务器和客户端都可以成为文件的发送者。从客户端的角度来说，客户端向服务器传送文件称为上传，服务器向客户端传送文件称为下载。
