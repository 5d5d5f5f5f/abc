针对不同类型壳子订阅使用的格式，提供两种格式部署脚本
## TXT订阅格式请部署`worker.js`
## M3U订阅格式请部署`workerm3u.js`
![图片1](https://raw.githubusercontent.com/5d5d5f5f5f/10102/main/10.jpg)
![图片2](https://raw.githubusercontent.com/5d5d5f5f5f/10102/main/11.jpg)
![图片3](https://raw.githubusercontent.com/5d5d5f5f5f/10102/main/12.jpg)
# Cloudflare Worker 部署
## Cloudflare注册地址 https://dash.cloudflare.com

复制代码文件：`worker.js` 在Cloudflare 创建`Worker` 链接数据库自动更新订阅资源

---


## 部署方法

### 1️⃣ 登录后台
登录 Cloudflare 后台

---

### 2️⃣ 进入 Workers
在左侧菜单找到：

👉 **Workers & Pages**

点击进入

---

### 3️⃣ 创建 Worker
依次点击：

👉 **Create Application（创建应用）**  
👉 **从 Hello World!开始**

然后点击：

👉 **Create Worker（创建 Worker）**

---

## 编辑代码

进入后会看到默认代码：

```javascript
export default {
  async fetch(request) {
    return new Response("Hello World!");
  }
}
把默认代码删除，替换为本项目 Worker 代码
点击右上角：

👉 Deploy（部署）

等待几秒即可完成部署
部署成功后，会生成一个访问地址，例如：

https://xxxx.workers.dev

直接在浏览器打开即可查看效果
绑定自定义域名（可选）

如果你有域名，可以绑定：

进入 Worker 设置
点击：
👉 Triggers（触发器）
添加：
👉 Custom Domain（自定义域名）

---

## 使用

部署完成后，会生成一个内部地址：
或者绑定域名可公开访问地址
## 免费域名注册地址   https://my.dnshe.com
使用邀请码，您与好友各增加 1 个注册额度。
## 邀请码：FQE4D39C49




# 版权说明
## LICENSE

本项目仅供个人学习、研究及技术交流使用，严禁用于任何形式的商业用途。

任何人不得利用本项目从事包括但不限于盈利、传播、非法获取资源等行为，否则后果自负，与本项目作者无关。

使用者应在下载后 24 小时内自行删除全部内容，不得进行二次传播、分发或长期存储。

本项目不提供任何内容存储或分发服务，所有资源均来源于互联网公开信息，仅用于学习测试网络连通性与技术实现方式。

本项目不对资源的合法性、准确性、完整性作任何保证，也不承担任何直接或间接责任。

如本项目内容侵犯了您的合法权益，请及时联系删除，作者将在第一时间进行处理。

使用本项目即代表您已阅读并同意以上声明内容。
