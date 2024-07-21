### QBTT: Quinn's Basic TOML Tests for Rust
#### Super-Simple Test Runner 
QBTT runs commands from a TOML and checks to see if they match their expected output on stdout, checksum, and number of lines. QBTT is used by a number of my rust projects (command-line tools), like [ngxav](https://github.com/qpxdesign/ngxav-rs) (a full-featured nginx log explorer) and [webgrep](https://github.com/qpxdesign/webgrep-rs) (a full-browser-spec terminal-based web reader with js and pdf support).

### How to use
install it from cargo: `cargo install qbtt`

create a .toml file with the correct entry syntax (see below)

then run the tests: `qbtt test_cases.toml`

### TOML Syntax
```
[[test_cases]]
name = "Name"
run_type = "lines_count/checksum/output"
cmd = "<path_to_build_des> <args>"
expect = "xxx"
...
```

### Contributing
please report any issues you encounter to the 'issues' tab. We welcome contributions (bug fixes or new features)! just make a pr. 
