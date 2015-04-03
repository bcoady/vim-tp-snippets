# VIM-TP-SNIPPETS

A snippet file of commonly used FANUC TP commands

## Installing and Using

- Install [pathogen](http://www.vim.org/scripts/script.php?script_id=2332) into '\vimfiles\autoload' and add the
   following line to your `_vimrc`:

        call pathogen#infect()

- Install [snipmate](https://github.com/garbas/vim-snipmate.git) into `vimfiles\bundle`

- Add the snippets folder to `vimfiles\bundle\vim-snipmate-master`
   Note: the snippets are all caps. Adding the following to your `_vimrc` will give you a separate caps-lock while in insert mode:

      
        
        "ctrl-6 is the new Caps Lock for insert mode only
        " Execute 'lnoremap x X' and 'lnoremap X x' for each letter a-z.
        for c in range(char2nr('A'), char2nr('Z'))
         execute 'lnoremap ' . nr2char(c+32) . ' ' . nr2char(c)
         execute 'lnoremap ' . nr2char(c) . ' ' . nr2char(c+32)
         endfor
         :set iminsert=1
         
      

- Edit the snipptes.tp file to see what snippets are available and to add or edit snippets

- If not already done, install [vim-tp-fanuc](https://github.com/onerobotics/vim-tp.git) into `vimfiles\bundle` for syntax highlighting

## License ##

MIT
