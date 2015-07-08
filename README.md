# oh-my-vpn!
Setup your own OpenVPN server in ~30 seconds! and secure your naked internet connections before it is too late.

### Server Setup
Pick a new cheap server, CPU and Memory does not really matter
Cloud providers are awesome for this setup

### Use the one-liner script (Server):
```
curl -L https://git.io/pdTu | sh
```
This will take care about setting up the Server for you, and generates the client config files for you at the following paths:

- ```/root/client.conf```
- ```/root/client.ovpn```

The client config files are actually ```Readable``` and ```Identical```, But some OpenVPN clients requires different file extension.

### Post-Installation (Client):

- Install OpenVPN client your machine.
- Copy the client configurations file ```client.conf``` or ```client.ovpn``` and import it to your favorite OpenVPN client.
- Server supports up to 3 connected clients, assuming you use it on your Laptop, Smart-Phone and Tablet.

### Supported Operating Systems (Tested):

- ``` Ubuntu 14.10 ```
- ``` Ubuntu 14.04 ```
- ``` Ubuntu 13.10 ```
- ``` Debian 7.0 ```
- ``` Debian 7.4 ```
- ``` Debian 7.6 ```
- ``` Debian 7.8 ```

### TODO
- Build Docker image for Server
- Build Docker image for client and route client connections through the container 
- Pipe-line the project to Travis-ci for continous testing
- Add Support for other platforms: Centos, Fedora, OpenSUSE, Archlinux, Gentoo
- Add Multi-Client support
- Improve the README

#### Contribute
- Fork and submit pull requests
- For new features or refactoring make sure all kitchen tests pass on all platforms
- You can run the tests:
```
cd cookbooks/openvpn/
kitchen verify -c 6
```
哦，我的-VPN！
在安装约30秒钟内你自己的OpenVPN服务器！并保护您的赤裸的互联网连接之前，为时已晚。

服务器安装

选择一个新的廉价的服务器，CPU和内存都无所谓云提供商是真棒，对于这种设置

使用单行脚本（服务器）：

curl -L https://git.io/pdTu | sh
这会照顾有关设置为你的服务器，并在以下路径生成客户端配置文件，为您提供：

/root/client.conf
/root/client.ovpn
客户端配置文件实际上是可读可完全相同，但有些客户的OpenVPN需要不同的文件扩展名。

安装后（客户端）：

安装OpenVPN客户端机器。
复制客户端配置文件client.conf或client.ovpn并将其导入到自己喜欢的OpenVPN客户端。
服务器最多可支持3连接的客户端，假设你在你的笔记本电脑，智能手机和平板电脑使用。
支持的操作系统（测试）：

- ``` Ubuntu 14.10 ```
- ``` Ubuntu 14.04 ```
- ``` Ubuntu 13.10 ```
- ``` Debian 7.0 ```
- ``` Debian 7.4 ```
- ``` Debian 7.6 ```
- ``` Debian 7.8 ```

构建多克图像服务器
构建多克图像通过容器客户端和路由客户端连接
管线工程特拉维斯-CI的连续测试
增加支持其他平台：Centos，Fedora，OpenSUSE，Archlinux，Gentoo
添加多客户端支持
完善的自述
贡献

叉，并提交请求拉
对于新的功能或重构确保所有的厨房测试通过所有平台上
您可以运行测试：
cd cookbooks/openvpn/
kitchen verify -c 6
