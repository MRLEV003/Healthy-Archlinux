# healthy-archlinux-rust

Rust port of the existing Python `hc` read-only Arch Linux diagnostic tool.

Run `hc-rs` for the usage reminder, or `hc-rs -s` for a full scan. Each scan
writes `hclogs-YYYY-MM-DD-HH-MM-SS.txt` to the invoking user's home directory.
The executable invokes only explicit diagnostic commands; it never uses a shell
or runs a package, service, bootloader, filesystem, network, or configuration
modification command.

<img width="1500" height="750" alt="Frame 1" src="https://github.com/user-attachments/assets/2a338f21-f0a0-4b1c-a366-983c87d4f08b" />
