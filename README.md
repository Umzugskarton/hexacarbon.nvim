# hexacarbon-lua.nvim

For now this readme is mostly a ripoff of the original oxocarbon-lua rewrite by @author: b4mbus. I will add to it as I advance this colorscheme further.

The overall structure is not changed in anyway for now I just add some new highlight groups to add to my favourtite plugins and change some colors.  

## Table Of Contents

- [Installing](#installing)
- [Using](#using)
- [Additional configuration](#additional-configuration)

## Installing

Install using your favourite package manager, e.g. packer:
```lua
use 'Umzugskarton/hexacarbon-lua.nvim'
```
or plug:
```vim
Plug 'Umzugskarton/hexacarbon-lua.nvim'
```

## Using

If you are using lua and the newest `0.8.0` neovim version do:
```lua
vim.cmd.colorscheme 'hexacarbon-lua'
```
Otherwise:
```lua
vim.cmd 'colorscheme hexacarbon-lua'
```

If you have a vimscript configuration this will get the theme running:
```vim
colorscheme hexacarbon-lua
```

## Additional configuration


<details>
	<summary><b>Disabling terminal colors</b></summary>

<br/>

The original theme sets the terminal colors to hexacarbon's pallete, but it seems like a lot of tools use only the few first (black and white), which can make the usage of the terminal really annoying.
```lua
vim.g.hexacarbon_lua_keep_terminal = true
```
or
```vim
let g:hexacarbon_lua_keep_terminal = 1
```

</details>


<details>
	<summary><b>Disabling italics</b></summary>

<br/>

```lua
vim.g.hexacarbon_lua_disable_italic = true
```
or
```vim
let g:hexacarbon_lua_disable_italic = 1
```

</details>

<details>
	<summary><b>Enabling transparency</b></summary>

<br/>

```lua
vim.g.hexacarbon_lua_transparent = true
```
or
```vim
let g:hexacarbon_lua_transparent = 1
```

</details>

<details>
	<summary><b>Alternative telescope style</b></summary>

<br/>

The original's telescope looks like this:
![Original telescope](../media/telescope-normal.png?raw=true)

With this variable set it will look like this:
![Original telescope](../media/telescope-alternative.png?raw=true)

```lua
vim.g.hexacarbon_lua_alternative_telescope = true
```
or
```vim
let g:hexacarbon_lua_alternative_telescope = 1
```

</details>
