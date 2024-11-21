Player 对 Player Gaming Network - PRO


PvPGN 是一款免费的开源跨平台服务器软件，支持 Battle.net 和 Westwood Online 游戏客户端。PvPGN-PRO 是官方 PvPGN 项目的一个分支，其开发于 2011 年停止，旨在为 PvPGN 提供持续的维护和附加功能。

许可证（GPL 版本 2） 语言 （C++） 语言 （Lua） Github 版本（按版本）

编译器 （Microsoft Visual C++） 编译器 （LLVM/Clang） 编译器 （GCC）

构建状态 构建状态

Deleaker 帮助我们找到内存泄漏。

跟踪
默认情况下，跟踪处于启用状态，并且仅用于将信息数据（例如服务器描述、主页、正常运行时间、用户数量）发送到跟踪服务器。要禁用跟踪，请在 中设置。track = 0conf/bnetd.conf

支持的客户端
魔兽争霸 2：Battle.net 版：2.02a、2.02b
魔兽争霸 3：混沌之治*：1.13a、1.13b、1.14a、1.14b、1.15a、1.16a、1.17a、1.18a、1.19a、1.19b、1.20a、1.20b、1.20c、1.20d、1.20e、1.21a、1.21b、1.22a、1.23a、1.24a、1.24b、1.24c、1.24d、1.24e、1.25b、1.26a、1.27a、1.27b、1.28、1.28.1、1.28.2、1.28.4、1.28.5
魔兽争霸 3：冰封王座*：1.13a、1.13b、1.14a、1.14b、1.15a、1.16a、1.17a、1.18a、1.19a、1.19b、1.20a、1.20b、1.20c、1.20d、1.20e、1.21a、1.21b、1.22a、1.23a、1.24a、1.24b、1.24c、1.24d、1.24e、1.25b、1.26a、1.27a、1.27b、1.28、1.28.1、1.28.2、1.28.4、1.28.5
星际争霸：1.08、1.08b、1.09、1.09b、1.10、1.11、1.11b、1.12、1.12b、1.13、1.13b、1.13c、1.13d、1.13e、1.13f、1.14、1.15、1.15.1、1.15.2、1.15.3、1.16、1.16.1、1.17.0、1.18.0
星际争霸：母巢之战：1.08、1.08b、1.09、1.09b、1.10、1.11、1.11b、1.12、1.12b、1.13、1.13b、1.13c、1.13d、1.13e、1.13f、1.14、1.15、1.15.1、1.15.2、1.15.3、1.16、1.16.1、1.17.0、1.18.0
暗黑破坏神：1.09、1.09b
暗黑破坏神 2：1.10、1.11、1.11b、1.12a、1.13c、1.14a、1.14b、1.14c、1.14d
暗黑破坏神 2：毁灭之王：1.10、1.11、1.11b、1.12a、1.13c、1.14a、1.14b、1.14c、1.14d
Westwood Chat 客户端：4.221
命令与征服：Win95 1.04a（使用Westwood Chat）
命令与征服：红色警报：Win95 2.00（使用Westwood Chat），Win95 3.03
命令与征服：红色警戒2：1.006
命令与征服：泰伯利亚太阳：2.03 ST-10
命令与征服：泰伯利亚太阳火风暴：2.03 ST-10
命令与征服：尤里的复仇：1.001
命令与征服：叛徒：1.037
氮氧化物：1.02b
诺克斯任务：1.02b
沙丘 2000：1.06
皇帝：沙丘之战：1.09
* 魔兽争霸 3 客户端无法连接到 PvPGN 服务器，除非通过 W3L 等工具进行客户端修改以禁用服务器签名验证。 * 由于协议更改，PvPGN-PRO 将不支持从补丁 1.18 开始的星际争霸客户端。包含 1.18.0 versioncheck 条目，以便与 bot 软件兼容。

支持
如果您对 PvPGN-PRO 有任何疑问、建议或任何其他要说的话，请创建一个问题。请注意，D2GS 不是 PvPGN 项目的一部分，因此此处不支持。在获取日志并发布日志之前设置。loglevels = fatal,error,warn,info,debug,tracebnetd.conf

