# 谷歌 AI Pro 助手

**Google AI Pro Helper｜本地自动化控制台**

想试 Google AI Pro，又不想反复折腾登录、订阅和查看结果？这个项目把相关流程放进了一个本地网页控制台，账号任务、执行进度和日志集中查看。

## 能做什么？

| 功能 | 说明 |
| --- | --- |
| 账号任务管理 | 导入账号，单独执行或批量处理 |
| 登录验证 | 按账号情况处理辅助邮箱或 2FA（双重验证） |
| 订阅流程 | 上游提供面向两年 AI Pro 的分阶段自动化流程 |
| 续订管理 | 按配置执行取消自动续订流程 |
| 结果查看 | 在控制台查看任务状态、日志和核验截图 |

功能依据 [原项目说明](https://github.com/worldonlyu/Google_AI_Pro_2Year_ZeroCost_Auto) 整理，实际订阅结果以 Google 页面为准。[实时检索｜上游 README 与源码｜可信度高（功能描述，未实测开通结果）]

## 先准备这几个东西

- **Windows 10／11**。
- **Google Chrome 浏览器**。
- **Python 3.10 或更高版本**，安装时勾选 `Add Python to PATH`（添加到系统路径）。
- 你自己拥有或获授权管理的 Google 账号，以及需要的验证方式。
- 上游要求的网络环境和本人可用的支付方式；具体条件查看 [原版说明](https://github.com/worldonlyu/Google_AI_Pro_2Year_ZeroCost_Auto/blob/main/README.md)。

## 怎么启动？

1. 点击仓库上方 **Code → Download ZIP**，下载后解压。
2. 打开解压后的项目文件夹。启动脚本就在根目录。
3. 首次使用，双击 **`1_首次运行_安装依赖并启动.bat`**。
4. 以后使用，双击 **`2_启动控制台.bat`**。
5. 按上游说明，浏览器会打开本地控制台：**`http://127.0.0.1:8765`**。

## 打开以后怎么用？

1. **检查配置**：核对控制台中的运行设置，再保存。
2. **导入账号**：按页面提示填写你自己的账号信息。
3. **先试一个**：点击单个任务的执行按钮，查看日志和页面反馈。
4. **确认结果**：检查账号订阅页面、续费日期和核验截图，再决定是否处理其他任务。

需要详细操作说明，直接看 [上游 README](https://github.com/worldonlyu/Google_AI_Pro_2Year_ZeroCost_Auto/blob/main/README.md)。

## 文件在哪里？

| 文件 | 用途 |
| --- | --- |
| `app.py` | 本地网页服务与任务接口 |
| `automation_engine.py` | 浏览器自动化执行逻辑 |
| `templates/index.html` | 控制台页面 |
| `config.json` | 本地运行配置 |
| `requirements.txt` | Python 依赖 |
| 两个 `.bat` 文件 | 安装依赖与启动控制台 |

## 使用时注意

- 确认订阅前，看清实际金额、附加项目和自动续费日期。
- 本地配置会涉及账号和支付信息，修改后的 `config.json`、登录数据、日志和截图不要上传到公开仓库。
- 遇到异常，先看日志，再核对账号实际状态，避免反复提交。

## 项目来源

原项目：[worldonlyu/Google_AI_Pro_2Year_ZeroCost_Auto](https://github.com/worldonlyu/Google_AI_Pro_2Year_ZeroCost_Auto)。本仓库保留其代码与提交历史，整理中文使用说明。
