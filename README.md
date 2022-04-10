# tonminer
ton挖矿内核平台软件
TON-矿池矿工
来自TON-Pool.com的矿工

指示
在https://github.com/1460293896/tonminer/releases/tag/v.0.0.1 下载我们矿机的最新版本，然后根据您的操作系统运行相应的命令。

# Windows
miner-windows.exe run https://next.ton-pool.club <your_wallet>

# Linux
./miner-linux run https://next.ton-pool.club <your_wallet>
如果您更新了硬件设置（例如超频），或者您不小心运行了我们的矿机两次，请确保benchmark_data.txt在再次运行之前将其删除，以获得最佳哈希率。

Hive 操作系统配置
安装 URL：去发布，复制任何hiveos文件的链接。

钱包和工人模板：%WAL%

矿池网址：https ://next.ton-pool.club

注意：哈希算法将在面板中显示为暗币，但实际上并非如此。

Rave 操作系统配置
转到发布，下载 RaveOS 包，并将其上传到自定义矿工。

创建一个新的钱包，选择我们的矿池，以及新上传的矿工，就可以开始挖矿了。

故障排除
如果矿机无法正常工作，您可以在issues中描述您遇到的问题，并附上矿机输出的截图，以及您的配置信息（显卡型号、操作系统等）

这里也有一些常见的问题和相应的解决方法。

它不适用于我的 AMD GPU
我们正在为此努力。

我无法连接到池
我们有两个挖矿域，https://next.ton-pool.com和https://next.ton-pool.club. 如果任何域不起作用，请尝试切换到另一个域。

我在输出中看到两倍的卡片
尝试添加参数-p 0。

运行 Python 代码
如果要调试矿机，可以直接运行 Python 代码。

您需要安装 Python 3 和 packages pyopencl、numpy和requests。

对于 Linux 用户，您可以运行pip3 install pyopencl numpy requests以安装软件包。如果您正在运行旧版本的 Python，请尝试pip3 install "pyopencl<2018.3"使用pip3 install "numpy<1.15".

对于 Windows 用户，可以运行pip3 install numpy requests安装后面的两个包。您需要访问https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyopencl并下载pyopencl二进制文件。

命令是

python3 miner.py [pool addr] [wallet address]
一个可选的依赖项是websocket-client，如果您安装它，您可以获得更及时的作业获取。

开发费
您可以在任何矿池中使用我们的矿机，但如果您不使用TON-Pool.com，那么您收入的 1% 将捐赠给开发者。
