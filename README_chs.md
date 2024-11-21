玩家对战游戏网络 - 专业版
=====
![](http://i.imgur.com/LfI3hXo.png)

PvPGN 是一款免费开源的跨平台服务器软件，支持 Battle.net 和 Westwood Online 游戏客户端。PvPGN-PRO 是官方 PvPGN 项目的一个分支，该项目的开发于 2011 年停止，PvPGN-PRO 的目标是为 PvPGN 提供持续维护和额外功能。

[![许可证 (GPL 版本 2)](https://img.shields.io/badge/license-GNU%20GPL%20version%202-blue.svg?style=flat-square)](http://opensource.org/licenses/GPL-2.0)
![语言 (C++)](https://img.shields.io/badge/powered_by-C++-brightgreen.svg?style=flat-square)
[![语言 (Lua)](https://img.shields.io/badge/powered_by-Lua-red.svg?style=flat-square)](https://lua.org)
[![Github 版本 (通过版本发布)](https://img.shields.io/github/downloads/pvpgn/pvpgn-server/1.99.7.2.1/total.svg?maxAge=2592000)]()

[![编译器 (Microsoft Visual C++)](https://img.shields.io/badge/compiled_with-Microsoft%20Visual%20C++-yellow.svg?style=flat-square)](https://msdn.microsoft.com/en-us/vstudio/hh386302.aspx)
[![编译器 (LLVM/Clang)](https://img.shields.io/badge/compiled_with-LLVM/Clang-lightgrey.svg?style=flat-square)](http://clang.llvm.org/)
[![编译器 (GCC)](https://img.shields.io/badge/compiled_with-GCC-yellowgreen.svg?style=flat-square)](https://gcc.gnu.org/)

[![构建状态](https://travis-ci.org/pvpgn/pvpgn-server.svg?branch=master)](https://travis-ci.org/pvpgn/pvpgn-server)
[![构建状态](https://ci.appveyor.com/api/projects/status/dqoj9lkvhfwthmn6)](https://ci.appveyor.com/project/HarpyWar/pvpgn)

[Deleaker](http://www.deleaker.com/) 帮助我们找到内存泄漏。

## 跟踪（Tracking）
默认情况下，跟踪已启用，仅用于向跟踪服务器发送信息数据（例如服务器描述、主页、正常运行时间、用户数量）。要禁用跟踪，请在“conf/bnet. conf”中设置“track=0”。

## 受支持的客户端
- **魔兽争霸 2：战网版（Warcraft 2: Battle.net Edition）**: 2.02a, 2.02b
- **魔兽争霸 3：混乱之治（Warcraft III: Reign of Chaos）**\*: 1.13a, 1.13b, 1.14a, 1.14b, 1.15a, 1.16a, 1.17a, 1.18a, 1.19a, 1.19b, 1.20a, 1.20b, 1.20c, 1.20d, 1.20e, 1.21a, 1.21b, 1.22a, 1.23a, 1.24a, 1.24b, 1.24c, 1.24d, 1.24e, 1.25b, 1.26a, 1.27a, 1.27b, 1.28, 1.28.1, 1.28.2, 1.28.4, 1.28.5
- **魔兽争霸 3：冰封王座（WarCraft 3: The Frozen Throne）**\*: 1.13a, 1.13b, 1.14a, 1.14b, 1.15a, 1.16a, 1.17a, 1.18a, 1.19a, 1.19b, 1.20a, 1.20b, 1.20c, 1.20d, 1.20e, 1.21a, 1.21b, 1.22a, 1.23a, 1.24a, 1.24b, 1.24c, 1.24d, 1.24e, 1.25b, 1.26a, 1.27a, 1.27b, 1.28, 1.28.1, 1.28.2, 1.28.4, 1.28.5
- **StarCraft**: 1.08, 1.08b, 1.09, 1.09b, 1.10, 1.11, 1.11b, 1.12, 1.12b, 1.13, 1.13b, 1.13c, 1.13d, 1.13e, 1.13f, 1.14, 1.15, 1.15.1, 1.15.2, 1.15.3, 1.16, 1.16.1, 1.17.0, 1.18.0
- **星际争霸：母巢之战（StarCraft: Brood War**: 1.08, 1.08b, 1.09, 1.09b, 1.10, 1.11, 1.11b, 1.12, 1.12b, 1.13, 1.13b, 1.13c, 1.13d, 1.13e, 1.13f, 1.14, 1.15, 1.15.1, 1.15.2, 1.15.3, 1.16, 1.16.1, 1.17.0, 1.18.0
- **Diablo**: 1.09, 1.09b
- **Diablo 2**: 1.10, 1.11, 1.11b, 1.12a, 1.13c, 1.14a, 1.14b, 1.14c, 1.14d
- **暗黑破坏神 2：毁灭之王（Diablo 2: Lord of Destruction）**: 1.10, 1.11, 1.11b, 1.12a, 1.13c, 1.14a, 1.14b, 1.14c, 1.14d
- **Westwood Chat 客户端**: 4.221
- **命令与征服（Command & Conquer）**: Win95 1.04a (使用 Westwood Chat)
- **命令与征服：红色警戒（Command & Conquer: Red Alert）**: Win95 2.00 (使用 Westwood Chat), Win95 3.03
- **命令与征服：红色警戒2（Command & Conquer: Red Alert 2）**: 1.006
- **命令与征服：泰伯利亚之日（Command & Conquer: Tiberian Sun）**: 2.03 ST-10
- **命令与征服：泰伯利亚之日—火线风暴（Command & Conquer: Tiberian Sun Firestorm）**: 2.03 ST-10
- **命令与征服：尤里的复仇（Command & Conquer: Yuri's Revenge）**: 1.001
- **命令与征服：变节者（Command & Conquer: Renegade）**: 1.037
- **救世传说（Nox）**: 1.02b
- **救世传说扩展包（Nox Quest）**: 1.02b
- **沙丘2000（Dune 2000）**: 1.06
- **帝王：沙丘之战（Emperor: Battle for Dune）**: 1.09

\* 如果不通过 [W3L](https://github.com/w3lh/w3l) 等工具进行客户端修改以禁用服务器签名验证，WarCraft 3客户端将无法连接到PvPGN服务器。
\* 由于协议变更，从 1.18 补丁开始的《星际争霸》客户端将不受 PvPGN-PRO 支持。为了与机器人软件兼容，包含了一个 1.18.0 版本检查条目。

## 支持Support
[创建一个问题](https://github.com/pvpgn/pvpgn-server/issues) 如果您对PvPGN-PRO有任何问题、建议或其他要说的。请注意，D2GS不是PvPGN项目的一部分，因此在这里不受支持。
在获取日志并发布之前，在“bnet. conf”中设置“loglevels=致命、fatal,错误、error,警告、warn,信息、info,调试、debug,跟踪、trace` ”。
## Development
提交拉取请求以为该项目做出贡献。尽可能利用C++11个功能并遵守[C++核心指南](https://github.com/isocpp/CppCoreGuidelines/blob/master/CppCoreGuidelines.md) 。

## Building
有关已确认与PvPGN一起使用的操作系统和编译器，请参阅  [docs/ports.md](https://github.com/pvpgn/pvpgn-server/blob/master/docs/ports.md)  任何支持WinAPI或POSIX的操作系统，以及任何符合C++11的编译器都应该能够构建PvPGN。CMake文件已被硬编码，以拒绝比Visual Studio 2015和GCC 5.1更早的编译器。

#### Windows
使用 [Magic Builder](https://github.com/pvpgn/pvpgn-magic-builder).

或者，使用 CMake 生成.sln 项目并从 Visual Studio 进行构建。
```
cmake -g "Visual Studio 14 2015" -H./ -B./build
```
这将在“build”目录中生成. sln。

#### 一般的 Linux
不要盲目运行这些命令。旧版本发行版的主要问题是安装 CMake 3.2.x 和 GCC 5，因此在示例中使用了外部存储库。

```
apt-get install git install cmake make build-essential zlib1g-dev
apt-get install liblua5.1-0-dev #Lua support
apt-get install mysql-server mysql-client libmysqlclient-dev #MySQL support
cd /home
git clone https://github.com/pvpgn/pvpgn-server.git
cmake -D CMAKE_INSTALL_PREFIX=/usr/local/pvpgn -D WITH_MYSQL=true -D WITH_LUA=true ../
make
make install
```

#### Ubuntu 16.04, 18.04
```
sudo apt-get -y install build-essential git cmake zlib1g-dev
git clone https://github.com/pvpgn/pvpgn-server.git
cd pvpgn-server && cmake -G "Unix Makefiles" -H./ -B./build
cd build && make
```

#### Ubuntu 14.04
```
sudo apt-get -y install build-essential zlib1g-dev git
sudo add-apt-repository -y ppa:ubuntu-toolchain-r/test
sudo apt-get -y update
sudo apt-get -y install gcc-5 g++-5
sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-5 60 --slave /usr/bin/g++ g++ /usr/bin/g++-5
sudo add-apt-repository -y ppa:george-edison55/cmake-3.x
sudo apt-get update
sudo apt-get -y install cmake
git clone https://github.com/pvpgn/pvpgn-server.git
cd pvpgn-server && cmake -G "Unix Makefiles" -H./ -B./build
cd build && make
```

#### Debian 8 搭配 clang 编译器
```
sudo apt-get -y install build-essential zlib1g-dev clang libc++-dev git
wget https://cmake.org/files/v3.7/cmake-3.7.1-Linux-x86_64.tar.gz
tar xvfz cmake-3.7.1-Linux-x86_64.tar.gz
git clone https://github.com/pvpgn/pvpgn-server.git
cd pvpgn-server && CC=/usr/bin/clang CXX=/usr/bin/clang++ ../cmake-3.7.1-Linux-x86_64/bin/cmake -G "Unix Makefiles" -H./ -B./build
cd build && make
```

#### CentOS 7
```
sudo yum -y install epel-release centos-release-scl
sudo yum -y install git zlib-devel cmake3 devtoolset-4-gcc*
sudo ln -s /usr/bin/cmake3 /usr/bin/cmake
git clone https://github.com/pvpgn/pvpgn-server.git
cd pvpgn-server
CC=/opt/rh/devtoolset-4/root/usr/bin/gcc CXX=/opt/rh/devtoolset-4/root/usr/bin/g++ cmake -G "Unix Makefiles" -H./ -B./build
cd build && make
```

#### Fedora 25
```
sudo dnf -y install gcc-c++ gcc make zlib-devel cmake git
git clone https://github.com/pvpgn/pvpgn-server.git
cd pvpgn-server
cmake -G "Unix Makefiles" -H./ -B./build
cd build && make
```

#### FreeBSD 11
```
sudo pkg install -y git cmake
git clone https://github.com/pvpgn/pvpgn-server.git
cd pvpgn-server
cmake -G "Unix Makefiles" -H./ -B./build
cd build && make
```

完整说明: [Русский](http://harpywar.com/?a=articles&b=2&c=1&d=74) | [English](http://harpywar.com/?a=articles&b=2&c=1&d=74&lang=en)

## 在局域网或具有私有 IP 地址的虚拟专用服务器上托管。
一些VPS提供商不会为您的服务器分配直接的公共IP。如果是这种情况，或者您在NAT后面的家中主机，您需要在“address_translation. conf”中设置路由转换。公共地址在寻找游戏时作为路由服务器地址推送给游戏客户端。未能将正确的地址推送给游戏客户端会导致玩家无法匹配和加入游戏（长时间游戏搜索和错误）。

如果你的网络接口直接绑定到公共 IP，PvPGN 可以自行确定，此步骤并非必要。

## 许可证

    This program is free software; you can redistribute it and/or
    modify it under the terms of the GNU General Public License
    as published by the Free Software Foundation; either version 2
    of the License, or (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program; if not, write to the Free Software
    Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
