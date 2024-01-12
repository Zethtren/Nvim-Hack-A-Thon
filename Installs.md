# Things to install

<!--toc:start-->

- [Things to install](#things-to-install)
  - [Nerd Fonts](#nerd-fonts)
  - [Terminal](#terminal)
  - [Neovim](#neovim)
  - [LazyVim](#lazyvim)
  <!--toc:end-->

## Nerd Fonts

[NF](https://github.com/tonsky/FiraCode/wiki/Installing)

Gives you ligatures + symbols in terminal.

## Terminal

MacOS / Linux
[Terminal Kitty](https://sw.kovidgoyal.net/kitty/binary/)
[Kitty Conf](https://sw.kovidgoyal.net/kitty/conf/)
To use nerd font set `font_family FiraCode Nerd Font`

MacOS / Linux / Windows
[WezTerm](https://wezfurlong.org/wezterm/installation.html)
[WezTerm Config](https://wezfurlong.org/wezterm/config/files.html)
To use nerd font. Copt all of the first quickstart block. Replace
`config.color_scheme = 'AdventureTime'`
with
`config.font = wezterm.font 'Fira Code'`

## Neovim

[Neovim](https://github.com/neovim/neovim/blob/master/INSTALL.md)

## LazyVim

[LazyVim](https://www.lazyvim.org/installation)

This will give us a ton of great features some of which I have in the docs.
After you install you may get some errors if things are missing and I will help walk through this on a per user basis.

The plugins that I use and recommend are

- coding.yanky,
- editor.aerial,
- editor.leap,
- formatting.black,
- both lang.python's
- lsp.none-ls

If you want things to feel a little more VS Code like ui.edgy can be added (This integrates well with both of the debuggers but, I have little experience here. I am more than happy to help you configure it though.)
