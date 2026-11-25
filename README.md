<div align="center">

<img src="docs/assets/hero-banner.png" width="100%" alt="贴贴桌宠 PitaPet" />

<br />

**简体中文** &nbsp;|&nbsp; [English](./README.en.md)

<p>
  <img src="https://img.shields.io/badge/Windows-64--bit-5B8FF9?style=flat-square" alt="Windows 64-bit" />
  <img src="https://img.shields.io/badge/Local-Portable-5AD8A6?style=flat-square" alt="Local Portable" />
  <img src="https://img.shields.io/badge/Current-v0.5.1%20Viola%20%C3%97%20Arale-E05A8D?style=flat-square" alt="v0.5.1" />
  <img src="https://img.shields.io/badge/Fanwork-Free%20%2F%20Non--Commercial-8C7AE6?style=flat-square" alt="Free Fanwork" />
</p>

一个跑在 Windows 上的本地桌面宠物程序，重点做了**双人互动**和**更跟手的拖拽**。<br />
绿色免安装、免登录，解压就能跑，所有同人角色包免费分享。

</div>

---

## 实机预览

<table>
  <tr>
    <td align="center" width="33%">
      <img src="docs/assets/preview-duo-pinch.webp" width="100%" alt="双人捏脸" />
      <br />
      <strong>双人捏脸</strong>
      <br />
      <sub>把两只拖近后触发</sub>
    </td>
    <td align="center" width="33%">
      <img src="docs/assets/preview-duo-pushface.webp" width="100%" alt="双人推脸" />
      <br />
      <strong>双人推脸</strong>
      <br />
      <sub>自带转向和回落衔接</sub>
    </td>
    <td align="center" width="33%">
      <img src="docs/assets/preview-egg-gag.webp" width="100%" alt="煎蛋彩蛋" />
      <br />
      <strong>煎蛋彩蛋</strong>
      <br />
      <sub>连续快点 6 次触发</sub>
    </td>
  </tr>
</table>

---

## 主要功能

- **双人贴贴互动**：把两只桌宠拖近会触发专属双人动作（当前已含捏脸、推脸、理头发、揪兜帽、说悄悄话共 5 套）。
- **60Hz 全向跟手拖拽**：上、下、左、右拖拽和急转都有对应的实时摆动和松手回落，不是静态立绘硬拖。
- **日常待机动作**：包含站姿、坐姿、翘腿、趴卧打盹、桌面散步、屏幕边缘探头，以及角色各自的小动作，不会一直死盯着屏幕。
- **内置轻量模式一键切换**：在控制台「设置 → 运行模式」可随时在**标准模式**与**轻量模式**之间切换——保持原画质不糊的同时，拖拽改静态贴图省显存内存、遮挡/全屏自动暂停渲染、辅助窗按需启停、自动双人互动降频。
- **本地预渲染 & 分包导入**：免登录、不用安装、不连云端 AI。后续出新角色可以直接通过 `.petpack`（单人包）和 `.duopack`（双人互动包）导入，不用重下整个客户端。

---

## 角色进度

