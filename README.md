# Snack App 交互原型

[在线预览](https://sweemondr.github.io/snack-app-prototype/)

Snack 移动端交互演示，包含聊天、日程、持续跟进和资料库。

## 预览

下载或克隆仓库后，直接用浏览器打开 `index.html`。页面所需的样式、脚本、Logo 和图标均已内嵌，无需安装依赖。

需要通过本地服务预览时，在仓库目录运行：

```sh
python3 -m http.server 8000
```

然后打开 <http://localhost:8000>。

## 当前交互

- 授权分为连接说明、供应商授权确认、连接成功、选择会议。支持取消、全选/取消全选和选中数量。
- 选中会议统一开启会前准备、会中记录和会后跟进，重复导入不会重复创建。
- 支持钉钉、企业微信、飞书与系统日历；手动日程在聊天中收集信息并确认。断开来源后保留历史并停止该来源的新跟进检查。
- 持续跟进空态采用分组点子，支持描述自己的事项；已完成目标可重新开始新一轮。
- 资料库记忆采用摘要与三个目录：身份与偏好、跟进与历史、日程与会议。可补充、纠正、查看来源、搜索和删除记忆。
- 设置保留秘书名称、连接应用、通知与提醒、关于我的了解与关于 Snack，移除重复提醒开关和重复偏好入口。
- 白色页面、橙色强调；实心橙色按钮使用白字。

## 参考

授权参考 [Google 授权流程](https://support.google.com/accounts/answer/14012355?hl=en)和 [Notion 连接流程](https://www.notion.com/help/add-and-manage-connections-with-the-api)。设置按 [Muse 连接应用](https://www.meta.com/help/superintelligence/1687253048996149/)与[权限管理](https://www.meta.com/help/superintelligence/1385290430137537/)的公开说明取舍，未声称完整复刻其设置页。点子与记忆结构参考用户提供的 Muse / Today 截图。

## 演示边界

日程、授权、录音、业务数据与 AI 处理使用预设数据或本地交互模拟，不执行真实业务授权或数据读取。上传仅保存文件名，不读取、上传或解析文件内容。交互状态保存在浏览器本地存储中。

当前副本来自 2026-11-16 修订的本地原型，内容与原 HTML 一致。

## 图标来源

钉钉图标来自[钉钉官网](https://www.dingtalk.com/)的[官方图标资源](https://gw.alicdn.com/imgextra/i3/O1CN014ZbI6ZTEhdC0ttN2_!!6000000003783-2-tps-444-444.png)，已内嵌于页面。
