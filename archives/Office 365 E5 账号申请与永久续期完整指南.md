# Office 365 E5 账号申请与永久续期完整指南

Office 365 E5 是微软为开发者提供的免费临时管理账号，拥有丰富的功能权益，包括分配 25 个子账号、OneDrive 5T 存储以及完整的 Office 客户端使用权。本文将详细介绍如何申请 Office 365 E5 账号，并实现永久自动续期。

## 申请 Office 365 E5 账号

1. **打开申请页面**  
   访问 [Microsoft 365 开发者计划页面](https://developer.microsoft.com/microsoft-365/dev-program)，使用你的微软账户登录。如果没有账户，点击“创建一个”并按步骤完成注册。

2. **填写基本信息**  
   登录后，选择国家，随意填写公司名称，勾选“接受条款”，然后点击“下一步”。

3. **个性化体验设置**  
   在个性化体验页面，随意勾选几个必选项，点击“加入”。

4. **设置 E5 订阅**
   进入下一页面后，点击“设置 E5 订阅”。在弹出的对话框中填写国家、用户名、域名和密码，并保存密码。域名是网址前缀，如果提示已被使用，可尝试其他字母组合。

5. **绑定手机号**  
   按照提示绑定手机号，完成人机验证。填入收到的验证码，点击“设置”。

6. **订阅成功**  
   等待约一分钟，页面将显示订阅成功。

## 开始使用 Office 365 E5

订阅成功后，访问 [Office 官网](https://www.office.com)，使用管理员账号和密码登录。关闭向导后，即可使用网页端的 OneDrive 和 Office 应用。如需使用客户端，点击右上角的“安装 Office - Office 365 应用”，下载并安装。

👉 [WildCard | 一分钟注册，轻松订阅海外线上服务](https://bbtdd.com/WildCard)

## 扩展 OneDrive 存储空间

默认情况下，OneDrive 空间为 1T，可通过以下步骤扩展至 5T：

1. 打开 [OneDrive 存储管理页](https://admin.onedrive.com/?v=StorageSettings)，登录管理员账号。
2. 将存储空间设置为 5120，点击“保存”。  
   如果页面无法加载，可能是系统未完成初始化，等待 24 小时后重试。

## 分配子账号

管理员可分配 25 个子账号，每个账号均享有 Office 365 和 5T OneDrive 空间：

1. 在管理页面点击“管理”按钮，进入管理员中心。
2. 选择左侧菜单栏的“用户 - 活跃用户”，点击“添加用户”。
3. 填写必要信息后，点击“下一步”。
4. 在接下来的步骤中，保持默认选项，完成用户添加。

## 实现永久自动续期

Office 365 E5 订阅的有效期为 90 天。如果微软检测到账号被用于开发（如 API 被频繁调用），将自动续期。以下是实现永久续期的步骤：

1. **使用 Github Action**  
   Github Action 是 Github 提供的虚拟 Linux 环境，可通过定时任务执行指定代码。  
   首先，登录或注册一个 Github 账号。

2. **导入私有仓库**  
   打开 [AutoApiSecret 仓库](https://github.com/vcheckzen/AutoApiSecret)，点击“Fork”并导入为私有仓库。

3. **创建个人访问密钥**  
   访问 [密钥创建页面](https://github.com/settings/tokens/new)，创建一个具有 workflow 权限的密钥，复制备用。

4. **关闭两步验证**  
   按照 [微软官方文档](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults) 关闭 E5 管理员账号的两步验证。

5. **触发注册流程**  
   在 Github 仓库的 Action 面板中，找到“Register APP”并手动触发。等待 2 分钟左右完成注册。

通过以上步骤，即可实现 Office 365 E5 的永久自动续期，确保账号长期可用。