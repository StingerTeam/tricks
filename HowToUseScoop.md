# HowToUseScoop

## 介绍

Scoop是Windows下的包管理器，类似于Linux下的apt-get、yum等，可以方便地安装和更新一些常用软件，尤其是开源软件，以及一些运行环境，如node.js、python、java、php等。

使用Scoop可以方便的安装、卸载、更新软件，更换软件版本，而且可以自动处理依赖关系。

## GitHub仓库

<https://github.com/ScoopInstaller/Scoop>

## 安装

Run the following command from a non-admin PowerShell to install scoop to its default location `C:\Users\<YOUR USERNAME>\scoop`.

从非管理员 PowerShell 运行以下命令，将 scoop 安装到其默认位置 `C:\Users\<YOUR USERNAME>\scoop` 。

```powershell
iwr -useb get.scoop.sh | iex
```

Advanced installation instruction and full documentation of the installer are available in [ScoopInstaller/Install](https://github.com/ScoopInstaller/Install). Please create new issues there if you have questions about the installation.

[ScoopInstaller/Install](https://github.com/ScoopInstaller/Install) 中提供了高级安装说明和安装程序的完整文档。如果您对安装有疑问，请在那里创建新问题。

## 应用程序桶(Bucket)

Scoop使用桶来组织应用程序。默认情况下，Scoop安装`main`桶

推荐的桶：`extras`, `versions`

### 添加桶

```powershell
scoop bucket add <name>
```

例如：

```powershell
scoop bucket add extras
```

## 搜索应用程序

```powershell
scoop search <app_name>
```

例如：

```powershell
# 搜索java
scoop search openjdk
```

```txt
Results from local buckets...

Name                Version    Source Binaries
----                -------    ------ --------
openjdk-ea          22-29-ea   java
openjdk             21.0.1-12  java
openjdk10           10.0.2-13  java
openjdk11           11.0.2-9   java
openjdk12           12.0.2-10  java
openjdk13           13.0.2-8   java
openjdk14           14.0.2-12  java
openjdk15           15.0.2-7   java
openjdk16           16.0.2-7   java
openjdk17           17.0.2-8   java
openjdk18           18.0.2.1-1 java
openjdk19           19.0.2-7   java
openjdk20           20.0.2-9   java
openjdk21           21.0.1-12  java
openjdk22           22-29-ea   java
openjdk7-unofficial 7u80-b32   java
openjdk8-redhat-jre 8u342-b07  java
openjdk8-redhat     8u342-b07  java
openjdk9            9.0.4-12   java
```

## 安装应用程序

```powershell
scoop install <app_name>
```

例如：

```powershell
scoop install openjdk17
```

使用Scoop安装应用程序后会自动添加到环境变量中，一般可以直接在命令行中使用（针对非图形界面软件）。

## 安装特定版本的应用程序

```powershell
scoop install <app_name>@<version>
```

例如：

```powershell
scoop install python@3.8.9 python@3.11.7
```

## 切换某个应用程序的版本

```powershell
scoop reset <app_name>
```

例如：

```powershell
scoop reset python@3.11.7
```

说明：reset可以理解为重新配置环境变量，即将`python`命令指向指定版本的python可执行文件。

## 卸载应用程序

```powershell
scoop uninstall <app_name>
```
