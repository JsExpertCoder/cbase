# CBase

**CBase** is a Vim plugin designed to quickly insert a starter template for C programming exercises, specifically tailored for 42 School projects.

## Features
- Inserts a clean and minimal C starter template at line 14 (after you insert the header):
```c
#include <unistd.h>

int     main(void)
{
        return (0);
}
```
- Saves time when setting up repetitive C programming exercises.

## Installation

### Using [vim-plug](https://github.com/junegunn/vim-plug)

Add a vim-plug section to your `~/.vimrc` (or `~/.config/nvim/init.vim` for Neovim)

1. Begin the section with `call plug#begin()`
1. List the plugins with `Plug` commands
1. End the section with `call plug#end()`

For example,

```vim
call plug#begin()

" List your plugins here
Plug 'JsExpertCoder/cbase'

call plug#end()
```

Reload the file or restart Vim, then you can,

* `:PlugInstall` to install the plugins
* `:PlugUpdate` to install or update the plugins
* `:PlugDiff` to review the changes from the last update
* `:PlugClean` to remove plugins no longer in the list

### Manual Installation

1. **Open your terminal:**

    Open a terminal window on your system. 

2. **Download the plugin repository:**

    Run the following command in the terminal to download the repository:

    ```bash
    git clone https://github.com/JsExpertCoder/cbase.git
    ```

3. **Move the plugin to the Vim runtime path:**

    Copy the `cbase` folder into the `~/.vim/pack/plugins/start/` directory:

    ```bash
    mv cbase ~/.vim/pack/plugins/start/
    ```

    For Neovim, use this directory instead:

    ```bash
    mv cbase ~/.local/share/nvim/site/pack/plugins/start/
    ```

4. **Restart Vim or Neovim:**

    Close and reopen Vim or Neovim to load the plugin automatically.


## Usage

1. Insert the Header:
 Press **F1** or run : **StdHeader** to insert your 42 School project header.
2. Insert the Template:

- Press **CBase** to **insert** the C starter template.

- Alternatively, run the command:
```vim
:Cbase
```
### Notes
- Ensure that your header is inserted first to maintain 42 School coding standards.
- This plugin assumes the C code starts after line 14 (common for projects at 42 School).
