### cargo创建项目
```rust
$ cargo new hello_cargo
$ cd hello_cargo
```
+ 生成一个 Cargo.toml 文件，一个 src 目录，以及位于 src 目录中的 main.rs 文件。

### ```cargo build```构建项目
```rust
$ cargo build
   Compiling hello_cargo v0.1.0 (file:///projects/hello_cargo)
    Finished dev [unoptimized + debuginfo] target(s) in 2.85 secs
```
+ Cargo将根据项目的配置文件（Cargo.toml）编译代码，并会在 target/debug/hello_cargo 下创建一个可执行文件，而不是放在目前目录下

### 运行cargo项目
```rust
$ ./target/debug/hello_cargo # 或者在 Windows 下为 .\target\debug\hello_cargo.exe
Hello, world!
```

### ```cargo run``` 命令，一次性完成代码编译和运行的操作
```rust
$ cargo run
    Finished dev [unoptimized + debuginfo] target(s) in 0.0 secs
     Running `target/debug/hello_cargo`
Hello, world!
```
### ```cargo check```快速检查代码确保其可以编译，但并不产生可执行文件
```rust
$ cargo check
   Checking hello_cargo v0.1.0 (file:///projects/hello_cargo)
    Finished dev [unoptimized + debuginfo] target(s) in 0.32 secs
```
