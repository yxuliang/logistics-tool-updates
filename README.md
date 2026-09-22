# 物流工作台 · 软件更新

USPS / GOFO / SpeedX 物流标签批处理与表格自动化工具。此仓库仅用于分发软件与更新说明。

## 推荐下载：v2.11.4

- **[Windows x64 安装版（推荐）](https://github.com/yxuliang/logistics-tool-updates/releases/download/v2.11.4/USPS_GOFO_Label_Tool-2.11.4-Windows-x64-Setup.exe)**
- [Windows x64 便携版](https://github.com/yxuliang/logistics-tool-updates/releases/download/v2.11.4/USPS_GOFO_Label_Tool-2.11.4-Windows-x64-Portable.zip)
- [版本说明及文件校验值](https://github.com/yxuliang/logistics-tool-updates/releases/tag/v2.11.4)
- [全部历史版本](https://github.com/yxuliang/logistics-tool-updates/releases)

支持 Windows 10/11 x64，不需要安装 Python。本次没有 macOS 成品。
GitHub 自动生成的 Source code 压缩包只有本仓库说明，不是软件安装包。

## 首次安装与在线升级

1. 下载上方安装版，关闭正在运行的旧版软件后安装，沿用原安装目录。
2. 之后在软件右上角点击“检查软件更新”，按提示下载、校验并确认安装。
3. 首次检查需确认信任更新渠道；不会后台自动更新或强制安装。

初始版本 **v2.11.1** 保留在历史记录中。它的 GitHub 下载跳转兼容问题已在 **v2.11.2** 修复。
**2.11.1 及更早版本需要通过本页手动安装最新版本一次，不能依赖旧版的更新入口完成修复。2.11.2/2.11.3 用户可从软件内直接升级。**

2.11.4 新增：在“高级兼容”中可人工忽略 GTIN 校验位异常，按映射表原码和数量处理，保留全部数字和前导 0，报告记录人工忽略。默认关闭，更换映射表或重开软件后自动关闭；其他错误仍拦截。忽略校验不代表编码正确，请先核实映射表。

保留 2.11.3 的单击物流单号复制、不弹窗、大结果列表、可调分隔线和收起设置功能。

固定更新清单地址：
`https://github.com/yxuliang/logistics-tool-updates/releases/latest/download/latest.json`

已自行保存过其他更新地址的用户，可在软件更新窗口按需改为上方地址。

## 功能

- USPS、GOFO、SpeedX 面单和拣货单批处理，支持一单多 UPC，异常订单单独报告。
- SKU 新增入库、重复跳过、校验清理；独立于面单映射功能。
- ITA 订单金额回填、仓库邮编、按物流商生成智猴发货表。
- 单击物流单号复制；处理结果右键复制、Ctrl+C 复制选中行，完整报错及详情通过右键菜单查看。

## 数据与安全

业务 PDF、Excel、处理报告及本机新增 SKU 在本地处理，不上传到本仓库。
软件包包含用户已授权公开的内置 SKU 库。升级不删除独立保存在本机的 SKU 库。
不安装后台服务，不开机自启；只有用户主动检查或下载更新时联网。

安装包尚未进行商业代码签名。请核对下载来源及 SHA-256，并遵守设备安全策略，不要关闭系统安全防护。
不要向这个公开仓库提交订单、收件地址、原始面单、业务表格、密码或访问令牌。
