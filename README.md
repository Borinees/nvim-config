# nvim-config

My personal Neovim configuration

## Requirements

The following dependencies are required:

- Neovim
- Rust
- Tree-sitter CLI
- JDK - required for Java development
- JDTLS - required for Java development

### Rust

Install Rust using `rustup`:
```sh
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

You can verify the installation with:

```sh
rustc --version
cargo --version
```

### Tree-sitter CLI


The Tree-sitter CLI can be installed using [`cargo-binstall`](https://github.com/cargo-bins/cargo-binstall):

```sh
cargo binstall tree-sitter-cli
```

Alternatively, you can build it from source:
```sh
cargo install --locked tree-sitter-cli
```

Verify the installation:
```sh
tree-sitter --version
```

## Java Support

Java support requires JDK and JDTLS

### JDK

Install a JDK using your distro's package manager

For Arch Linux:
```sh
sudo pacman -S jdk-openjdk
```

Verify the installation:
```sh
java --version
javac --version
```

### JDTLS

You can install JDTLS using your package manager or build it from the [`official github repository`](https://github.com/eclipse-jdtls/eclipse.jdt.ls)

For arch you can use an AUR helper such as `yay` or `paru`:
```sh
yay -S jdtls
```

or:
```sh
paru -S jdtls
```

> [!WARNING]
> If installing from AUR, always review the PKGBUILD before installing them.

## Java Build Tools

Depending on the Java project you are working with, you may also need a build tool such as Apache Maven or Gradle

### Maven

For Arch Linux:
```sh
sudo pacman -S maven
```

### Gradle

For Arch Linux:
```sh
sudo pacman -S gradle
```

## Installation 

Clone this repository into your Neovim configuration directory:

```sh
git clone https://github.com/Borinees/nvim-config ~/.config/nvim
```