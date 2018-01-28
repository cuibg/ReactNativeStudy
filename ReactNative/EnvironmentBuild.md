# ReactNative环境搭建

## 安装

### 必需的软件

#### Chocolatey

[Chocolatey](https://chocolatey.org/)是一个Windows上的包管理器，类似于linux上的yum和 apt-get。 你可以在其[官方网站](https://chocolatey.org/)上查看具体的使用说明。一般的安装步骤应该是下面这样：

```
@powershell -NoProfile -ExecutionPolicy Bypass -Command "iex ((new-object net.webclient).DownloadString('https://chocolatey.org/install.ps1'))" && SET PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin
```
#### python 2

打开命令提示符窗口，使用Chocolatey来安装Python 2.

> **[warning] 注意目前不支持Python 3版本**

```
choco install python2
```

#### Node

打开命令提示符窗口，使用Chocolatey来安装NodeJS。

```
choco install nodejs.install
```

安装完node后建议设置npm镜像以加速后面的过程（或使用科学上网工具）。注意：不要使用cnpm！cnpm安装的模块路径比较奇怪，packager不能正常识别！

```
npm config set registry https://registry.npm.taobao.org --global
npm config set disturl https://npm.taobao.org/dist --global
```

#### Yarn、React Native的命令行工具（react-native-cli）

Yarn是Facebook提供的替代npm的工具，可以加速node模块的下载。React Native的命令行工具用于执行创建、初始化、更新项目、运行打包服务（packager）等任务,官方推荐Yarn

```
npm install -g yarn react-native-cli
```

安装完yarn后同理也要设置镜像源：

```
yarn config set registry https://registry.npm.taobao.org --global
yarn config set disturl https://npm.taobao.org/dist --global
```

>**[warning] 如果你遇到EACCES: permission denied权限错误，可以尝试运行下面的命令（限linux系统）： sudo npm install -g yarn react-native-cli**

安装完yarn之后就可以用yarn代替npm了，例如用yarn代替npm install命令，用yarn add 某第三方库名代替npm install --save 某第三方库名。

#### AndroidStudio

AndroidStudio 配置好sdk，模拟器，gradle等