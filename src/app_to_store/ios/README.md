# iOS上架

* app上架的地方：
  * 公开版本：苹果官网的唯一的App Store
  * 企业版：无需上架，找个app应用发布的地方供用户下载即可，比如
    * fir.im
    * OTA版：自己提供对应的服务器用于存放ipa和对应的plist
      * 注意必须要支持https才可以
  * AdHoc版本：临时发布供测试
    * 在用Xcode打包之前就要设置好对应的profile，添加iPhone等设备等GUID，发布后，加了GUID的iPhone等设备才能安装和使用
* 需要提供App的测试账号和密码
  * 苹果官方审核人员会登录你的app
  * 测试你的基本功能
    * 看看app内容是否有违规内容
    * 且要确保你的app的稳定性
      * 不会随便就崩溃了
        * 否则影响用户体验，就会被拒
