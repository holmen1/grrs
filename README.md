# Hello Rust Project

This project is a simple Rust application that demonstrates command-line argument parsing and file handling taken from the [cli-book](https://rust-cli.github.io/book/index.html)

## Prerequisites

- [Rust](https://www.rust-lang.org/tools/install) (including `cargo`)

## Creating the Project

To create a new Rust project, run:

```bash
cargo new grrs
```

## Running the Project
To run the project with specific arguments, use:
```bash
cargo run -- <pattern> <file>
```

## Testing the Project
To run the tests, use:
```bash
cargo test
[...]
running 2 tests
test file_doesnt_exist ... ok
test find_content_in_file ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s
```


## Building the Project
To build the project in release mode, run:
```bash
cargo build --release
```

## Adding the Binary to PATH
To add the compiled binary to your PATH, you can either move it to a directory that's already in your PATH or add the build directory to your PATH.

Option 2: Add Build Directory to PATH
Add the release build directory to your PATH:
```bash
export PATH=$PATH:/home/holmen1/repos/grrs/target/release
```
You can add this line to your ~/.bashrc or ~/.profile to make it permanent.

## Running the Binary
After adding the binary to your PATH, you can run it from anywhere:

For example:
```bash
grrs la ~/.bashrc 
alias ll='ls -lat'
#alias la='ls -A'
```
