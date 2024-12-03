# Nodepay Automate with Proxies 
使用代理自动化Nodepay网络。重要！请阅读以下信息：
- 旧版本不再工作，请使用``run.py``！对于Windows用户，请使用[WSL](https://learn.microsoft.com/en-us/windows/wsl/install)
- 最新的curl_cffi模块（用于模拟chrome131版本）``curl_cffi==0.8.0b7``未从Windows Python库服务器更新。我尝试了模拟chrome110版本和其他版本，但仍然出现错误，稳定的模拟版本是chrome131版本。
- 该机器人仅支持Linux和[WSL](https://learn.microsoft.com/en-us/windows/wsl/install) Windows.
- 该机器人支持多个账户。支持socks和http代理。每个账户使用3个代理。

## 所需工具和组件
1. Nodepay账户 | 注册：[https://app.nodepay.ai/register](https://app.nodepay.ai/register)
2. VPS（可选）和Python3
3. 代理

## 购买代理
- 免费代理静态住宅：
1. [WebShare](https://www.webshare.io/?referral_code=p7k7whpdu2jg)
2. [ProxyScrape](https://proxyscrape.com/?ref=odk1mmj)
3. [MonoSans](https://github.com/monosans/proxy-list)
- 付费优质静态住宅：
1. [922proxy](https://www.922proxy.com/register?inviter_code=d03d4fed)
2. [Proxy-Cheap](https://app.proxy-cheap.com/r/JysUiH)
3. [Infatica](https://dashboard.infatica.io/aff.php?aff=544)

# 设置教程
- 打开[Nodepay](https://app.nodepay.ai/register?ref=ZUCBuJaIoBXLE6J)并登录到仪表板
- 按F12或CTRL + SHIFT + I
- 选择控制台并输入```allow pasting```然后按回车
- 然后输入``localStorage.getItem('np_token')``并按回车
- 出现的文本是您的nodepay令牌，请复制该文本

# 组件安装

### LINUX
- 对于Linux，安装Python3和Git：
```bash
apt update; apt upgrade -y; apt install git python3 python3-pip -y
```
- 使用Git下载此脚本：
```bash
git clone https://github.com/Horizen5/Nodepay-automate.git
```
- 安装要求，请确保您在此脚本目录中：
```bash
python3 -m pip install -r requirements.txt
```
### Windows
git仓库
```bash
git clone https://github.com/Horizen5/Nodepay-automate.git
```
安装依赖
```bash
pip install -r requirements.txt
```

# 运行机器人
- 在```proxies.txt```中替换代理示例为您自己的代理，请仅使用3个代理。如果您运行多个账户，请确保每个账户有3个代理。
- 对于多个账户，请在文件``tokens.txt``中逐行插入您的令牌。

## 运行命令
- 运行Linux - 单账户：
```bash
python3 run.py
```
> 按回车，选择1，然后插入您的nodepay令牌
- 运行Linux - 多账户：
> 确保您在``tokens.txt``中有令牌
```bash
python3 run.py
```
 - 对于windows
```bash
python run.py
```
> 按回车然后选择2

# 操作状态
如果出现以下日志，则表示运行成功。
```bash
[2024-12-02 14:54:54] [INFO] 账户: user@email.com | 浏览器ID: xxxxxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx | IP: 127.0.0.1 | IP评分: 99
[2024-12-02 14:54:58] [INFO] 账户: user@email.com | 浏览器ID: xxxxxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx | IP: 127.0.0.1 | IP评分: 86
[2024-12-02 14:54:59] [INFO] 账户: user@email.com | 浏览器ID: xxxxxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx | IP: 127.0.0.1 | IP评分: 92
[2024-12-02 14:55:02] [INFO] 账户: user@email.com | 浏览器ID: xxxxxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx | IP: 127.0.0.1 | IP评分: 81
[2024-12-02 14:55:11] [INFO] 账户: user@email.com | 浏览器ID: xxxxxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx | IP: 127.0.0.1 | IP评分: 82
```

# 注意事项
- 运行此机器人，它将更新您的推荐代码为我的邀请代码，如果您没有一个。
- 一个账户只能连接3个代理。如果您运行多个账户，请确保每个账户有3个代理。
- 如果您运行脚本仍然出现错误，请使用付费代理，因为并非所有免费代理都受支持。
- 您可以自行风险运行此机器人，我不对因该机器人造成的任何损失或损害负责。此机器人仅用于教育目的。

