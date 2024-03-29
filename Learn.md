### 安装rust

1. 命令行安装

   ```
   curl https://sh.rustup.rs -sSf | sh
   ```

2. 安装过程中会出现如下信息：

   ```
   Current installation options:
      default host triple: x86_64-unknown-linux-gnu
        default toolchain: stable
     modify PATH variable: yes
   1) Proceed with installation (default)
   2) Customize installation
   3) Cancel installation
   ```

3. 选择1 继续安装。

4. 安装完成后会提示如下信息：

   ```
   source $HOME/.cargo/env
   ```

5. （按需）重启系统 打开终端输入`rustup`查看效果，如果命令未找到，按如下方式为当前用户添加path。

   ```
   sudo vi /etc/profile。
   // 在文件结尾 添加如下内容
   export PATH="$HOME/.cargo/bin:$PATH"
   ```

运行：
```
ssc@ssc-root-> cargo build
ssc@ssc-root-> cargo build --release # 这个属于优化编译
ssc@ssc-root-> ./target/debug/hellorust.exe
ssc@ssc-root-> ./target/release/hellorust.exe # 如果前面是优化编译，则这样运行
ssc@ssc-root-> cargo run # 编译和运行合在一起
ssc@ssc-root-> cargo run --release # 同上，区别是是优化编译的
```


### 简单学习和使用

1. 参考<https://www.rust-lang.org/zh-CN/learn/get-started>
2. 极客学院 http://wiki.jikexueyuan.com/project/rust-primer/quickstart/rust-travel.html

1. ```
   curl https://sh.rustup.rs -sSf | sh
   ```

    