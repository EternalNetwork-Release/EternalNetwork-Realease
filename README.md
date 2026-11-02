# Eternal Network 服务介绍页

这是一个单文件静态页面，用来介绍 Eternal Network 的线路、套餐、客户端和支持渠道。页面默认使用白色主题，可切换黑夜模式；不展示任何客户端下载直链，客户端入口统一指向官网。

- 在线页面：<https://eternalnetwork-release.github.io/>
- 注册、购买与客户端入口：<https://etcloud.top/#/register?code=QkfuWy3i>
- 备用入口：<https://edu.artyun.top/#/register?code=QkfuWy3i> · <https://9d4b878b9d8e2b31.cdn.jiashule.com/#/register?code=QkfuWy3i>
- Telegram 群组：<https://t.me/Etcloud>
- 页面文件：[`index.html`](./index.html)

## 页面内容

### 服务权益

- 16 元起套餐提供 IEPL 专线，线路侧重低延迟和稳定连接。
- 节点统一使用 AnyTLS，支持 TUN、全局和规则模式。
- 可用于 YouTube、Netflix、Disney+、Spotify 等服务，并提供 [RegionRestrictionCheck](https://github.com/lmc999/RegionRestrictionCheck) 解锁检测方法。
- 支持 Windows、macOS、Android、Linux 和 OpenWrt。iOS 用户可按文档使用 Nextin，输入标识码 etcloud 后登录账号。
- 官网文档、工单和 Telegram 群组都可获得支持，遇到配置或线路问题可以直接联系群主、管理员和群友。

### 月付套餐

| 套餐 | 流量 | 线路 | 价格 |
| --- | ---: | --- | ---: |
| 焦糖布丁 | 60 GB | 低延迟隧道 | ￥6/月 |
| 芒果奶昔 | 130 GB | 低延迟隧道 | ￥10/月 |
| 黄油曲奇 | 245 GB | 低延迟隧道 + IEPL | ￥16/月 |
| 奶油奶酪 | 335 GB | 低延迟隧道 + IEPL | ￥24/月 |
| 芝士蛋糕 | 720 GB | 低延迟隧道 + IPLC | ￥42/月 |

价格和线路状态以官网实时信息为准。

## 稳定性测试

页面提供三种测试方式，适合先测试再决定是否购买：

1. 安装 [NexTrace](https://github.com/nxtrace/NTrace-core)，在 WSL、Linux 或 macOS 终端运行：

   ```bash
   curl -fsSL https://raw.githubusercontent.com/nxtrace/NTrace-core/main/nt_install.sh | bash
   nextrace 节点域名或IP
   ```

2. Windows 安装 [tcping](https://github.com/elifulkerson/tcping/releases)：

   ```powershell
   winget install --id ELIFULKERSON.tcping --exact
   tcping -t 节点域名或IP 443
   ```

   持续运行几分钟，观察 TCP 建连是否超时、延迟是否反复升高。

3. 不想安装工具时，使用 [ITDOG TCPing 持续测试](https://www.itdog.cn/tcping/)，填入节点域名或 IP，端口填写 `443`。

持续 TCPing 比单次 ping 更接近真实连接体验。比较不同节点时，尽量使用相同网络、相同端口和相近的测试时长。

## 本地预览与部署

项目不需要构建工具。直接打开 `index.html` 即可预览，也可以在项目目录运行：

```bash
python -m http.server 8000
```

GitHub Pages 发布源设置为 `master` 分支的根目录 `/`。当前页面发布于 [`EternalNetwork-Release/EternalNetwork-Release.github.io`](https://github.com/EternalNetwork-Release/EternalNetwork-Release.github.io)。

## 信息来源

页面内容整理自 Eternal Network 使用文档。套餐价格、线路可用性、客户端版本和支持政策可能变化，请以官网和 Telegram 群组中的最新信息为准。