| 角色 / 组合 | 内容 | 状态 | 说明 |
| :--- | :--- | :---: | :--- |
| **薇欧拉 × 仲町阿拉蕾**（薇蕾）<br /><sub>*BanG Dream! YUME∞MITA*</sub> | 双人单宠（含全向拖拽）+ 5 套双人互动（捏脸/推脸/理头发/揪兜帽/说悄悄话）+ 煎蛋彩蛋 | ![v0.5.1](https://img.shields.io/badge/v0.5.1-已完成-5AD8A6?style=flat-square) | [Releases](../../releases) / 群内网盘分流 |
| **MyGO!!!!!**（千早爱音 / 要乐奈 等） | 单人多姿态 + 全向拖拽 + 双人互动包 | ![WIP](https://img.shields.io/badge/进度-验收中-F6BD16?style=flat-square) | 做好后会先发群里，再同步到 Releases |

---

## 下载与交流

- **直接下载**：去右侧 **[Releases](../../releases)** 下载最新的 `win64.zip`（单一原画质完整包，内置标准/轻量模式开关）。
- **QQ 交流群**：`1137271893`（GitHub 下载慢可以进群拿网盘分流，新角色、新 `.duopack` 也会优先发群里，有 Bug 或想看的角色可以直接群里说）

> 原创形象（OC）或 VUP 如有专属桌宠合作意向，进群私聊群主即可。

---

## 运行模式与设备适配

软件内置**标准模式 / 轻量模式**一键切换（控制台 → 设置 → 运行模式），**两种模式均保持原画质不糊**：

| 对比项 | 标准模式（默认） | 轻量模式（办公 / 核显 / 省资源） |
| :--- | :--- | :--- |
| **清晰度** | 原画质（高清） | **同样保持原画质** |
| **拖拽方式** | 60Hz 全向丝滑拖拽（BC7 贴图池） | 静态贴图拖拽（不加载 BC7 拖拽贴图池，省显存与内存） |
| **互动节奏** | 完整日常待机与拉近自动双人互动 | 自动双人互动降频（冷却拉长 3 倍），主动点击/摸头正常回应 |
| **后台资源回收** | 常规常驻 | 辅助窗用完自动销毁；**被遮挡 / 全屏游戏自动暂停渲染** |

### 设备适配要求

- **系统**：Windows 10 / 11（64 位），暂不支持 macOS / Linux / 32 位系统。
- **显卡**：纯本地预渲染播放，**无需联网，也不需要高端独显或本地跑 AI**；支持 WebGL2 与 BC7 纹理的常见核显 / 独显均可运行（轻薄本/核显/游戏党建议在控制台切到「轻量模式」）。
- **内存与硬盘**：建议 `8 GB` 以上内存（标准模式双宠同屏建议 `16 GB` 内存 + 独显），预留约 `4 GB` 硬盘空间。

---

## 使用说明与常见问题

<details open>
<summary><strong>1. 怎么打开？（绿色包）</strong></summary>

<br />

1. 下完 `win64.zip` 后，**先完整解压到一个普通文件夹里**（别在压缩软件预览窗口里直接双击 `.exe`，也尽量不要放到 `C:\Program Files`，不然可能读不到资源或权限不足）。
2. 打开解压后的文件夹，双击 `PitaPet.exe` 启动（同目录的 `resources` 等文件别删）。
3. **基本操作**：
   - 按住角色随便拖；把两只拖近可触发 5 套随机双人互动（有冷却时间）。
   - 连点角色 6 次触发变身彩蛋；右下角系统托盘图标可打开控制台（切换标准/轻量模式、换角色、调大小/话痨度、导包、退出）。

</details>

<details>
<summary><strong>2. 怎么导入新的 <code>.petpack</code> / <code>.duopack</code>？</strong></summary>

<br />

打开右下角托盘「控制台」→「导入」，选中 `.petpack` 或 `.duopack` 文件即可。导完后在角色列表里手动添加到桌面，不会覆盖你原来的设置。

</details>

<details>
<summary><strong>3. Windows 弹蓝框提示“已保护你的电脑”怎么办？</strong></summary>

<br />

个人免费发的包没买商业签名证书，Windows SmartScreen 第一次见到新版本 `.exe` 都会弹这个。点 **更多信息 → 仍要运行** 就行。所有动画与核心功能均在本地运行；如启用匿名基础统计（仅统计活跃天数与互动次数用于优化体验，不含个人隐私），也可随时在控制台「设置 → 匿名使用统计」中一键关闭。

</details>

---

## 版权与防倒卖说明

1. 本仓库发布的《BanG Dream!》相关角色桌宠均为个人非营利同人二创，角色版权归原著作权方（Bushiroad Inc. / BanG Dream! Project 等）所有，**永久免费分享**，仅限个人桌面自用。
2. **禁止任何形式的倒卖**（闲鱼、淘宝、拼多多、付费网盘、付费群等），也禁止解包提取内部 `.webm` / `.bc7z` 素材二次分发或拿去炼丹。如果你是花钱买的，请直接退货并举报卖家。

完整协议见根目录 [LICENSE](./LICENSE)。
