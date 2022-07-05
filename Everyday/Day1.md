# 整理与计划
## 第一阶段
[训练营](https://github.com/LearningOS/rust-based-os-comp2022/blob/main/scheduling.md)

[issues](https://github.com/LearningOS/rust-based-os-comp2022/issues/)

[基于Rust语言学习和实践操作系统内核](https://github.com/LearningOS/rust-based-os-comp2022)

[RUST进行系统编程的自学资源](https://github.com/rcore-os/rCore/wiki/study-resource-of-system-programming-in-RUST)

[Rust语言圣经](https://course.rs/about-book.html)

[Rustling小练习classroom](https://classroom.github.com/a/YTNg1dEH)

[classroom使用视频](https://www.bilibili.com/video/BV1fY4y1n7up?share_source=copy_web&vd_source=2be4a217a97aeb225551786e1fa8e967)


# 安装RUST
## Windows没有行通
## Linux安装
1.sudo apt install curl
2.curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
  如果出现错误：
  curl: (23) Failure writing output to destination
  rustup: command failed: downloader https://mirrors.ustc.edu.cn/rust-static/rustup/dist/x86_64-unknown-linux-       gnu/rustup-init /tmp/tmp.NYHsHHrYc1/rustup-init x86_64-unknown-linux-gnu
  解决：
  确认一下你的curl是不是用snap安装的：
  sudo snap list | grep curl

  如果是，卸载：
  sudo snap remove curl

  然后用apt重新安装：
  sudo apt install curl

  如果出现“无法下载”，执行
  sudo apt-get update

