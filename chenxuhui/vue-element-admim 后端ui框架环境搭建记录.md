# vue-element-admim 后端ui框架环境搭建记录

------

### 1.github上获取项目源代码

[源代码链接](https://github.com/PanJiaChen/vue-element-admin)          [vue-element-admin官方文档](https://panjiachen.github.io/vue-element-admin-site/zh/)

环境要求：（1）[python2.7](https://www.python.org/downloads/release/python-2718/)    （2）[git](https://git-scm.com/)   （3）[nodejs16.8.0](https://nodejs.org/en/)



### 2.安装依赖和运行

```javascript
//(1)方法一:缺点较慢，有vpn可能会好一点，不过也比较慢，主要取决于你的网络
npm install
//(2)方法二：使用淘宝镜像,且建议不要用 cnpm 安装 会有各种诡异的bug 可以通过如下操作解决 npm 下载速度慢的问题
npm install --registry=https://registry.npm.taobao.org
//(3)运行
npm run dev
```

### 3.安装依赖和运行过程中遇到的一些error

npm install 安装的时候通过不了，python注意用2.x版本的，如果慢的话就用官方的淘宝镜像

出现以下错误的情况以及解决方法如果所示

*（1）node-sass依赖包下载异常*

![image-20210828170311791](C:\Users\TrustMe\AppData\Roaming\Typora\typora-user-images\image-20210828170311791.png)

*（2）gyp ERR！系列错误*

![image-20210828170213454](C:\Users\TrustMe\AppData\Roaming\Typora\typora-user-images\image-20210828170213454.png)

*（3）运行的时候提示缺少二进制文件*

![image-20210828165909266](C:\Users\TrustMe\AppData\Roaming\Typora\typora-user-images\image-20210828165909266.png)

思路：错误提示说缺少二进制，那么估计sass-loader安装的时候有点问题安装一个版本第一点的就行了

解决方法：**终端运行 ``npm install sass-loader@7.3.1 --save-dev``  **

链接：[二进制异常解决](https://blog.csdn.net/qq_45844443/article/details/114994335)



*（4）npm run dev运行成功后会自动加载到[http://localhost:9527](http://localhost:9527/)*

成功截图以及展示

![image-20210828173949469](C:\Users\TrustMe\AppData\Roaming\Typora\typora-user-images\image-20210828173949469.png)

![image-20210828174006681](C:\Users\TrustMe\AppData\Roaming\Typora\typora-user-images\image-20210828174006681.png)

