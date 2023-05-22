# RUST-NOTE

> 鲁迅说过：“好记性不如烂笔头，学东西也做好笔记”

开这个 PROJECT 主要是为了给我那杂乱无章的 RUST 知识做一份梳理，充当一份备忘录的功能。

以下是我学 Rust 的几个重要途径（持续更新中...）:

[1. Rust 语言圣经](https://course.rs/about-book.html)

[2. Rust 程序语言设计](https://kaisery.github.io/trpl-zh-cn/)

[3. 这个 B 站视频教程很不错，推荐一下，是 2 的视频版，觉得看书枯燥可以试试...](https://www.bilibili.com/video/BV1hp4y1k7SV/?spm_id_from=333.788.recommend_more_video.0&vd_source=4e58e9f5189db560a6838eca8f86969d)

我学习 RUST 就靠上面几个链接 + Chatgpt + BingAI(更加推荐 BingAI)。

# GET-START

1. git clone 本仓库

```shell
git clone https://github.com/kunfan96/rust-note.git
```

2. 下载 RUST 插件依赖

运行项目

```shell
cargo install mdbook
```

测试 demo 代码

```shell
cargo install cargo-script
```

3. 运行项目

```rust
mdbook serve -p 3001
```

4. 测试代码

```
cargo script demo/xxx.rs
```

5. 打开[该地址](http://localhost:3001)

6. 如果可以点个 ⭐️