发展
提交拉取请求以参与此项目。尽可能使用 C++11 功能并遵守 C++ 核心准则。

建筑
请参阅 docs/ports.md 了解已确认可与 PvPGN 配合使用的操作系统和编译器。任何支持 WinAPI 或 POSIX 的操作系统，以及任何符合 C++11 标准的编译器都应该能够构建 PvPGN。CMake 文件已经过硬编码，以拒绝早于 Visual Studio 2015 和 GCC 5.1 的编译器。

窗户
使用 Magic Builder。

或者，使用 cmake 生成 .sln 项目并从 Visual Studio 构建它。

cmake -g "Visual Studio 14 2015" -H./ -B./build
这将在 directory 中生成 .sln。build

一般的 Linux
不要盲目地运行这些命令。旧发行版的主要问题是安装 CMake 3.2.x 和 GCC 5，因此示例中使用了外部存储库。

apt-get install git install cmake make build-essential zlib1g-dev
apt-get install liblua5.1-0-dev #Lua support
apt-get install mysql-server mysql-client libmysqlclient-dev #MySQL support
cd /home
git clone https://github.com/pvpgn/pvpgn-server.git
cmake -D CMAKE_INSTALL_PREFIX=/usr/local/pvpgn -D WITH_MYSQL=true -D WITH_LUA=true ../
make
make install
Ubuntu 16.04、18.04
sudo apt-get -y install build-essential git cmake zlib1g-dev
git clone https://github.com/pvpgn/pvpgn-server.git
cd pvpgn-server && cmake -G "Unix Makefiles" -H./ -B./build
cd build && make
Ubuntu 14.04 版本
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
带有 clang 编译器的 Debian 8
sudo apt-get -y install build-essential zlib1g-dev clang libc++-dev git
wget https://cmake.org/files/v3.7/cmake-3.7.1-Linux-x86_64.tar.gz
tar xvfz cmake-3.7.1-Linux-x86_64.tar.gz
git clone https://github.com/pvpgn/pvpgn-server.git
cd pvpgn-server && CC=/usr/bin/clang CXX=/usr/bin/clang++ ../cmake-3.7.1-Linux-x86_64/bin/cmake -G "Unix Makefiles" -H./ -B./build
cd build && make
CentOS 7 操作系统
sudo yum -y install epel-release centos-release-scl
sudo yum -y install git zlib-devel cmake3 devtoolset-4-gcc*
sudo ln -s /usr/bin/cmake3 /usr/bin/cmake
git clone https://github.com/pvpgn/pvpgn-server.git
cd pvpgn-server
CC=/opt/rh/devtoolset-4/root/usr/bin/gcc CXX=/opt/rh/devtoolset-4/root/usr/bin/g++ cmake -G "Unix Makefiles" -H./ -B./build
cd build && make
软呢帽 25
sudo dnf -y install gcc-c++ gcc make zlib-devel cmake git
git clone https://github.com/pvpgn/pvpgn-server.git
cd pvpgn-server
cmake -G "Unix Makefiles" -H./ -B./build
cd build && make
FreeBSD 11 版本
sudo pkg install -y git cmake
git clone https://github.com/pvpgn/pvpgn-server.git
cd pvpgn-server
cmake -G "Unix Makefiles" -H./ -B./build
cd build && make
完整说明： Русский |中文

使用私有 IP 地址在 LAN 或 VPS 上托管
一些 VPS 提供商不会为您的服务器分配直接公共 IP。如果是这种情况，或者您在家中使用 NAT 进行托管，则需要在 中设置路由转换。在寻找游戏时，公网地址会作为路由服务器地址推送给游戏客户端。未能将正确的地址推送到游戏客户端会导致玩家无法匹配和加入游戏（长时间游戏搜索和错误）。address_translation.conf

如果你的网络接口直接绑定到公网 IP，PvPGN 可以自己想办法，而且这一步就不用了。

许可证
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
