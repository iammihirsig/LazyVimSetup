![image](https://github.com/user-attachments/assets/ac0caa09-c1a1-4436-a23b-262dfa54eee4)


# LazyVimSetup

This repository contains my personal configuration for LazyVim, a Neovim setup powered by [lazy.nvim](https://github.com/folke/lazy.nvim), designed to streamline and enhance my daily development workflow.

---

## 🚀 Features

* **Modular Configuration**: Easily extendable and customizable setup using `lazy.nvim`.
* **Optimized Performance**: Blazing fast startup time and responsive editing experience.
* **Pre-configured Plugins**: Comes with a curated set of plugins ready to use.
* **Sane Defaults**: Includes sensible default settings for options, autocmds, and keymaps.
---

## 📦 Requirements

* **Neovim**: Version 0.9.0 or higher (built with LuaJIT).
* **Git**: Version 2.19.0 or higher (for partial clones support).
* **Nerd Font**: Optional, but recommended for better UI.
* **C Compiler**: Required for `nvim-treesitter`.

---

## ⚙️ Installation

### 1. Backup Existing Configuration

Before installing, it's advisable to back up your current Neovim configuration.

```bash
mv ~/.config/nvim ~/.config/nvim.bak
mv ~/.local/share/nvim ~/.local/share/nvim.bak
```



### 2. Clone the Repository

Clone this repository into your Neovim configuration directory.

```bash
git clone https://github.com/iammihirsig/LazyVimSetup ~/.config/nvim
```



### 3. Remove Git Metadata

To prevent accidental commits or pushes, remove the `.git` directory:

```bash
rm -rf ~/.config/nvim/.git
```



### 4. Launch Neovim

Open Neovim to initialize the configuration.

```bash
nvim
```



LazyVim will automatically install the necessary plugins on the first launch.

---

## 🧩 Configuration

The configuration is organized as follows:

```
~/.config/nvim
├── init.lua
└── lua
    ├── config
    │   ├── autocmds.lua
    │   ├── keymaps.lua
    │   ├── lazy.lua
    │   └── options.lua
    └── plugins
        ├── spec1.lua
        ├── spec2.lua
        └── ...
```



* **`init.lua`**: Main entry point for the configuration.
* **`lua/config/`**: Contains core configuration files for options, keymaps, and autocommands.
* **`lua/plugins/`**: Houses individual plugin specifications.

You can customize your setup by modifying or adding new Lua files in the appropriate directories.

---

## 📚 Resources

* **LazyVim Documentation**: For detailed information and advanced configurations, refer to the [LazyVim documentation](https://lazyvim.github.io/).
* **Starter Template**: Explore the official [LazyVim starter template](https://github.com/LazyVim/starter) for a clean slate setup.
* **Walkthrough Video**: Watch a comprehensive walkthrough by [@elijahmanor](https://twitter.com/elijahmanor) to get started.
* **Book**: Read *LazyVim for Ambitious Developers* by [@dusty-phillips](https://github.com/dusty-phillips) for an in-depth guide.

---

## 📝 License

This configuration is licensed under the [Apache-2.0 License](LICENSE).
