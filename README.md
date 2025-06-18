# maipluginv2
MaiBot 0.8.0 (v2)插件公共仓库

本仓库是<a href="https://github.com/MaiM-with-u/MaiBot">MaiBot</a>V2的插件合集

## 🔥 安装0.8.0

**最新Dev版本: v0.8.0** 
可前往 [Release](https://github.com/MaiM-with-u/MaiBot/tree/dev#) 页面查看最新版本

**GitHub 分支说明：**
- `main`: 稳定发布版本(推荐)
- `dev`: 开发测试版本(不稳定)

### 最新dev版本部署教程
- 如何从0.7升级:不到
- Linux全新安装0.8:
```
#如果无法连接Github可以使用镜像源https://gh-proxy.com/原地址
```
 第一步:获取文件
```
mkdir MaiBotv2
cd MaiBotv2
git clone -b dev https://github.com/MaiM-with-u/MaiBot.git
git clone -b dev https://github.com/MaiM-with-u/MaiBot-Napcat-Adapter.git
```
 第二步:配置环境
```
# 确保Python在3.10及以上
python3 --version
```
```
# 如果版本低于3.10，请更新Python版本。
# 此处以 Python 3.12 为例
# Ubuntu/Debian
sudo apt update
sudo apt install python3.12 python3.12-venv
# 如执行了这一步，建议在执行时将python3指向python3.12
# 更新替代方案，设置 python3.12 为默认的 python3 版本:
sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.12
sudo update-alternatives --config python3
```
```
#创建虚拟环境
python3 -m venv MaiBot/venv      # 创建虚拟环境    
source MaiBot/venv/bin/activate  # 激活环境
```
 第三步:安装依赖
```
cd MaiBot
pip install uv -i https://mirrors.aliyun.com/pypi/simple
uv pip install -i https://mirrors.aliyun.com/pypi/simple -r requirements.txt --upgrade
```
如果此处quick_algo安装失败:
（一）
基于Debian的系统（如Ubuntu、Linux Mint等）
```
# 更新软件包索引
sudo apt update
# 运行以下命令来安装`gcc`和`g++`：
sudo apt install build-essential
```
基于Red Hat的系统（如Fedora、CentOS、RHEL等）
```
# 更新软件包索引
sudo dnf check-update
# 安装`gcc`和`g++`
sudo dnf install gcc gcc-c++
# 如果使用的是`yum`，将`dnf`替换为`yum`即可
```
安装完成后执行
```
gcc --version
g++ --version
# 如果安装成功，会显示`gcc`和`g++`的版本信息。
```
（二）

## 💬 讨论（仅显示空余可用）
- 麦麦QQ[四群](https://qm.qq.com/q/wGePTl1UyY) 

## 📚 文档

**部分内容可能更新不够及时，请注意版本对应**

- [📚 核心 Wiki 文档](https://docs.mai-mai.org) - 项目最全面的文档中心，你可以了解麦麦有关的一切。

## 麦麦仓库状态

![Alt](https://repobeats.axiom.co/api/embed/9faca9fccfc467931b87dd357b60c6362b5cfae0.svg "麦麦仓库状态")

## License

GPL-3.0
