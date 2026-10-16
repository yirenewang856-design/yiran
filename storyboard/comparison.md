# 网站状态对比与设计匹配规则

[返回总目录](README.md)

这里的左右图均为真实网站截图。**目前没有可用的 Figma 画板，不能把此页说成已完成网站与设计稿对照。**

[Figma 访问说明与候选保留规则](figma/README.md)

## Cookie 提示前后

拒绝后提示消失；接受分支另存，不与拒绝串成一次会话。

| 状态 A | 状态 B |
|---|---|
| W001：首次打开首页 | W003：拒绝 Cookie 后的首页 |
| [![状态A](screenshots/01-home.png)](screenshots/01-home.png) | [![状态B](screenshots/03-home-clean.png)](screenshots/03-home-clean.png) |

## 地图说明展开与关闭

关闭后露出地图背景。

| 状态 A | 状态 B |
|---|---|
| W008：进入 2D：首次说明面板 | W009：关闭地图介绍 |
| [![状态A](screenshots/06-map-intro.png)](screenshots/06-map-intro.png) | [![状态B](screenshots/07-map-intro-closed.png)](screenshots/07-map-intro-closed.png) |

## 数字导航与完整导航

All 展示额外栏目；这是菜单分支。

| 状态 A | 状态 B |
|---|---|
| W011：展开主菜单：数字平台 | W012：切换完整导航 |
| [![状态A](screenshots/09-main-menu.png)](screenshots/09-main-menu.png) | [![状态B](screenshots/22-menu-all.png)](screenshots/22-menu-all.png) |

## 搜索空结果与有结果

不同关键词的结果对比，不是同一次搜索的前后。

| 状态 A | 状态 B |
|---|---|
| W016：搜索无结果分支 | W018：查看搜索结果 |
| [![状态A](screenshots/18-search-typed.png)](screenshots/18-search-typed.png) | [![状态B](screenshots/search-submit.png)](screenshots/search-submit.png) |

## 数字路径“查看全部”前后

不同捕获时刻；复测确认 URL 和正文均无变化。

| 状态 A | 状态 B |
|---|---|
| W025：凝视与记忆 | W026：凝视与记忆：查看全部无变化 |
| [![状态A](screenshots/page-base-topics-1-digital-paths-1.png)](screenshots/page-base-topics-1-digital-paths-1.png) | [![状态B](screenshots/see-all-1.png)](screenshots/see-all-1.png) |

## 购物车打开与点击结账后

不同币种测试分支；重点看空购物车点击后的面板关闭，不把币种差异误判为结账结果。

| 状态 A | 状态 B |
|---|---|
| W111：打开购物车 | W113：空购物车点击结账 |
| [![状态A](screenshots/store-cart.png)](screenshots/store-cart.png) | [![状态B](screenshots/store-checkout-empty.png)](screenshots/store-checkout-empty.png) |

## 条款未勾选与勾选

勾选后 Google 按钮可用，随后主站 OAuth 失败。

| 状态 A | 状态 B |
|---|---|
| W134：打开账户登录面板 | W135：启用 Google 登录入口 |
| [![状态A](screenshots/21-profile-entry.png)](screenshots/21-profile-entry.png) | [![状态B](screenshots/23-login-terms.png)](screenshots/23-login-terms.png) |

## 视频全屏与退出

通过 fullscreenElement 确认状态 true → false。

| 状态 A | 状态 B |
|---|---|
| W073：进入视频全屏 | W074：退出视频全屏 |
| [![状态A](screenshots/media-fullscreen-confirmed.png)](screenshots/media-fullscreen-confirmed.png) | [![状态B](screenshots/media-exit-fullscreen.png)](screenshots/media-exit-fullscreen.png) |

## 不确定画面保留规则

同一操作有多个设计候选时，分别展示候选 A、B、C，保留画板名、节点、版本、匹配依据与未确认点；不因外观相似直接定为同一页面。当前未取得设计，候选数量也无法确认。
