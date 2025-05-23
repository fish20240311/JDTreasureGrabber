# 京东夺宝岛助手

在 release 中可直接下载或自行打包构建😘

[![release](https://img.shields.io/github/v/release/GilHogan/JDTreasureGrabber?color=blue&label=Release)](https://github.com/GilHogan/JDTreasureGrabber/releases)

**注意📢**

- [关于软件商用、二次开发及AGPL-3.0协议的相关说明](https://github.com/GilHogan/JDTreasureGrabber/issues/27)
- 本软件不保证能抢购成功😂
- 使用前先安装 Chrome 浏览器
- 所有抢购方式均为：在商品抢购结束时刻之前出价一次
- 除了一口价抢购方式外，加价抢购方式均以他人的出价为基础进行加价
- 关闭抢购商品所在的浏览器即为结束抢购；抢购还未开始时，最小化浏览器或离开商品页面不会进行后续的出价
- telegram配置中，bot token和chat id参数的获取[参考](https://medium.com/@ManHay_Hong/how-to-create-a-telegram-bot-and-send-messages-with-python-4cf314d9fa3e)，或自行搜索解决


## 功能🎉

1. 支持多种方式进行抢购、支持列表抢购
2. 设置最后出价时间（出价后提示抢购已结束时，调大最后出价时间试试）
3. 商品信息查询
4. 抢购结果通知到telegram
5. 自动登录（记住登录信息）
6. 自动更新（MacOS暂不支持）

## 截图预览📺

<img alt='review' src="assets\images\preview.png" width="60%" style="">
<img alt='review' src="assets\images\preview2.png" width="60%" style="">
<img alt='review' src="assets\images\preview3.png" width="60%" style="">
<img alt='review' src="assets\images\preview_telegram.png" width="60%" style="">

## 开发相关🐵

- - 安装模块,卸载旧版本的nodejs 本工程使用nodejs18，安装完成后使用管理员权限，切换到工程目录
  - 设置镜像
  ```
  npm config set registry https://registry.npmmirror.com
  ```
  - 安装依赖，如果要打印安装过程使用：npm install -g yarn
     
  ```
      npm i
  ```
  - 重新安装依赖，删除现有的 node_modules 和 package-lock.json 文件
  ```
      rm -rf node_modules package-lock.json
  ```
  - 更改 npm 缓存目录，如果默认缓存目录存在问题，可以将其更改为其他路径
  ```
     npm config set cache "C:\\Users\\<你的用户名>\\npm-cache" --global
  ```
  - 试使用 Yarn，如果 npm 仍然无法正常工作，可以尝试使用 Yarn 安装依赖：安装 Yarn：   
    ```
         npm install -g yarn
    ```
    
- 启动服务，可在本地浏览器上进行 UI 调试
  ```
      npm run serve
  ```
- 构建&运行项目进行开发调试
  ```
      npm run build
      npm start
  ```
- 构建&打包项目
  ```
      npm run dist
  ```

- arm架构的系统构建方式参考，[参考1](https://github.com/jordansissel/fpm/issues/1801#issuecomment-919877499)，[参考2](https://www.beekeeperstudio.io/blog/electron-apps-for-arm-and-raspberry-pi)

## 免责声明❗

重要提示：请在使用本软件（京东夺宝岛助手）之前仔细阅读本免责声明。使用本软件即表示您已阅读、理解并同意本声明的全部条款。

### 软件用途

本软件（京东夺宝岛助手）旨在为个人学习和技术研究目的，提供一个辅助用户在京东夺宝岛平台进行商品抢购的工具。 开发本软件的目的是为了探索自动化技术和软件开发实践。

本软件**免费提供**，作者未授权任何个人或组织进行商业贩卖。任何收费行为均与作者无关，请用户自行甄别风险。

本软件与京东（或任何相关公司）没有任何关联，也未获得京东的授权或认可。

### 禁止的用途

严禁将本软件用于任何违反京东服务条款（包括但不限于禁止使用自动化工具抢购商品）的行为。

严禁将本软件用于任何违反中华人民共和国法律法规（包括但不限于《中华人民共和国反不正当竞争法》、《中华人民共和国消费者权益保护法》、《中华人民共和国网络安全法》等）的行为。

严禁将本软件用于任何可能对京东服务器造成过大压力或干扰其正常运营的行为。

严禁将本软件用于任何侵犯他人知识产权或其他合法权益的行为。

严禁任何未经授权的商业贩卖行为，包括但不限于假冒作者名义的销售、转售、分发或提供本免费软件的付费服务。

严禁未经授权的修改、反编译、反汇编或以其他方式试图获取本软件的源代码用于商业用途（除非您根据 AGPL-3.0 许可证的条款进行操作）。

严禁移除或修改本软件中的任何版权声明、商标或其他所有权声明。

### 风险自负

使用本软件的全部风险由您自行承担。

您理解并同意，使用本软件可能违反京东平台的相关规则，并可能导致您的京东账户受到限制、封禁或其他处罚。

您理解并同意，使用本软件可能导致您面临法律诉讼或其他法律风险。

### 免责条款

本软件按“原样”提供，不提供任何形式的明示或暗示的保证，包括但不限于适销性、特定用途适用性和不侵权。

在任何情况下，对于因使用或无法使用本软件而导致的任何直接、间接、偶然、特殊、惩罚性或后果性损害（包括但不限于利润损失、数据丢失、业务中断等），本软件的作者或版权持有者均不承担任何责任，即使已告知可能发生此类损害。

对于任何非根据 AGPL-3.0 许可证条款合法使用本软件的第三方（包括但不限于软件的购买者、转售者、未经授权的使用者等）因使用、修改、分发本软件或其衍生作品而导致的任何违法违规行为、侵权行为、违反服务条款的行为，或由此产生的任何民事责任、刑事责任、行政责任，本软件的作者或版权持有者均不承担任何责任。本条款是对 AGPL-3.0 许可证中免责声明的补充，而非取代。

### 开源协议

本软件基于 AGPL-3.0 许可协议开源。 任何对本软件的使用都必须遵循该协议的规定。

AGPL-3.0 许可协议包含免责声明，明确声明不对软件的使用后果负责。

### 其他

作者保留对本免责声明的解释权。

本免责声明可能随时更新，恕不另行通知。请定期查看最新版本。
