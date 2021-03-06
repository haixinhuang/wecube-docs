# 上手指引：安装并运行WeCube

现在，我们开始在腾讯云华南地区来创建资源并安装以单机模式运行的WeCube。为此，您需要拥有一个可以正常使用的腾讯云用户账号并准备好在安装过程中会使用到的该账号的API密钥。

此外，在安装完成后，您还将需要为WeCube准备一个供其在运行过程中使用的API密钥。您可以复用在安装过程中使用过的API密钥，当然，也完全可以额外分配一个新的API密钥。

!!! info "提示"
    请注意，WeCube的安装过程需要在腾讯云上创建按量付费使用的云资源，因此，根据腾讯云的要求，您的账号中需要有一定的余额才能正常进行安装过程。

!!! warning "请留意并谨慎评估您使用的API密钥所属的用户账号的权限设定，以免在后续使用和操作WeCube时为您现有的云上资产带来安全风险。"

## 在腾讯云上安装和启动WeCube

!!! note ""
    关于安装WeCube，请参见文档 “[在公有云上以单机模式安装WeCube](standalone-mode-on-public-cloud.md)”。

安装完成后，请使用预置的用户名`umadmin`和密码`umadmin`来访问云上的WeCube。

## 确认WeCube使用的云资源

WeCube的部署完成后，您可以登录腾讯云控制台确认本次部署中创建并使用的云资源情况：

在“云服务器”产品下，您可以在`华南地区（广州）`找到名称为“`instance_wecube_platform`”的云服务器实例，它运行了单机部署方案下所有WeCube平台服务和插件服务。您可以根据需要自行对实例进行资源和配置的调整、重置密码、销毁释放等管理操作。在当前WeCube的版本条件下，我们建议保留至少 **4核CPU的计算资源** 和 **16GB的内存资源**，以满足正常运行的需要。

在“私有网络”产品下，您可以在`华南地区（广州）`找到名称为“`GZ_MGMT`”的私有网络，其中包含一个名称为“`GZP2_MGMT_MT_APP`”的子网，WeCube运行使用的云服务器实例“`instance_wecube_platform`”就包含在这个子网之中。

## 进一步了解

关于WeCube安装的详细信息，请参见以下文档：

- [在私有资源上以单机模式安装](standalone-mode-on-premises.md)
- [在公有云上以单机模式安装](standalone-mode-on-public-cloud.md)
