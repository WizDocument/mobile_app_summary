# APP托管总结

在发布到其他app托管平台期间，会涉及到给对于页面的命名


## 项目发布时页面命名规则

比如要将一个项目发布到fir.im时，给页面的短写的名字，命令，就和项目起包名，很类似。

对于：

> 大众RSE 下载安装地址：
> 
> Android：https://fir.im/ArdVolkswagenRSE
> 
> iOS： https://fir.im/iOSVolkswagenRSE”

建议fir.im中路径命名规则为：**项目名+平台+环境**

比如此处就是：

* 项目名：RSE，驼峰法命名（camel casing），Rse
* 平台：iOS或Android等
* 环境：
  * 开发版dev
  * 测试版test-》tst
  * 正式版
    * production-》prd
    * release-》rls

> #### info:: fir.im页面命名举例
> 之前的RSE的压测版的例子，供参考：
> 
> 【压测 压力测试版】
> * 卓越零售RSE 压测版 iOS 1.071 20170221 https://fir.im/RseiOSStress
> * 卓越零售RSE 压测版 Android v1.7.1 20170221 https://fir.im/RseAndroidStress
> 
> 其中：
> * Rse：表示RSE（卓越零售）项目的驼峰法命名
> * iOS或Anroid表示平台
> * Stress：表示 压力测试 Stress Test 的缩写，简写

另外，不同的公司，项目的缩写，前期不了解用哪个单词或如何缩写，可以理解

-> 随着深入接触和了解，慢慢就知道常见缩写了。

此处的 大众 德语的英文写法 的确是：Volkswagen

但是如果是 上汽大众 则是 csvw

-> 由之前接触的项目中，可以得知：

1. 上汽大众的主页是：http://www.csvw.com
2. 之前项目中知道对方员工的邮箱是：xxx@csvw.com

->

* 如果客户是德国大众（总部），则用：Volkswagen，或简写vw
* 如果是客户是上汽大众，则用：csvw

-> 此处，建议改为：

* RseiOSCsvw
* RseAndroidCsvw
  * -> 如果太长，可改为：RseAdrCsvw
