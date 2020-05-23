# OSC52.vim for Vim and Neovim

This script can be used to send an arbitrary string to the terminal clipboard
using the OSC 52 escape sequence, as specified in
http://invisible-island.net/xterm/ctlseqs/ctlseqs.html, section "Operating
System Controls", Ps => 52.

## Install

### vim-plug

```viml
Plug 'kuntau/vim-osc52'
```

## Mapping

Edit your `.vimrc` to include this code

```viml
vmap <C-c> <Plug>(YankOSC52)
```

This will map Ctrl+C to copy.  You can now select text in vim using the visual
mark mode or the mouse, and press Ctrl+C to copy it to the clipboard.

