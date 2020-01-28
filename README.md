# (WIP) Nix Special Runtime Linker

This is a little program which is intended to be in `/lib/ld-linux.so.2` which
just uses nix-index to resolve potential packages needed, and outputs a
nix-expression using buildFHSUserEnv, which could run that program.

## Links

- Inspiration from https://discourse.nixos.org/t/how-to-make-nixos-so-easy-that-people-can-be-productive-up-front-without-having-to-first-learn-the-nix-language
- Nix-inndex https://github.com/bennofs/nix-index
- Creating a shared library with Rust https://doc.rust-lang.org/1.5.0/book/rust-inside-other-languages.html
- Rust ELF https://github.com/cole14/rust-elf
