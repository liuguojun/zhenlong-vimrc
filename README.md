This zhenlong's vimrc


My personal Vim configurations and some plugins which I used in my daily job.

I put Vim related settings in `plugin/settings/Settings.vim`, and isolate other plugins' settings in `plugin/settings` directory.



## Usage

### Installation and Requisites:

1. BACKUP your `.vim` directory and `.vimrc` first.(IMPORTANT!)

2. `cd ~` to change directory to your home directory.

3. copy files to your home directory:

        git clone vundle

4. cd to `zhenlong-vimrc` directory and execute the `:BundleInstall!  ` to get latest version modules:

5. link the vimrc to

        ln -s .vim/vimrc .vimrc


### Update:

1. :BundleInstall  --init
2. :BundleInstall! --update

### Features and Key Mappings:

1. Resize splited windows automatically, so that you  get a bigger editing room if you're working with a smaller screen. (stole from [Gary Bernhardt](https://github.com/garybernhardt))

2. Toggle between working mode and presentation mode by `<leader>z`, but only work in GUI version Vim.

3. some usually used key mappings in normal mode:

    a. `<F1>` to toggle a Calendar window on and off.

    b. `<F2>` to toggle NERDTree on and off.

    c. `<F4>` to toggle Taglist window.

    d. `<F5>` is the script runner, according to it's filetype, it will run Ruby(*.rb) ,Python(*.py) or Javascript(*.js) file(SpiderMonkey is needed), even CoffeeScript(*.coffee, but you may have to install CoffeeScript first). If the filetype is VimScript, `<F5>` will run `:source %` for you.

    e. `<F7>` to switch to previous tab, and `<F8>` to the next tab.

    f. hit `<ctrl>p` will launch a quick window to match keywords from your current working directory, not only file name, but also path name. And `<ctrl>w u` will match from your MRU(Mostly Recent Used) files, which is also frequently used.

    g. hit `<leader>` twice to toggle comment on and off.

    h. `<tab>` and `<shift><tab>` to increase and decrease the syntax identation.

    i. `<leader>v` to open `.vimrc` in a new tab.

    j. `<leader>0` to edit or create `README.md` in current working directory.

    k. `<leader>s` for ack search
    l. `<leader>f` for nohlsearch
    m.

4. Remove tailing whitespace automatically while saving.

## FAQ

if you can not found `ctags` command, just find your ctags path and replace my settings in `plugin/settings/Ctags.vim` file:

    let Tlist_Ctags_Cmd = '/your/path/to/ctags'

and [Exuberant Ctags](http://ctags.sourceforge.net/) is recommended.

## Contact

Enjoy it, and if there's any question or comment, feel free to let me know :)
