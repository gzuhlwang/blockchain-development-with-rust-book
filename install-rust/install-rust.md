# Windows平台上安装rust

本节介绍在Windows平台上安装rust的关键步骤及注意事项。

## Windows平台上安装rust

1、下载并运行[rustup-init.exe](https://www.rust-lang.org/zh-CN/install.html)，然后按照屏幕上的说明进行操作。

![安装选项](C:\Users\cm\Desktop\paper on smart contract security\blockchain-development-with-rust-book\img\installation-opition.png)

安装完成后，在命令提示符中输入以下命令测试是否安装成功：

> rustc -V

上面的命令是查看Rust的编译器版本。我们采用的编译器版本是最新的稳定版本1.30.1。

> cargo -V   

上面的命令是查看Rust的包管理器cargo的版本。

> rustup -V

上面的命令是查看Rust工具链安装程序rustup的版本。

若上述命令都能输出对应的软件版本，恭喜您，rust安装成功。

## 故障排错

Q1、按照上述安装好rust后，运行rust应用程序时，编译器报error: linker `link.exe` not found 。

A：在windows上，Rust需要Visual C++构建工具2013或更新版本的支持。获取Visual C++构建工具最方便的办法是下载并安装[VC++ Build Tools](https://go.microsoft.com/fwlink/?LinkId=691126)，在安装的时候选择默认就可以了！然后再重新安装rust(rustup_init.exe)。

![下面是安装的VC构建工具](C:\Users\cm\Desktop\paper on smart contract security\blockchain-development-with-rust-book\img\vs-tools.png)

